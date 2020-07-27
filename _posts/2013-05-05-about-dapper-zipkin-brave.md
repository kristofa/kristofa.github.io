---
layout: post
title: About Dapper, Zipkin and Brave
tags: [dapper, zipkin, brave, distributedtracing]
---

In last few months I looked into [Zipkin](https://github.com/twitter/zipkin/) which is a 'Distributed Systems Tracing' framework implementation open sourced by [Twitter](https://www.twitter.com) and implemented based on the [Dapper paper](https://research.google/pubs/pub36356/) published by Google.

While looking into Zipkin I decided to create a Java implementation of the Dapper paper which can integrate with Zipkin so the Zipkin back-end components (mainly data store, query service and web UI) can be reused. My Open Source Java implementation is called [Brave](https://github.com/kristofa/brave).

The Twitter developers added Brave to the [Zipkin wiki](https://github.com/twitter/zipkin/wiki) after which it gained some more popularity... going from 1 star to 28 times starred in less than a week :-)

If you work on a distributed system with lots of services interacting and want to improve observability I advice you to have a look at Dapper / Zipkin / Brave.

