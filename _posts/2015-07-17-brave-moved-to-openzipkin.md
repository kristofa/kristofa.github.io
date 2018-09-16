---
layout: post
title: Brave moved to OpenZipkin org
tags: [zipkin, brave, openzipkin, distributedtracing]
---

Yesterday I moved brave from https://github.com/kristofa/brave to [https://github.com/openzipkin/brave](https://github.com/openzipkin/brave)

I started brave in April 2013 after I saw the [Zipkin video](http://www.infoq.com/presentations/Zipkin) but soon found out that integrating Zipkin in a Spring Java app was not that straight forward.  I started it on github thinking it might be useful to others... and here we are today:


   * Brave has 229 stars
   * Has 13 releases published to Maven central
   * Has 14 contributors
   * Has 44 closed pull requests
   * Has 32 closed issues
   * It is or has been used in production by several companies (Finn.no, Flipkart,...)

Reasons why I decided to move brave to the openzipkin github org:

   * I'm not maintaining any services anymore that use brave in production.  At [SoundCloud](https://soundcloud.com/) we [use Finagle](https://developers.soundcloud.com/blog/building-products-at-soundcloud-part-3-microservices-in-scala-and-finagle) so there is no need to use Brave. I prefer not to be the only contributor with commit rights for a project I don't use anymore myself.  By moving it to openzipkin we open it up.
   * open-zipkin is an excellent initiative that I see as being very positive for the open source distributed tracing space. [It gets supported by Twitter](https://groups.google.com/forum/#!msg/zipkin-dev/fbOgEZpuQx4/QpwqDYktRjIJ) and has members of different companies including myself. The people part of the community are there because they are passionate about building good open source distributed tracing solutions. So they have the same purpose as I have with brave.
The move to the openzipkin org does not mean I will abandon brave. I still have planned to finish and release [brave 3.0.0.](https://github.com/openzipkin/brave/issues/59) And as being part of the openzipkin org I will help with looking into bugs, following up pull requests and participate in discussions. But it will definitely be good that others step in and participate.

\o/

Cheers,
Kristof

_Originally posted [here](http://kdevlog.blogspot.com/2015/07/brave-moved-to-openzipkin-org.html)_