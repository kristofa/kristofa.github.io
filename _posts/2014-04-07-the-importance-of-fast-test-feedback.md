---
layout: post
title: The importance of fast test feedback
tags: [testing, softwaredevelopment, feedback]
---

Fast feedback is very important during software development. The [Agile Manifesto](http://agilemanifesto.org/) has several principles that stress the importance of fast feedback which results in validating sooner that what we are building works and is what our customer wants.

One aspect of fast feedback is that the tests that we write that prove our software works and avoid regression should complete fast.  This is especially important if you are working towards implementing [Continuous Delivery](http://en.wikipedia.org/wiki/Continuous_delivery). If you don't have fast test feedback the Continuous Delivery setup won't scale as it will take too much time to get feedback for every commit and your build queue will pile up.

To accomplish fast test feedback we should get most of the feedback from low-level unit tests or single component integration tests as opposed to end-to-end tests.

Advantages of unit tests vs end-to-end tests:
   * Unit tests run quickly.
   * They are fine grained. It is easier to spot the root cause in case of test failures.
   * No need for complicated set-up and no external dependencies: tests are deterministic and everything is stored in version control.
   * Tests can be run on developer's laptop without relying on external dependencies (or the library dependencies are pulled in by your favourite build tool). This improves scalability of the development process as developers can execute tests locally.


## Single component integration tests: dealing with integration points

When you only rely on unit tests you will not be sure your component will work end-to-end.

Creating one or more single component integration test will help but than you need to have a strategy to deal with your integration points (databases, external services, files). Some possibilities:

   * mocking the dependent system: when relying on external services you can can implement a mock service that returns predefined results. Depending on the implementation of the mock service it can support returning hardcoded results or record requests/responses and replay them.  The mock server can be started/set-up from within your tests and everything remains in version control.  For implementations that support http services, see [mock-http-server](https://github.com/kristofa/mock-http-server) or [wiremock](https://github.com/tomakehurst/wiremock) (both Java/JVM based).
   * mocking the client: when the client code that communicates with the dependent system has a clear interface you can use a different implementation during tests. For example by changing your dependency injection configuration for the test.
   * in-memory database: In some cases you can replace your database with an in-memory database that's started before running your tests and shut down afterwards.


By adding single component integration tests and using some of the strategies explained before you further decrease the risk of issues in your software while still having the possibility to have everything in version control (source + test code + configuration).

Those single component integration tests should still run fast as you avoid access to other machines or systems.  The tests should also rely only on small amounts of mocked data. They have the purpose of validating the end-to-end integration of the single component and shouldn't be used to test all possible permutations or edge cases which should have been tested by the unit tests.


## No need for end-to-end tests?

You might still need some end-to-end tests which validate that the integration between systems works but you should need very few of them.  As they depend on multiple systems being available and deployed they might not run on a developer's machine and are more likely to break.

## To conclude

If you spot a missing test you should try to add it at the lowest level possible which is as a unit test and try to avoid having to create new single component integration tests or end-to-end tests.

See also the [Test Pyramid](http://martinfowler.com/bliki/TestPyramid.html) blog post.