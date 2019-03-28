---
layout: article
title: Cameras
short_title: Cameras
excerpt: You're one step closer to being a paranoid old man now.
category: [security, home automation]
permalink: /security/camera
key: security-camera
aside:
  toc: true
banner: assets/images/overlay/cameras.png
mode: immersive
header:
  theme: dark
article_header:
  type: overlay
  theme: dark
  background_color: '#203028'
  background_image:
    gradient: 'linear-gradient(135deg, rgba(34, 139, 87 , .4), rgba(139, 34, 139, .4))'
    src: /assets/images/overlay/cameras.png
---

<!--more-->

**Image:** The Dark Knight. Warner Bros.

**Quick Links:**
<div class="grid-container">
  <div class="grid grid--p-2">
    <div class="cell cell--3"><a href="security/camera#indoor-camera"><div><div class="card">
      <div class="card__image">
        <img class="image" src="/assets/images/grid/indoor-camera.jpg"  />
      </div>
    </div></div></a></div>
    <div class="cell cell--3"><a href="security/camera#doorbell-camera"><div><div class="card">
      <div class="card__image">
        <img class="image" src="/assets/images/grid/doorbell-camera.jpg"/>
      </div>
    </div></div></a></div>
    <div class="cell cell--3"><a href="/security/camera#outdoor-camera"><div><div class="card">
      <div class="card__image">
        <img class="image" src="/assets/images/grid/outdoor-camera.jpg"/>
      </div>
    </div></div></a></div>    
  </div>
</div>


# Indoor Cameras

**Published on: xx/xx/2019**

**Competitors in this space:** Nest, Ring, Wyze, Arlo, Blink, Laview, D-Link, Hikvision, Xiaomi, Simplisafe, Abode, Canary 

I’ve personally tested the following:

|---
| ![](\assets\images\logo\nest.png){:.image--md} |  ![](\assets\images\logo\wyze.png){:.image--xl} | ![](\assets\images\logo\xiaomi.png){:.image--lg}
|:-:|:-:|:-:
| **Nest Cam Indoor** | **Wyze Cam v2** | **Xiaomi Xiaofang 1080p Camera** 

### What you need to know

For privacy reasons, I am very cautious when it comes to the placement of indoor cameras. In my household, we have a camera in the living room that covers all the entry points into the house while avoiding areas where I and my roommates frequent. With the help of presence sensors, I can turn off the camera when someone is at home. My goal is to provide additional security in my home, not invade the privacy of my household members.

Besides using as a pet or baby monitor, cameras can provide visual confirmation of intruders. I wouldn’t make a 911 call based on sensors alone unless the alarm system wasn’t disabled timely. What if I forgot that a relative was stopping by? 

Even if it was only me being recorded on my camera, it doesn’t feel right to be recorded. Maybe that is because there is the possibility of someone other than me viewing the camera footage. Whether it is a rogue IT admin at the company, someone with access to the servers storing the footage, or a hacker who obtained user credentials or exploited a vulnerability on the camera—it is possible that someone can view your footage without permission.

There is a good selection of cameras at different price ranges. My recommendation is to buy one quality camera and one cheap camera to cover your bases. Though if you’re rich, feel free to go nuts with the cameras and spyng.

### Considerations before buying an indoor camera

> - Consider if the camera placement violates any household member’s privacy.
> - Decide whether you want local or cloud storage features.
> - Cameras can be powered by battery, AC or ethernet cable..
> - Look into the company's free video storage tier offering. Also look into notification features if the camera works locally only.
> - security Do a quick search on the company's history with security vulnerabilities. You will be surprised how many well known companies have gaping security flaws.

### What you get with an indoor camera

> - Monitor the garage to ensure the door is closed. Acts as a  Secondary check of who is coming in/out of the garage.
> - Monitor pets or babies.
> - If a sensor goes off in the house while you’re away, cameras can provide visual verification of intruders.

### Recommended reading

