---
layout: article
title: Tablets
short_title: Tablets
excerpt: Some say it's just a big ass phone...
category: [gadgets, home automation]
permalink: /gadgets/tablet
key: gadgets-tablet
aside:
  toc: true
banner: assets/images/overlay/tablet.jpg
mode: immersive
header:
  theme: dark
article_header:
  type: overlay
  theme: dark
  background_color: '#203028'
  background_image:
    gradient: 'linear-gradient(135deg, rgba(34, 139, 87 , .4), rgba(139, 34, 139, .4))'
    src: /assets/images/overlay/tablet.jpg
---

<!--more-->

**Competitors in this space:** Apple, Amazon, Google partners

I’ve personally tested the following:

|---
| ![](\assets\images\logo\amazon-fire.png){:.image--lg} |  ![](\assets\images\logo\apple.png){:.image--sm} | ![](\assets\images\logo\lg.png){:.image--md}
|:-:|:-:|:-:
| **Fire HD10 (2017)**<br> **Fire HD8 (2017)**<br>**Fire HD7 (2017)** | **iPad 9.7"  6th Generation**<br>**iPad Mini 4** | **G Pad 7 (2015)**

### What you need to know
When I first started planning for a smart home, I knew I needed tablets—to put on the wall, a stand, my body—wherever it made sense. A smart home without tablets was blasphemy, I thought. Even though I didn’t have a good use for a tablet before, I thought having a dedicated tablet would make it useful, or at least be nice to show off the smart home.  With that in mind, I bought a bunch of tablets during Black Friday to see how useful they would be.

I started off with many tablets, but have since downgraded to two: one iPad 9.7” for my room and one Amazon Fire HD8 for the media center. I also use cheap Android phones (the LG Rebel 4 is an amazing value at $15) around the house as music and TV remotes.

Finding the right spot in the house for a tablet takes time, so hold off on wall mounting projects until settling on a location. I decided against mounting tablets because of the cost and the fact that it would be too far away to use. That, and living in a rental also prevents me from mounting anything to a wall. 

Tablets seem to be versatile, so I tried using the tablets in every way possible—as a voice assistant, security camera, and replacement laptop, but eventually settled on using the tablet in three ways:

> - Home Assistant dashboard to view weather, traffic, upcoming events, and media.
> - Media center dashboard and remote control to view the music and TV currently playing.
> - Watch videos through streaming apps and cast to TV 

An expensive tablet can do all three tasks, but a cheap tablet can have some difficulties performing just one task. For that reason, I have tablet recommendations for two categories: budget and premium. You can probably guess what the premium recommendation will be.

{:.warning}
There is a risk to keeping tablets or phone always plugged into a power source as the battery can swell and potentially explode. Keep a close eye of bulging batteries and unplug the tablet once every few weeks to let the battery discharge.

### Considerations before buying a tablet
> - If you have an old tablet lying around, re-use it as a Home Assistant display.


### What you get with a tablet
> - A dedicated home automation dashboard.
> - A portable media viewing device.

## Apple iPad 9.7" (6th Generation)

![](\assets\images\product-photo\ipad.jpg){:.image--xl.align-left}

