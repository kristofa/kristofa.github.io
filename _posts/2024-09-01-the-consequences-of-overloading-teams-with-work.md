---
layout: post
title: The consequences of overloading teams with work
tags: [productivity, wip, sustainability]
---

_In 2023, we let a company install a Photovoltaic (PV) system (solar panels) on the flat roof of our house.  The team installing the PV system had a packed schedule which resulted in some unexpected consequences which I'll share in this blog post. In a follow-up blog post I'll come up with some suggestions how to avoid overloading a team with work and prevent the negative effects in a product development context._

# A story about the installation of a Photovoltaic system

Around mid-2022 we signed a contract with a company to install a [Photovoltaic (PV) system](https://en.wikipedia.org/wiki/Photovoltaic_system) (solar panels) on the flat roof of our house.

Because of factory closures as a consequence of the Covid-19 lockdown and high energy prices caused by a potential shortage of gas due to the war in Ukraine, the company told us that the demand for PV systems was very high and the waiting time for both the equipment (solar panels, inverter etc.) and installation was going to be long.

Finally, more than 6 months after ordering, they phoned us to make an appointment for installing the PV system in January 2023.

We settled on a date a few weeks later, and they told us they would arrive around 11:30 in the morning. Expected completion time by end of day. The day before the installation someone came and parked an [aerial work platform](https://en.wikipedia.org/wiki/Aerial_work_platform) in front of our house which was going to be used to get all the equipment and people on the roof efficiently the next day.

The next day the craftsmen and the equipment didn't arrive at 11:30 as the project manager had told us but only at 14:30. They had finished another installation in the morning, but it took longer than expected, and so they ended up 3 hours later at our place.

They swiftly started unloading their van and put all the equipment on the aerial work platform. You could see that they were in a hurry. While two people were busy on the roof another person started drilling a hole so the cables coming from the roof could reach our electricity distribution board.

I was working from home that day to make sure they had access to our house and was in a video call when I heard the drilling start. A few seconds later I dropped out of the video call because the Internet connection stopped working. I went to see the man who had been drilling the hole and asked if he by accident cut our Internet connection cable. He hadn't noticed it yet but when he came inside and checked he indeed noticed that he had cut the cable. He excused himself. You could see that he felt bad for not paying more attention. He said that he could not fix the broken cable, which I understood. I called our Internet provider company to explain the issue and to make an appointment to replace the broken cable.

I spent more than 30 minutes waiting on the phone before I could reach someone from our Internet provider. I explained the situation, made an appointment (luckily someone could come over already the next day) and agreed that they could charge the company that was installing the PV system with the cost of replacing the broken cable.

Time passed and around 17:00 they were still busy. Since it was January it was dark already and around 17:30 they came down from our roof and said that they hadn't been able to finish the installation. They told us that they had left everything on the roof and that they had secured it as good as possible to prevent it from blowing off the roof in case of strong winds. When I asked when they would come back to finish the installation they said they couldn't tell because as far as they knew their schedule was packed for the coming weeks.

Finally, more than 3 weeks later we got another appointment, and they came to finalise the installation. It took them another half day to finish everything.

# Consequences

The consequences of overloading teams with work are all negative. 

- People work in stressful situations and become less motivated
   - Installing solar panels should be a rewarding job. The customer is happy because they will end up with a lower energy bill and the work contributes to the transition to renewable energy. But if like in this case the team is burdened by too much work it will soon become demotivating. If the feedback of the team is not taken into account and the situation persists it can lead to employee churn or worse burnout.
- Lower quality
   - because of time pressure and many context switches mistakes are made or work is done less thorough which negatively impacts quality.
- The cycle time (time to value) becomes longer and predictability lowers
   - the schedule was so full that they only could come back 3 weeks later to finalise the installation. It's likely that we were not the only client impacted by the packed schedule which means planning becomes harder and harder and predictability goes down.
- Lower quality leads to lower customer satisfaction
   - the solar panel installation was finished 3 weeks later than expected.
   - we could only benefit from a reduced energy bill weeks later.
   - there was additional work to call the Internet provider (including a 30-minute waiting time on the phone) to restore our Internet.
   - we had one evening without Internet.
   - we had to be home the next day to let someone fix the Internet connection.
   - we had to be home 3 weeks later to finalise the PV system installation.
- More overhead and cost
   - The company had to pay the cost for restoring our Internet connection.
   - They needed to plan another visit to our house to finish the work.
   - The people who came the 2nd time were other people than the 1st time which means they had to get some context first about the situation which probably took more time. Several restarts of the same work including handover to other people are typical indications of too much work in progress.


Besides all these we were still lucky that there was no stormy weather during the 3 weeks that all the equipment was laying on our roof. The cost and delay could have been a lot worse if all or part of the equipment would have blown off our roof.

If you reflect on these consequences I think many of you will probably be able to see similarities with product development environments you've worked in. I definitely do. Some personal examples I experienced from the product / software development domain:

- a migration from Vue.js 2 to Vue.js 3 got started because Vue.js 2 became end-of-life and stopped getting updates. Because the team was working on many things at the same time and there were conflicting priorities there was no capacity for thorough regression testing. For several months bug fixes and new features needed to be implemented in both the Vue.js 2 and Vue.js 3 versions. This resulted in additional work, higher chance of mistakes and a longer time to value.
- the discovery phase of an initiative got started and stopped multiple times over the period of 1 year. Each time another technical lead gets appointed resulting in a handover and getting familiar with the context over and over again. 
- the functionality for a yearly contract renewal wasn't tested well. It would only be needed a year after launch, there was still time to validate it, and other work was waiting which got started. A year later renewals didn't happen because the assumptions about the integration with a third party were wrong. This resulted in 3 weeks of high priority unplanned work. There was additional work to do manual fixes for the impacted customers whose contracts were cancelled unjustified and work to analyse and fix the implementation, so future renewals would work as expected.

Despite the many unwanted consequences, and despite so much research and material that's available on the subject, many organisations in all kind of domains still fall in the trap of starting too much work.

In a follow-up blog post I'll propose some suggestions on how to avoid too much work in progress in a product development context.


------
Reading tips:
- [THIS IS LEAN](https://thisislean.com) by Niklas Modig and Pär Åhlström. A small but beautiful book with nice illustrations about the efficiency paradox. The fact that the busier we are, the more inefficient we become. It also includes great inspiring examples.
- [The Principles of Product Development Flow](https://www.goodreads.com/book/show/6278270-the-principles-of-product-development-flow) by Donald G. Reinertsen. Not an easy read but a fundamental book in which many solid principles are explained to improve product development flow. Thanks to Tom Stuart and Matt Weiden for bringing it to my attention during my time at SoundCloud.

Viewing tips:
- [Henrik Kniberg: Multiple WIP vs One Piece Flow Example](https://www.youtube.com/watch?v=Yqi9Gwt-OEA&t). Seven-minute video by Henrik Kniberg that clearly shows why too much WIP is inefficient.