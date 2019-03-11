---
layout: article
title: Smart Home Wireless Standard
category: Infrastructure

---

## Smart Home Wireless Standard
Published xx/xx/2019

**Competitors in this space:** Z-Wave Plus, Zigbee, Wi-Fi, Bluetooth LE, Homekit, Thread

I’ve personally tested the following:

- Z-Wave Plus (sensors from Zooz, Dome, Monoprice, Leviton)
- Zigbee (smart bulbs from Sengled, Sylvania, Philips Hue)
- Wi-Fi (TP-Link Kasa and D-Link devices)
- Homekit (using iPhone SE, iPad 6th Generation)

### Overview
There’s another set of wireless standards in the smart home space that you need to know about. Familiar standards like Wi-Fi, bluetooth, RF, infrared, didn’t quite cut it for smart home use, so we’re left with two new standards: Zigbee and Z-Wave. Each have their set of advantages and disadvantages with no clear winner.

Your hub supports most of the wireless standards (Zigbee, Z-Wave, Wi-Fi), but smart devices usually support only one standard—either Zigbee, Wi-Fi or Z-Wave. Adding to the confusion are companies like Philips, Ikea, Sengled and Xiaomi selling their own Zigbee hubs that are compatible with their respective bulbs only. Great job segmenting the market there, people.

Innovelli and Tom’s Guide offers a great primer on the different wireless technologies, though I have some straightforward advice for the consumer: don’t worry about using more than one wireless standard in your home. I think it’s inevitable to use more than one standard as to avoid limiting your options.

In the three-story home I set up, I use Zigbee light bulbs and door sensors, Z-Wave Plus motion sensors and outlets, and Lutron Caseta light switches. It was a matter of convenience, cost, and availability that I ended up using three standards, but surprisingly I have no issues with range or connectivity.  If wireless range was a concern, I could install range extenders such as smart bulbs, outlets, light switches, or USB-powered sensors. 

In my search for deals on smart devices, I’ve noticed the following trends:

- The most reliable motion sensors readily available are usually Z-Wave. 
- The cheapest contact sensors are Zigbee, but new sensors are hard to find. Z-Wave sensors tend to be 1.5 to 2x higher in price, but the difference is negligible—about $5-10 more per device.
- The cheapest and most readily available smart bulbs are Zigbee bulbs. Colored bulbs are expensive, no matter what standard it is.
- Zigbee and Z-Wave Plus power outlets are around the same price, though Zigbee availability is low.
- Light switches usually use Z-Wave, but I strongly urge you to consider Lutron Caseta switches.

#### Considerations before choosing a wireless standard

- The total number of connected devices. Z-Wave device limit is 255. Zigbee is much higher at 65,355. Most homes will likely never hit Zigbee limits.
- Placement of the hub, and powered repeaters. Will you have enough repeaters to reach the furthest device? Z-Wave can hop at most 4 always-powered devices.
- Philips Hue and its incompatible Zigbee standard. Philips Hue is Zigbee, but uses a different profile called ZLL.  Hue bulbs act as repeaters for Hue bridge only.
- The wireless communications can be slow. There is a noticeable delay between the sensor registering a change, sending data to hub, running automation, turning on a light. I’ve noticed a 1-2 second delay.

#### What you get with a smart home wireless standard

- A dedicated wireless network for your smart devices that hopefully doesn’t interfere with existing wireless tech like Wi-Fi.


### Z-Wave Plus
![](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1551244282226_whitespace.png)
![Image: Amazon](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1551244082211_zwave_plus-logo.jpg)
![](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1551244269701_whitespace.png)


If I had to choose one standard, I would hesitantly recommend Z-Wave Plus because new Z-Wave products are being released and readily available on the market. I hesitate because reliable Z-Wave devices are hard to find—just look at 3-star Amazon reviews when you search for “Z-Wave.” The same can be said for Zigbee devices, depending on the category.

Theoretically, Z-Wave is better than Zigbee in most cases because it operates on a different, less congested wireless frequency. This reduces the chance of interference caused by other devices sharing the same frequency—a problem that Zigbee devices face with Wi-Fi devices using the same 2.4ghz frequency. Z-Wave’s hop and device limit looks bad compared to Zigbee, though I bet most homes will never hit this limit. 

#### The Problems
Z-Wave Plus should be winning the wireless smart home standard, but it’s not. Z-Wave devices are more expensive than Zigbee counterparts, likely due to licensing and certification costs. Certification doesn’t necessarily guarantee quality, and the number of issues reported on Z-Wave devices are just too high for me to consider it a reliable standard. Here’s hoping that its successor, Z-Wave Plus, doesn’t repeat the same mistakes.


#### The Competition

There are new standards like Homekit, Thread, or WiFi-based ones like Wemo, but adoption rates remain low and I have concerns about the longevity of these standards. Homekit is slowly growing its footprint, but it is not usable outside Apple devices, or even the iOS ecosystem. Be especially wary of any Wi-Fi labeled products from D-Link, TP-Link Kasa or Belkin Wemo as those are not open standards and may not be supported if the company shuts down. 

#### Recommended Reading
- Tom’s Guide to Wireless Home Standards
- A good Z-Wave/Zigbee/Bluetooth/Wifi Comparison Article by Innovelli
- “What is Z-Wave Plus?” Article by Innovelli
- Wirecutter - Building a Home with Homekit