> - Nothing?
> - Homealarmreport.com [article](https://homealarmreport.com/using-wyze-cam-with-and-without-a-microsd-card/) on using Wyze Cam's new features
> - Mozilla's *Privacy Not Included* [Analysis](https://foundation.mozilla.org/en/privacynotincluded/products/wyzecam/) of the WyzeCam

## Nest Cam Indoor
![](\assets\images\product-photo\nest-indoor.jpg){:.image--xl.align-left}

**If you plan to buy only one camera, then get a quality camera that supports continuous recording, like the Nest camera.**  Although I talk about Nest often, that doesn’t mean I recommend them to everyone. There are many similar quality cameras that offer better free storage tiers than Nest—start by checking out the [Wirecutter’s guide](https://thewirecutter.com/reviews/best-wi-fi-home-security-camera/) for other recommendations.

The value of Nest cameras is in its ease of setup and use. There are many issues I have using cheaper cameras—wireless range, connection dropouts, unreliable cloud servers—but I haven’t run into any of those issues with Nest. Once you have the camera plugged in and the Nest app installed, everything works reasonably well out of the box. The Nest app is also lightning fast at loading live and recorded footage—it takes under 10 seconds to load the app, authenticate and access my cameras. I’ll leave it to users to decide whether the improved experience is worth the premium price of Nest products.

<figure style="width: 100%;" >
 <img src="\assets\images\other\nest_aware.png" alt="" />
 <figcaption>
New pricing for Nest Aware monthly plans.
 </figcaption>
</figure>

The Nest Aware monthly service used to be the most expensive of the competition, but at the time of this writing,  Nest introduced a $5/month pricing tier. This is much more affordable and I don’t feel as bad anymore when recommending Nest products to customers. Though if you plan on getting a Ring security system, any camera monthly fees are included with the security monitoring fee. 

Nest sends notifications when the camera is offline (due to power outage, or someone unplugging the cord). It’s a nice feature that other companies have.

### The Problems
There is a Home/away Assist feature on the Nest app, but I found it doesn’t work reliably. There were a few times when I received an alert and opened the Nest app to see my roommate in the living room, watching TV. I’ve done my own testing of the feature (Home Assistant integration gives you access to this data) and found it can take hours for Nest to update to Home or Away status. As phones get more aggressive with battery saving, a lot of apps are going to have trouble with presence detection. Unfortunately Nest has not solved this issue either.

Nest’s motion detection algorithm also left me disappointed. I’ve received false alerts from moving window blinds and sunlight piercing through the windows. There are workarounds with camera placement and angle, but I expected more from a Nest camera.

### Installation and Smart Home Integration

Nest works well with Google Assistant, though there isn’t much need for voice control of a camera, except to broadcast messages or video feeds to a Chromecast. Home Assistant integration works with a Nest developer account, though the Nest camera feed in Home Assistant is only a still image that’s updated every few seconds. It’s better to use the Nest app for viewing live and recorded footage. Nest detection alerts can be tracked in Home Assistant, so you can pair an automation with it, like, blinking the lights when someone is at the door. I never found the need to use it though. 

<figure class="figure figure--25">
 <img src="/assets/images/integrations/nest-indoor-ha.png" alt="Small picture of a kitten" />
 <figcaption>
 <b>Home Assistant: Okay</b><br>It works, but impossible to see real-time footage. What is important is the ‘motion detected’ sensor.
 </figcaption>
</figure>

<figure class="figure figure--25">
 <img src="/assets/images/integrations/google-home.png" alt="Small picture of a kitten" style="width: 100%" />
 <figcaption>
 <b>Voice: Great</b><br>Can send broadcast messages when someone is at the door.
 </figcaption>
</figure>

<figure class="figure figure--25">
 <img src="/assets/images/integrations/nest-indoor-st.png" alt="Small picture of a kitten" style="width: 100%; height: 100%" />
 <figcaption>
 <b>SmartThings: Okay</b><br> NST Manager SmartApp shows camera, but not real-time.
 </figcaption>
</figure>

<figure class="figure figure--25">
 <img src="/assets/images/integrations/nest-indoor-app.jpg" alt="Small picture of a kitten" style="width: 100%" />
 <figcaption>
 <b>Native App: Great</b><br>Simple, easy-to-use
 </figcaption>
</figure>





## Wyze Cam v2

![](\assets\images\product-photo\wyze.jpg){:.image--lg.align-left}

**The Wyze Cam v2 continues to add great value for the price and features it offers—I think everyone should have one as a cheap, spare camera.** Originally, I had a slightly negative opinion about this camera, but the slew of new features added in 2018 like continuous and extended event recording, local storage, make it hard not to change my mind. If Wyze ever releases a high quality camera at an affordable price, then I am on board.

Despite using a cheap camera and hardware, Wyze engineers have figured out reasonable workarounds for previous issues like the 12-second recording time, or the five minute cooldown periods between events. Viewing locally stored footage through your phone's cellular network is possible too! As long as you have a compatible micro SD card (and who doesn’t), the Wyze cam will get these features. [Homealarmreport.com](https://homealarmreport.com/using-wyze-cam-with-and-without-a-microsd-card/) offers a good, detailed breakdown of the features for those interested.

Motion detection works reasonably well, though it takes some testing to find the right settings. In one example, I setup a Wyze camera in an empty apartment to monitor for break-ins. I wanted to detect any large changes, like the opening of a door, but I was getting false alerts from sunlight and weather changes. I eventually found the right sensitivity settings for my needs, though it took some trial and error.

### The Problems
Without an SD card, the original limitations of the camera are back. Recordings are limited to 10 to 12 seconds, with a five minute cooldown between each alert. I've read on the Wyze forums that some people are experiencing SD card failures using the continuous recording feature.  The app is a little slower than Nest, and it takes longer to load live footage, but these are reasonable compromises for a $25 camera..

There is usually a catch when a company offers a camera and free video recordings at an ridiculously low price.  At the time of this writing, all Wyze wants to do is sell you more stuff. The company is expanding its smart home presence with the introduction of low-priced motion and contact sensors and a DIY NAS video storage solution.  That is reasonable strategy that I'm okay with.

The Mozilla Foundation interestingly offers a [privacy-focused analysis](https://foundation.mozilla.org/en/privacynotincluded/products/wyzecam/) on the Wyze camera and rates it as “Meets our minimum security standards.”

I generally do not recommend using any Wyze camera custom firmware as you lose existing functionality. I’ve tried hacks on similar cameras (Xiaofang) and found that the loss of features like automatic night vision, cloud, or reliable motion detection wasn’t worth the trade-off.

### Installation and Smart Home Integration
Viewing camera footage in Home Assistant and SmartThings is not a good experience in general—for that reason, the Wyze app is better for reviewing alerts and accessing camera footage.

Google Assistant integration is coming ~. in beta. ability to stream camera footage onto a Chromecast.


# Doorbell Cameras

Picture here

**Published on: xx/xx/2019**

**Competitors in this space:** Nest, Ring, Securisafe, Laview 

I’ve personally tested the following:

|---
| ![](\assets\images\logo\nest.png){:.image--md} 
|:-:
| **Nest Hello** 

### What you need to know

I’ve installed the Nest Hello doorbell cameras for a few friends and they all love it—I secretly believe it is because of the ability to spy on passerbys. The biggest selling point for me is the piece of mind knowing when and where my package was delivered. While the camera may not stop package theft altogether, at least it makes your house less of a target by being present.

{:.info}
**Before installing a camera, it’s important to be aware of the rules and regulations regarding cameras and external installations. Living in an HOA neighborhood means you likely need approval before installing anything on the outside of your home.**

Installation of doorbell cameras requires more planning, particularly with wired cameras. Consider the location and angle of the doorbell, and whether your home is equipped to support a wired doorbell.  There are solutions for nearly every scenario, though it may require a battery-operated doorbell camera.

### Considerations before buying a doorbell amera

> - Check with your HOA before installing any hardware outside your house.
> - Check with household members about installing any indoor cameras. Privacy should be respected, after all.
> - A good wireless network is needed to avoid wireless range issues. See my router recommendation.
> - Check an online compatibility checker like Nest as not all homes are compatible with wired doorbell cameras. Wireless ones (like the Ring 2) can be installed anywhere.
> - Cameras have decent viewing angles, but check that your doorbell location is ideal for a camera. 

### What you get with a doorbell camera

> - Know when your packages are delivered, and potentially stolen.
> - Know when household members arrive and leave home.
> - Send a message to your Chromecast speakers when someone is at the door.
> - Receive phone notification when someone arrives at the door. 
> - Continuous recording is useful when tracking suspicious neighborhood activity.

### Recommended Reading

- thewirecutter.com comparison


## Nest Hello
![](\assets\images\product-photo\nest-hello.png){:.image--lg.align-left}

**My personal experience with the Nest Hello camera is that it is reliable at sending timely notifications, but the monthly fee is required to get any real use out of it.** Monthly fees can add up quickly, though with Nest's new $5/month plan, I think it's worth paying for reliability. Wi-Fi cloud cameras have a lot of points of failure (poor Wi-Fi performance, slow upload speed, crap servers) but Nest gets most of it right. I recommend it for the continuous recording, timely alerts and a reliable mobile app. Alerts are sent to my phone within seconds, and recordings are available within a minute or two of the event. Viewing live footage takes only a few seconds too. Did I mention how quick it is to view an alert?

### The Problems

There is a Home/away Assist feature on the Nest app, but I found it doesn’t work reliably. There were a few times when I received an alert and opened the app to see my roommate watching TV in the living room. I’ve done my own testing of the feature (Home Assistant integration gives you access to this data) and found it can take hours for Nest to update to Home or Away status.

An option to store recorded videos locally will likely never come, as every company loves subscription revenue. Power-over-ethernet (PoE) is not an option either; it’s either wireless or nothing with the Nest doorbell.

<figure style="width: 100%;" >
 <img src="\assets\images\other\nest-doorbell.jpg" alt="" />
 <figcaption>
The hole is quite big and can’t be covered up by the camera alone. Nest doesn't provide a wall plate.
 </figcaption>
</figure>

One surprising omission with the Nest Hello package is the lack of a wall plate. Without it, the doorbell area is exposed and the doorbell install looks unprofessional. To deal with this issue, I used the Elago wall plate and can confirm it covers up the hole nicely.

### Installation and Smart Home Integration
The wiring is easy, though first follow the Nest compatibility checker to see if your house supports wired doorbells. The hardest part of the install is physically mounting the doorbell onto a hard surface. I had to use a hammer drill and a pair of earplugs to get the job done, though I definitely annoyed some neighbors in the process.

There isn’t any usable integration with Home Assistant and SmartThings, but I think it’s better to use the Nest app to watch videos.

<figure class="figure figure--25">
 <img src="/assets/images/integrations/nest-doorbell-ha.png" alt="Small picture of a kitten" />
 <figcaption>
 <b>Home Assistant: Great</b><br> It works, but impossible to see real-time footage. What is important is the ‘motion detected’ sensor.
 </figcaption>
</figure>

<figure class="figure figure--25">
 <img src="/assets/images/integrations/google-home.png" alt="Small picture of a kitten" style="width: 100%" />
 <figcaption>
 <b>Voice: Good</b><br>Can send broadcast messages when someone is at the door.
 </figcaption>
</figure>

<figure class="figure figure--25">
 <img src="/assets/images/integrations/na.png" alt="Small picture of a kitten" style="width: 100%; height: 100%" />
 <figcaption>
 <b>SmartThings: None</b><br> Integration does not exist.
 </figcaption>
</figure>

<figure class="figure figure--25">
 <img src="/assets/images/integrations/nest-doorbell-app.png" alt="Small picture of a kitten" style="width: 100%" />
 <figcaption>
 <b>Native App: Great</b><br>Simple, easy-to-use.
 </figcaption>
</figure>


# Outdoor Cameras

To be updated if I ever get an outdoor camera!