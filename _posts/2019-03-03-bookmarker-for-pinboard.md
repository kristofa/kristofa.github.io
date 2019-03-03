---
layout: post
title: Bookmarker for pinboard
tags: [pinboard, safari, safari app extension, macOS]
---

End of last year during my christmas and new year's break I decided to create a macOS Safari App Extension.

I use Safari as my main browser on our home MacBook and had noticed for some time that Safari extensions distributed as `.safariextz` files were not officially supported anymore starting with Safari 12.  You can still install them by using `Extension Builder` after enabling the `Develop` menu but it is a bit cumbersome and it might stop working in future versions.

The new way of writing Safari Extensions is by using the [Safari App Extension Architecture](https://developer.apple.com/documentation/safariservices/safari_app_extensions).  These extensions are developed using Xcode and allow you to use native code ( Objective-C or Swift) besides JavaScript and CSS to inspect, read or manipulate web pages.  Safari App Extensions can also be distributed using the macOS App Store.

I'm a [Pinboard](https://pinboard.in) user and I noticed there was no Safari App Extension yet using the new architecture, or at least I couldn't find one, so I thought it might be an interesting small personal project to try to create a minimal Pinboard Safari App Extension and get it in the App Store. I started the project for 3 main reasons:

   1. I would use the extension a lot myself.
   2. I would learn using a new development environment, programming language,... 
   3. It might be useful for others too.

I succeeded in my goal and my Safari App Extension is available in the App Store since about a week: [bookmarker for pinboard](https://itunes.apple.com/de/app/bookmarker-for-pinboard/id1451400394?l=en&mt=12). 

I decided to make the extension available at no cost and make the code available at my github [kristofa/bookmarker_for_pinboard](https://github.com/kristofa/bookmarker_for_pinboard) and license it under the the Apache 2.0 license.  This allows others to learn and contribute.

As a backend developer with mostly Java, Scala and a bit of Ruby experience it was an interesting project and I learned about:

   * Xcode
   * Swift
   * several of the macOS API's: `URLSession`, `NSUserDefaults`, using KeyChain (to store the API token securely), user interface building.
   * the [Pinboard API](https://pinboard.in/api/)
   * Distributing my App, the App Review Process and the tools at your disposal to find out how well your App is performing.


I made two small improvements since the initial release (issue [#1](https://github.com/kristofa/bookmarker_for_pinboard/issues/1) and [#2](https://github.com/kristofa/bookmarker_for_pinboard/issues/2)), suggestions by one of the first users, which I plan to submit to the App Store soon.  

I use my extension almost daily. If you're a Pinboard / Safari user you might want to check it out: [bookmarker for pinboard](https://itunes.apple.com/de/app/bookmarker-for-pinboard/id1451400394?l=en&mt=12).