**The latest Apple iPad (6th Generation) is the best tablet for both smart home and general use — if you can afford it.** Despite my recommendations for nearly every Google product so far, there is no Android tablet that beats the performance and price of an iPad. [The Wirecutter](https://thewirecutter.com/reviews/best-tablets/) also recommends it for similar reasons—overall performance is blazingly fast, which is crucial for navigating the Home Assistant UI or using video apps. The screen is gorgeous, if not overkill for my needs but worth paying for. You can get a similar high-end Android tablet like the Samsung Galaxy Tab S4, but it will be more expensive ($640) and not worth using solely as a dashboard. The cheapest price for a new entry-level iPad is $260, though used iPads could be found on Craigslist for cheaper. 

The iPad also makes for a great multipurpose device. Switching between apps is lightning fast and makes all the difference when jumping from Home Assistant UI to Hulu or Netflix. I find that saving a few seconds of frustration was worth it.

### Installation and Smart Home Integration
There a native iOS app called the [**``Home Assistant Companion``**](https://itunes.apple.com/us/app/home-assistant-companion/id1099568401?mt=8), which displays the Home Assistant UI in full screen without borders, complete with custom modules and Lovelace cards intact. It looks beautiful and makes me glad I purchased an iPad. Custom Lovelace cards are an issue with Amazon Fire tablets and require many workarounds to get it functional. The only downside to this app is that there is still a screen border when using it.

Google Assistant is not and will never be integrated into iOS, but you can use use Home Assistant’s **``Homekit component``** to connect with Siri and Homekit to control your devices. The Chromecast function is supported, so casting videos and music to Chromecast speakers is possible from every app I tested. Google Home, Roku, and the SmartThings iOS apps are present and function as well as the Android equivalents. 

If you are an Apple household, then you can use the iPad as a Homekit hub, which will allow you Homekit access when you are away from home. 

## Amazon Fire HD8 Tablet w/ Special Offers

 ![](\assets\images\product-photo\amazon-fire-hd.jpg){:.image--xl.align-left}

**If you don’t mind a slightly sluggish experience, the Amazon Fire HD8 with Special Offers ($50) is the cheapest tablet you can get with some acceptable compromises, though setting up workarounds can be a chore and not guaranteed to work on all tablet models or in the future.** The Fire HD8 is the right size and resolution—it's not too big, not too small at 1280x800 resolution. The physical size is larger than I imagined.  There is the smaller Fire HD7 ($30) with an even lower resolution screen, and the larger but still sluggish Fire HD10 ($100) — but having tried all three sizes, I think the HD8 remains the best value of the three and the perfect size for a tablet.

Looking back, I would get another iPad instead of the Fire HD8, but I have the tablet working acceptably now.

### The Problems
Out of the box, the Fire HD8 cannot display the Home Assistant UI properly without the Google Chrome browser.  Installing the Google Play Store and a new front-end like Nova Launcher can provide an Android-like experience, though it is never as good as a native Android tablet. The problem with workarounds is that they can be broken through Amazon’s system updates.

There is a new Windows tool called [Amazon Fire Toolbox](https://forum.xda-developers.com/hd8-hd10/development/official-amazon-fire-toolbox-v1-0-t3889604) that removes nearly everything Amazon-related from the tablet. I tried it recently and though it took some time to get it working, it did everything it claimed to do. I'm actually excited to see if this is finally **it (!!!)**  to fix my problems with the Amazon Fire tablets. It doesn't fix the issue with loading custom Lovelace cards, but it fixes nearly everything else.

There are several compromises made to reach the tablet's $50 price point. Web browser performance on the Home Assistant UI can range from acceptable to just plain bad after a few days of running without a reboot. Chromecast does not work on some apps like Netflix, even if downloaded from the Google Play store. I still haven’t figured out how to login to the SmartThings app yet, as the Fire HD8’s default Amazon Silk browser cannot load the login page. The terribleness of the Fire OS shows itself in the most unexpected ways, as you can see. 

### Installation and Smart Home Integration

I was planning to write a guide to cleaning up the Fire HD tablet, but an automated tool called Amazon Fire Toolbox was recently released that does the same job, but much quicker. It only supports a few Fire HD models. These are the steps to installing the necessary apps on a Fire tablet: 

> - Install Nova Launcher as a replacement home screen and Gboard for replacement keyboard. Nova Launcher only costs a few dollars and is one purchase for all devices in one account. Both apps are required for using Amazon Fire Toolbox.
> - Download and use Amazon Fire Toolbox on your tablet. It is complicated to setup (requires Windows PC,ADB drivers installed, ADB enabled in Developer Options, anti-virus disabled, ADB checks disabled, authorize PC), but it automates nearly every task you need to perform to debloat the tablet, disable auto-updates, remove lockscreen ads and install Google Play Store. My Fire HD8 is noticeably faster after using this tool. Doesn't work with all Fire HD tablets, but works with recent HD8 models.
> - Use Google Chrome app to create a webapp by accessing the Home Assistant webserver, then select the option **``Add to Homescreen``**. This creates a browser view that removes the browser tabs normally found on Google Chrome.
> - **``Optional``** Use the GMD Full Screen Immersive Mode app to remove borders and provide a full screen view of Home Assistant. There is a problem though: the screen becomes unresponsive after a few hours and requires you to refresh the page.
> - **``Optional``** Flash your Amazon Fire tablet to another OS. In March 2019, a method was discovered on XDA-Devleopers forum to do so. It requires physically opening the tablet and shorting two points on the circuit board.. There isn't a custom Android rom, so this technique is not useful yet.
> - **``Optional``** Use Fully Kiosk Browser app would be the ideal app for Home Assistant, but due to using an outdated version of Android Web View, custom Lovelace cards do not load in this browser. So close!
> - **``Optional``** The Home Assistant app for Android, called Ariela, also has issues displaying certain custom Lovelace cards on Fire tablets. It is constantly updated so keep an eye on it if it fixes the custom card issue.