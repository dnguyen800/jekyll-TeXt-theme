---
layout: article
title: Tablets
category: gadgets

---

## Tablets
**Published on xx/xx/2019**

**Competitors in this space:** Apple, Amazon, Google partners

I’ve personally tested the following:

- Amazon Fire HD10, HD8, HD7
- Apple iPad 6th Gen, iPad Mini
- LG G Pad 7.0 (a really old tablet)

### Overview
When I first started planning for a smart home, I knew I needed tablets—to put on the wall, a stand, my body—wherever it made sense. A smart home without tablets was blasphemy, I thought. Even though I didn’t have a good use for a tablet before, I thought having a dedicated tablet would make it useful, or at least be nice to show off the smart home.  With that in mind, I bought a bunch of tablets during Black Friday to see how useful they would be.

I started off with many tablets, but have since downgraded to two: one iPad 9.7” for my room and one Amazon Fire HD8 for the media center. I also use cheap Android phones (the LG Rebel 4 is an amazing value at $15) around the house as music and TV remotes.

Finding the right spot for a tablet takes time, so hold off on wall mounting projects until settling on a location. I decided against mounting tablets because of the cost and it would be too far away to be convenient to use. Living in a rental is also an obstacle against wall-mounting.

I tried using the tablets in every way possible—as a voice assistant, security camera, and replacement laptop, but eventually settled on using the tablet in three ways:

- Home Assistant dashboard to view weather, traffic, upcoming events, and media.
- Media center dashboard and remote control to view the music and TV currently playing.
- Watch videos through streaming apps and cast to TV 

An expensive tablet can do all three tasks, but a cheap tablet can have some difficulties performing. For that reason, I have tablet recommendations for two categories: budget and expensive. Let’s start with the expensive recommendation.

#### Safety Warning
There is a risk to keeping tablets or phone always plugged into a power source as the battery can swell and potentially explode. Keep a close eye of bulging batteries and unplug the tablet once every few weeks to let the battery discharge.

#### Considerations before buying a tablet
- If you have an old tablet lying around, use it as a Home Assistant display.
.

#### What you get with a tablet
- A dedicated home automation dashboard.
- A portable media viewing device.

### Apple iPad (6th Generation)

![](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1547224207188_tablet-ipad-photo.jpg)


The latest Apple iPad (6th Generation) is the best tablet for both smart home and general use — if you can afford it. Despite my recommendations for nearly every Google product so far, there is no Android tablet that beats the performance and price of an iPad. The Wirecutter also recommends it for similar reasons—overall performance is blazingly fast, which is crucial for navigating the Home Assistant UI or using video apps. The screen is gorgeous, if not overkill for my needs but worth paying for. You can get a similar high-end Android tablet like the Samsung Galaxy Tab S4, but it will be more expensive ($640) and not worth using solely as a dashboard. The cheapest price for a new entry-level iPad is $260, though used iPads could be found on Craigslist for $200. 

#### Installation and Smart Home Integration
There a native iOS app called the Home Assistant Companion, which displays the Home Assistant UI in full screen without borders. It looks beautiful and makes me glad I purchased an iPad. The app renders the new Lovelace UI with custom modules and cards in tact, without any issues. Custom Lovelace card is an issue with Amazon Fire tablets and required many workarounds to get it functional.

Google Assistant is not and will never be integrated, but you can use use Home Assistant’s Homekit component to connect with Siri and Homekit and control your devices. The Chromecast function is supported, so casting videos and music to Chromecast speakers is possible from every app I tested. Google Home, Roku, and SmartThings iOS apps are present and function as well as the Android version. 

If you are an Apple household, then you can use the iPad as a Homekit hub, which will allow you Homekit access when you are away from home. 

### Amazon Fire HD8 Tablet w/ Special Offers

![](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1547275109462_tablet-amazonfirehd8-photo.jpg)


If you don’t mind a slightly sluggish experience, the Amazon Fire HD8 ($50 on sale) is the cheapest tablet you can get with some acceptable compromises, though setting up workarounds can be a chore and not guaranteed to work in the future. The Fire HD8 is the right size and resolution—not too big, not too small at 1280x800 resolution. There is the smaller Fire HD7 ($30) with an even lower resolution screen, or the larger but still sluggish Fire HD10 ($100) — but having tried both, I think the HD8 remains the best value of the three. 

Looking back, I would get another iPad instead of the Fire HD8, but I have the tablet working now so that the experience is acceptable.

#### Installation and Smart Home Integration
Out of the box, the Fire HD8 cannot run Home Assistant because Google Chrome is needed. Several workarounds needed to get the tablet working close to its potential. Installing the Google Play Store and a new front-end like Nova Launcher can provide an Android-like experience, though it is never as good as a native Android tablet. The problem with workarounds is that they can be broken through Amazon’s system updates.

There are several compromises made to reach the $50 price point. Web browser performance on the Home Assistant UI can range from acceptable to just plain bad after a few days of running without a reboot. Chromecast does not work on some apps like Netflix, even if downloaded from the Google Play store. I still haven’t figured out how to login to the SmartThings app yet, as the Fire HD8’s default Amazon Silk browser cannot load the login page. The terribleness of the Fire OS shows itself in the most unexpected ways, as you can see. 