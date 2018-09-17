---
layout: page
title: About me
---


I'm working as an Engineering Manager at [SoundCloud](https://soundcloud.com).
I like to build and support diverse teams and be part of them. 

Having a positive impact is really important for me and there is a lot we can do to make a better and more sustainable future for all of us. I'm interested in organisations and teams that contribute to reach one or more of the [UN Sustainable Development Goals](https://www.globalgoals.org) or work in the field of Social Innovation.

## The story about 'brave'

In 2013 I was confronted with performance problems in a microservices architecture at my employer at that time. The performance problems were hard to nail down and we had no easy way to get insight in the number of internal service requests that were needed to fulfill user requests.  

During that time I saw a presentation about [Zipkin](https://zipkin.io) which was built at Twitter and based on the [Google Dapper paper](https://ai.google/research/pubs/pub36356).  Zipkin looked like it could help us give insight in the performance issues we were facing and I decided to try to integrate it in our Java microservices.  However soon I found out that the Twitter implementation was integrated in [Finagle](https://twitter.github.io/finagle/) and not really reusable in Spring based Java microservices.

That made me decide to create a new Java library called [Brave][1]. I implemented Brave in such a way so that it was compatible with the Twitter Zipkin back-end components used to store/query and visualize trace data and from the start I made it available on github under the Apache Version 2.0 license.  

Once I got a first version working I shared it in the Zipkin google group and it received attention immediately. With many companies adopting a microservices architecture around 2013 / 2014 it seems like it was the perfect moment to start an open source distributed tracing solution that integrated with mainstream technologies like Java Spring.

Brave suddenly got several interested adopters and contributors which was exciting and I spent quite some free time following up community requests, reviewing pull requests and making improvements.  Fairly soon also [Adrian Cole](https://twitter.com/adrianfcole) who worked at Twitter at that time got involved.  He had great suggestions and spent a lot of time helping and contributing.  He became the driving force behind the Zipkin community.

My work on Brave also got the attention of SoundCloud who was also moving to a microservices architecture. After some exchange of emails they invited me to go through the job interview process. This resulted in me moving to Berlin and start working at SoundCloud.

Around mid 2015 all core Zipkin related repositories were moved to the OpenZipkin org and in July 2015 I also moved brave from my personal github account to the OpenZipkin organisation (see my blog post [Brave moved to OpenZipkin org](../2015-07-17-brave-moved-to-openzipkin/)).

I kept working on brave till v3.0.0. After that I started having other priorities and stopped most involvement.  

Brave still exists, is in active development, and is officially integrated in the [Spring framework](https://spring.io) as part of [Spring Cloud Sleuth](https://cloud.spring.io/spring-cloud-sleuth/).

The example of Brave shows how powerful sharing your ideas and work can be.  Besides learning from the community it gave me additional exposure and had a huge impact on my life. I moved to a new country and started a new job which was a great experience.



[1]: https://github.com/openzipkin/brave


