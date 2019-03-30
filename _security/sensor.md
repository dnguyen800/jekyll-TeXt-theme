---
layout: article
title: Sensors
short_title: Sensors
excerpt: I see dead people!!
category: [security, home automation]
permalink: /security/sensor
key: security-sensor
aside:
  toc: true
banner: assets/images/overlay/sensor.jpg
mode: immersive
header:
  theme: dark
article_header:
  type: overlay
  theme: dark
  background_color: '#203028'
  background_image:
    gradient: 'linear-gradient(135deg, rgba(34, 139, 87 , .4), rgba(139, 34, 139, .4))'
    src: /assets/images/overlay/sensor.jpg

---

<!--more-->

At a high level, sensors detect a change in the environment and report the details back to the home automation hub.  Whether it is a change in motion, water leak, voltage, someone’s presence, temperature, or an opening of a door—there likely exists a sensor for it. 

You will need door and motion sensors in your home so that the hub can detect activity and respond with an action, like turning on the lights. The sensors communicate using Zigbee or Z-Wave, which your SmartThings hub supports. I prefer to buy Z-Wave sensors as it is the newer technology, but I use a mix of Zigbee and Z-Wave, depending on pricing and quality.  You may have noticed that despite recommending a SmartThings hub, I do not use any SmartThings sensors. That is because nearly all SmartThings sensors have terrible ratings on Amazon! That is too bad—I would have given my money to one company if I could trust the quality of the product.

# Door (Contact) Sensors

**Published on: xx/xx/2019**

**Competitors in this space:** Dome, Monoprice, Visonic, SmartThings, Ecolink, Aeon Labs, and no-name brands.

I’ve personally tested the following:

|---
| ![](\assets\images\logo\dome.png){:.image--xl} |  ![](\assets\images\logo\monoprice.png){:.image--xl} | ![](\assets\images\logo\visonic.png){:.image--xl} | ![](\assets\images\logo\konnected.png){:.image--md} 
|:-:|:-:|:-:|:-:
|**Z-Wave Plus Door Sensors (DMWD1)** | **Z-Wave Plus Door and Window Sensor, No Logo** | **Door Sensor (MCT-340E)** | **Konnected Alarm Panel**

###  What you need to know

Contact sensors consists of two pieces: a magnet piece, and a piece that holds the wireless radio that communicates to the hub. Sensor are incredibly easy to install on doors and windows—just mount the pieces next to each other on a flat surface.  There is usually a gap between the door and door frame, but some sensors allow for a gap as large as one inch (check your product details). 

It seems like door sensors are the easiest to get right, as all of my sensors work as expected without any disconnect issues. Even the cheapest sensors work reliably. Still, I’ve noticed whenever SmartThings notifies me of opened doors, there may be a several minute delay. I don’t think it is a sensor issue, but an issue with Android’s battery saver function. 

Some sensors handle this better than others, but the sensitivity of door sensors is quite low—so the door can be slightly open, but the sensor reports it as closed. I tried using a sensor on a refrigerator door, but it failed to report the door as open when the door was open by as much as one fourth of an inch. Needless to say, the electricity bill did not go down that month.

I have my recommendation of contact sensors listed below, but there are plenty of sensors out there that work just fine and are probably cheaper. 

### Considerations before buying a door sensor

> - When installing the sensor, don’t place it on the door where the battery cover is blocked. 
> - Select a contact sensor that uses a battery type you commonly have. Monoprice uses AAA batteries, Dome is CR14250 (rare), and Visonic is CR2032.

### What you get with a door sensor

> - Know when people arrive or leave home. The lights can turn on right as you open the front door. 
> - Use sensors as a part of a DIY security system.

### Recommended Reading
> - Link?
> - SmartThings custom device handlers for [Dome](https://community.smartthings.com/t/release-dome-door-sensor-official/76321)


## Dome Z-Wave Plus Door Sensors (DMWD1) 
![Image: Dome](\assets\images\product-photo\dome-door-sensor.jpg){:.image--md.align-left}

I was able to snag the Dome Z-Wave Plus Door Sensors (DMWD1) during a sale from domeha.com and it was a good purchase at the time. **But no matter how good the Dome DMWD1 sensor is, the irregular battery size is a huge drawback as no one wants to buy a pair of batteries for one device.** Heck, it even uses a different battery size than the Dome motion sensor (CR123A)! I prefer a lower cost than a smaller sensor size, and I would have not purchased this if I had paid more attention to the battery size.

### The Problems

I’ll bring up the issue with the [odd battery size (CR14250)](https://www.amazon.com/s?k=CR14250&ref=nb_sb_noss_2) again, because in a market with reliable contact sensors, I can find a better sensor. I use these sensors on windows that are rarely opened, so changing batteries won’t be an issue until a year or two from now. 

### Installation and Smart Home Integration

I used these sensors with SmartThings and a [custom device handler by user @krlaframboise](https://community.smartthings.com/t/release-dome-door-sensor-official/76321) and haven’t run into any issues with pairing or general use. Detection happens nearly instantly, though not noticeably faster or slower than the other sensors I used. The sensors include double-sided tape to easily mount on the door.

<figure class="figure figure--25">
 <img src="/assets/images/integrations/dome-door-st.png" alt="Small picture of a kitten" style="width: 100%" />
 <figcaption>
 <b>SmartThings: Good</b><br>Using the free ST device handler adds more settings.
 </figcaption>
</figure>
<figure class="figure figure--25">
 <img src="/assets/images/integrations/dome-door-ha.png" alt="Small picture of a kitten" />
 <figcaption>
  <b>Home Assistant: Great</b><br>Creates one binary sensor entity in HA. 
 </figcaption>
</figure>
<figure class="figure figure--25">
 <img src="/assets/images/integrations/blank.png" alt="" style="width: 100%" />
 <figcaption>
 Testing to make sure formatting doesn't go out of whack.
 </figcaption>
</figure>
<figure class="figure figure--25">
 <img src="/assets/images/integrations/blank.png" alt="" style="width: 100%" />
 <figcaption>
 Testing to make sure formatting doesn't go out of whack.
 </figcaption>
</figure>



## Monoprice Z-Wave Plus Door Sensors (No Logo)
![ | *Monoprice*](\assets\images\product-photo\monoprice-door.jpg){:.image--md.align-left}

**The Monoprice Z-Wave Plus Door Sensors are a bit pricey, but they work as advertised and are a great way to use my spare AAA batteries.** The sensors won’t win any awards for design—these are the bulkiest door sensors I have and and can be an eyesore. If you’re looking for hidden sensors, then look into Monoprice’s recessed sensors. Make sure not to buy the **``Stitch version``** (Monoprice’s new line of WiFi-based smart devices) as they are not compatible with any of the home automation hubs.

For $20, I was expecting a low-profile sensor, but the sensors are reliable at least and that is most important aspect in a connected device.. 

### Installation and Smart Home Integration

The maximum gap between the sensor and magnet is 0.4”, which is slightly smaller than the other door sensors I tested. If you plan to use this sensor with the garage door, that is unlikely to go well without workarounds. 

Pairing the sensors is straightforward in SmartThings and Home Assistant, so I won’t go over it here. There is a tamper switch located on the back of the sensor, but is only usable with a [SmartThings device handler by user @rboy](https://community.smartthings.com/t/release-official-monoprice-z-wave-plus-sensor-door-window-mailbox-open-close-sensor-recessed-mounted-15268-15270-24259-with-external-trigger-option-and-tamper-device-handler/97273) that is locked behind a paywall. Device handlers are nice to have to access more details (like battery level), but not necessary.

<figure class="figure figure--50">
 <img src="/assets/images/integrations/monoprice-door-st.png" alt="Small picture of a kitten" style="width: 100%" />
 <figcaption>
 <b>SmartThings: Good</b><br> Works. More settings in a paid device handler.
 </figcaption>
</figure>
<figure class="figure figure--50">
 <img src="/assets/images/integrations/monoprice-door-ha.png" alt="Small picture of a kitten" />
 <figcaption>
  <b>Home Assistant: Good</b><br> This is how a door sensor looks like in HA
 </figcaption>
</figure>


## Visonic Door Sensor (MCT-340E) 

![](\assets\images\product-photo\visonic-sensor.jpg){:.image--md.align-left}

**I bought the Visonic Door Sensor (MCT-340E) on a whim because they were so cheap ($10), but the small profile, battery size (CR2032), and reliability convinced me that this would make a solid budget recommendation.** The sensor also monitors temperature, though I have never received an accurate reading. If you don’t have any issues with your Zigbee network, then I would recommend giving these sensors a try.

I have a Wi-Fi mesh network and a small Zigbee network of smart bulbs—both operating on the 2.4ghz frequency—but haven’t run into any connection issues. I would worry about connectivity in a much larger home, but for medium-sized homes and condos, range is not going to be a concern.

{:.info}
*The sensor is $5 cheaper at mydigitaldiscount.com, where I originally bought it for $10.*


### Installation and Smart Home Integration

Pairing these sensors with Home Assistant can get a little messy as it creates multiple entities for contact and temperature sensor, but pairing with SmartThings is easy. It is one reason I still recommend SmartThings over Home Assistant, where pairing devices is much more straightforward. 

## Konnected

![Konnected](\assets\images\product-photo\konnected.jpg){:.image--xl.align-left}

If you already have wired sensors installed from a security system in your home, you should check out the Konnected board, which can reuse those sensors with home automation hubs like SmartThings, Home Assistant and Hubitat. I installed one at a friend’s house and was able to connect four door sensors, a siren, a piezo buzzer, and used the 12V port to power a wall-mounted tablet. Be warned that it is a product with bugs—I spent two days trying to figure out an issue that was eventually resolved with a firmware update.

The cost of a Konnected module ($89) is high, but when you factor in the cost of purchasing wireless sensors at $20-30 each, then the module pays for itself with five wired sensors. I also like the fact that I can use a Honeywell wired siren with Konnected because it’s much louder and effective at scaring off intruders than any wireless siren I’ve tried.

<figure style="width: 30%;" >
 <img src="/assets/images/integrations/konnected-st.png" alt="" />
 <figcaption>
  I frequent the Konnected status page for troubleshooting issues.
 </figcaption>
</figure>
<figure style="width: 30%;" >
 <img src="/assets/images/integrations/konnected-st-02.png" alt="" />
 <figcaption>
 SmartThings Four Konnected sensors and a siren connected in ST.
 </figcaption>
</figure>
<figure style="width: 30%;" >
 <img src="/assets/images/integrations/konnected-st.png" alt="" />
 <figcaption>
 What a Konnected sensor looks like in SmartThings.
 </figcaption>
</figure>


### Installation and Smart Home Integration

This is an advanced DIY installation and requires some study of your previous alarm system. Not every system is compatible, so it’s important to read through the Konnected Support section before purchasing. The Konnected Facebook group is also a friendly group to ask questions—I received responses within an hour of asking, though none of the advice solved my issue. Experience with electrical wiring, voltage, and a lot of patience is needed.


# Motion Sensors

Overlay

Kind of like a camera (but less creepy)

**Published on: xx/xx/2019**

**Competitors in this space:** Dome, Zooz, Monoprice, SmartThings, Ecolink, GE, Fibaro, Besense, Aeon Labs

*I’ve personally tested the following:*

|---
| ![](\assets\images\logo\dome.png){:.image--xl} |  ![](\assets\images\logo\zooz.png){:.image--xl} | ![](\assets\images\logo\ge.png){:.image--sm} | ![](\assets\images\logo\ecobee.png){:.image--xl} 
|:-:|:-:|:-:|:-:
|**Z-Wave Plus Motion Sensor (DMMS1)** | **Z-Wave Plus Motion Sensor (ZSE18)** | **GE Z-Wave Plus Smart Motion Sensor (34193)** | **Room Sensors**


### What you need to know

I’m very surprised at the lack of quality motion sensors on the market today. A quick glance through [Amazon](https://www.amazon.com/s?k=z-wave+motion+sensor&ref=nb_sb_noss_2) shows only three motion sensors with 4-star ratings—the rest don’t make the cut. It seems hard to make a reliable sensor with good battery life and USB charging capability. It’s not cheap either—having to pay $35-40 adds up quickly for a basic but necessary sensor in your smart home.

With these high prices, I always remind people to think of alternatives, like installing simple motion-sensing light switches where possible. Not only are they significantly cheaper, but they double as a light switch and motion sensor. Guest bathrooms, closets, garage, and pantry areas make the most sense for these switches. ~ See section: <??~Light switches??>

I’ve tested a few motion sensors and I found a few that I like. All of them happen to be **``Z-Wave Plus sensors``**, which is also my recommended wireless standard. I can’t promise you that the ones listed are the best sensors out there, but I can promise they are good for specific scenarios.

### Considerations before buying a motion sensor

> - Read reviews before buying. Common issues with pairing and disconnecting from the hub.
> - Motion sensor response is not instant—it takes about two seconds for the light to turn on from a detection.
> - Thoroughly test sensors and isolate failures in your automations. It’s possible to receive defective sensors.
> - Check that the battery type is common. My sensors all use CR123 batteries, though yours may be different.

### What you get with a motion sensor

> - Lighting that turns on as you walk around the house.
> - Lights remain on as long as a room is occupied.

### Recommended Reading
> - Amazon searches for [Z-Wave motion sensors](https://www.amazon.com/s?k=z-wave+motion+sensor&ref=nb_sb_noss_2)


## Dome Home Automation Z-Wave Plus (DMMS1) sensor

![](\assets\images\product-photo\dome-motion-sensor.jpg){:.image--md.align-left}

My first motion sensor was the Dome Home Automation Z-Wave Plus **``(DMMS1)``** sensor, and I can say it is the most reliable motion sensor I used and repurchased over the years. I use them in stairways, hallways, entrances—mainly low to medium traffic areas where I absolutely need the light to turn on. Walking down the stairs in the dark shouldn’t happen in a smart home and Dome motion sensors haven’t failed me in this regard.

The detection range is better than most sensors, with objects reliably detected at 30 feet, and even further using higher sensitivities (and likely more false positives). In the living room, I use one sensor to detect someone entering from the opposite end of the room—about 30 feet. 

The sensors can’t be powered by micro-USB, so I don’t use them in high-traffic areas that will drain batteries quickly. I don’t have battery life benchmarks, but in real use, I change batteries every 3 to 6 months in medium traffic areas. 

### The Problems

The design of the base makes it impossible to mount on wall corners, so I place them right above the door or on a bookshelf for similar coverage. 

### Installation and Smart Home Integration

Right out of the box, Dome sensors can be paired with SmartThings and Home Assistant, but sensitivity settings cannot be adjusted without installing the SmartThings custom device handler created by @krlaframboise. 

Pairing in Home Assistant is messy, as the sensor adds motion and ambient light entities, and some other values I’m not sure what to do with, like ``**Burglar**``, ``**Alarm Level**``, and so on. Motion detected is represented as a number value, rather than a binary value, so you would need to create a template sensor to simplify things.

## Zooz Z-Wave Plus Motion Sensor (ZSE18)

![](\assets\images\product-photo\zooz.png){:.image--xl.align-left}

If a sensor only works 90% of the time, is it worth buying? The Zooz Z-Wave Plus Motion Sensor (ZSE18) is one of the cheapest motion sensors on the market ($20-23) but after testing for months and running into several issues, I can’t recommend these for any use.  With a reduced range (around 15-20ft) and less than 100% reliability, I can’t use the sensor in areas where I absolutely need the light to turn on, so I relegated it to less critical areas like the bedroom or office. If I could return them, I would and purchase some reliable sensors instead.

The sensor’s design is my favorite out of all that I’ve tested. It uses a magnetic base like the Dome sensors, but has the micro-USB port accessible from the outside of the case. This lets me position the sensor in a way that doesn’t create tension on the cable and keep the sensor steady. 

### The Problems

My first batch of sensors turned out to be faulty—the default sensitivity settings were way too low to be useful in any scenario. Luckily, I received a replacement but the sensors continue to exhibit different issues. 10% of the time, the motion sensor reports active motion but remains as active indefinitely, which breaks my lighting automations and keeps the lights on. Once I walk by the sensor, it reports active motion again, though it has already been reporting active for several hours! The same issue happens with reporting inactive motion, though the issue is fixed by walking near the sensor and waking it up. My theory is that the sensor goes into sleep mode, but forgets to update status before doing so. It’s a frustrating hardware flaw that is unlikely to be fixed.

### Installation and Smart Home Integration

Connecting to SmartThings is hit-or-miss for me. I’m never able to pair the sensor on the first try. I have also had to reconnect the sensor to SmartThings once a month, on average.

## GE Z-Wave Plus Motion Sensors

![](\assets\images\product-photo\ge-motion-sensor.jpg){:.image--md.align-left}

I continue to buy GE Z-Wave Plus Motion Sensors for its excellent range and USB power, but since it’s no longer being sold at retailers, I can’t recommend it. I sometimes find deals on eBay for under $30, which is a fair price as the sensor isn’t perfect (poor battery life and limited mounting options come to mind). These sensors are great in high traffic and large areas, but only if you can power the sensors with a USB cable.

<figure style="width: 50%;" >
 <img src="\assets\images\other\motion-sensor-range.jpg" alt="" />
 <figcaption>

 </figcaption>
</figure>

I can vouch that the range is really good, around 35 to 40 feet. I use these sensors in the living room and dining room and it always detect motion as expected, whether in light or darkness. Response is not instant—I experience about a 1-2 second lag from detecting motion to turning on the light. If you’re running around the house in the dark, you will definitely beat the lights. 

### Installation and Smart Home Integration

Pairing in SmartThings is easy, but Home Assistant is a little more difficult as it creates five entities (though only one is useful), and spits out number values instead of an on/off value. I ended up creating a template sensor to simplify automations.

## BeSense Ceiling Motion Sensor

![](\assets\images\product-photo\besense.jpg){:.image--md.align-left}

The BeSense ceiling motion sensor is a new sensor on the market that caught my eye on Amazon. I haven’t tested it, but the good reviews, use of AA batteries and affordable price made me curious. It is a ceiling sensor so it is best used in small rooms, hallways and condos where the ceiling isn’t so high. If I ever buy it, I’ll report my findings here.






## Ecobee Sensors

![](\assets\images\product-photo\ecobee-sensor.png){:.image--md.align-left}

Ecobee thermostats come with room sensors that monitor temperature, but did you know that it can also be used as a motion sensor? I would never buy purchase Ecobee sensors as dedicated motion sensors, but they are nice to have as secondary sensors to confirm if a room is truly empty.

Some important info about the sensors: they can be used only if you have an Ecobee thermostat installed as it uses an proprietary method to communicate. The sensor’s battery can last for over a year using a single CR2032 battery—the same ones used in most car key fobs. 

### The Problems

Motion detection is not timely, at all. It takes more than several minutes to report occupancy, andan empty room. I couldn’t think of many useful automations using this as a motion sensor, except as additional confirmation that no one is present in a room. 

### Installation and Smart Home Integration

If you integrate the Ecobee thermostat with Smartthings or Home Assistant, then these sensors are automatically added to your setup. 


# Tilt Sensors (for garage doors)

**Published on: xx/xx/2019**

**Competitors in this space:** Monoprice. Not much else.

*I’ve personally tested the following:*

|---
| ![](\assets\images\logo\monoprice.png){:.image--xl} 
|:-:
|** Z-Wave Plus Acceleration Sensor**


### What you need to know

Tilt sensors operate differently than door/contact sensors in that it is made of a single piece (versus two pieces for door sensors) and detects movement through gravity and acceleration. It’s easier to understand with the picture below.

<figure style="width: 50%;" >
 <img src="\assets\images\other\tilt-sensor.png" alt="" />
 <figcaption>
| randomnerdtutorials.com
 </figcaption>
</figure>

It is basically a small ball in a tube that completes the flow! The most obvious movement it can detect is when a garage door moves from a vertical position **``(closed)``** to a horizontal position **``(open)``**. A typical door sensor is difficult to use with garage doors due to the gap between the door and wall being too wide—this is where a tilt sensor becomes useful. I previously used a tilt sensor with the **``Chamberlain MyQ garage door opener``** to get an “accurate” reporting of garage door status, though I stopped using it due to unreliable status reporting. It seems that this is a common theme with tilt sensors like the Ecolink sensor, but there are workarounds mentioned in [Amazon reviews.](https://www.amazon.com/Z-Wave-Plated-Reliability-Garage-TILT-ZWAVE2-5-ECO/dp/B01MRZB0NT/ref=sr_1_1?keywords=ecolink+tilt&qid=1553801492&s=gateway&sr=8-1#customerReviews)

A tilt sensor for the garage door wouldn’t be necessary if Chamberlain allowed users access to the MyQ data outside of the app. A tilt sensor is meant to be an extra verification that the door is in fact, closed. With the poor reliability of the tilt sensor I used, I would rather rely on a camera to confirm the door is closed.

### Considerations before buying a tilt sensor

> - **RF signals may be absorbed by a metal garage door.** Try to place a portion of the sensor away from the door, like what this Amazon reviewer did. 
> - **Consider the position of the sensor on the garage door—and don’t place it at the bottom of the door.** When the door opens, the sensor should begin rotating immediately with the door.
> - **Random, false positives from the sensor are possible**, so I don’t recommend setting up alarm automations until thoroughly tested.
> - **Some remote garage openers include a tilt sensor,** like the Linear GoControl Z-Wave Garage Door Opener, so you don’t need to buy a separate sensor.

### What you get with a tilt sensor

> - Additional confirmation that the garage door is closed, though it’s not 100% accurate without workarounds.

### Recommended Reading

> - [Installation tips](https://www.amazon.com/Z-Wave-Plated-Reliability-Garage-TILT-ZWAVE2-5-ECO/dp/B01MRZB0NT/ref=sr_1_1?keywords=ecolink+tilt&qid=1553801492&s=gateway&sr=8-1#customerReviews) from Amazon.com reviews

## Monoprice Z-Wave Plus Acceleration Sensor

![](\assets\images\product-photo\monoprice-tilt.jpg){:.image--md.align-left}

**The Monoprice Z-Wave Plus Acceleration Sensor sucks, period. Don't buy it.** If a sensor is accurate only 80% of the time, then it's north worth it. I was getting the worst kind of false positives where the garage door is physically closed, but the sensor reported it as open. That is unacceptable when I’m away from home for days at a time and can’t confirm the door is closed, which is the sole purpose of a tilt sensor. The placement of the sensor on the garage door only needs to report status in two positions: horizontal or vertical. I don’t know how the sensor can report those states incorrectly so often, but it does. 

There are potential workarounds mentioned on Amazon reviews of the Ecolink tilt sensor, but I already stopped using the sensor by that point. My sensor was placed on the top panel of the garage door, but still had problems detecting vertical and horizontal position. I gave up on the sensor and installed a camera to check the garage door if needed. I haven’t had to use it as MyQ has been reporting status correctly without the sensor.


# Presence Sensor/Device Tracker

**Published on: xx/xx/2019**

**Competitors in this space:**
Hardware: SmartThings, iBeacons, Bluetooth LE devices
Software: SmartThings, Life360, Tile, iCloud, nmap, so many more.

I’ve personally tested the following:

|---
| ![](\assets\images\logo\smartthings.png){:.image--xl} |  ![](\assets\images\logo\monoprice.png){:.image--xl} | ![](\assets\images\logo\visonic.png){:.image--xl} | ![](\assets\images\logo\konnected.png){:.image--md} 
|:-:|:-:|:-:|:-:
|**Z-Wave Plus Door Sensors (DMWD1)** | **Z-Wave Plus Door and Window Sensor, No Logo** | **Door Sensor (MCT-340E)** | **Konnected Alarm Panel**

- SmartThings app
- Life360 app
- Tile app
- iCloud
- nmap

### What you need to know

Presence detection is the ability to detect whether someone approaches or leaves a specified area, like home, at work, or school. Detection can be simple (home/away) or complex (exact GPS coordinates) and relies on a mobile app or physical device—like a Tile tracker—to determine your location. I mainly use device trackers as another data point to enhance automations (e.g. if I arrive at home and open the door, then turn on the lights), and in a few scenarios, to unlock and lock doors. To me, a reliable device tracker is one that can detect I’m home right before I reach the door.

It took some time to find a capable presence sensor that was timely enough to update (within a minute’s notice), but it exists!

### Things to consider before adding a device tracker

> - When designing automations, make sure to test, test, and test. There are odd issues where for one millisecond, the sensor mistakenly reports you are home and opens the garage to intruders.
> - Make sure you have consent before installing a GPS tracking app like Tile or Life360.

### What you get with a presence detection sensor

> - Design automations using geofencing like announcements (Dan is arriving home).
> - Tell the difference between someone arriving at home and opening the door, versus opening the door. 

### Recommended Reading
> - ?

## Nmap

![](\assets\images\logo\nmap.jpg){:.image--md.align-left}

Nmap is a network scanning tool that has many uses, though at a basic level it scans the network for connected devices. In Home Assistant, we repurpose the Nmap component as a device tracker: it scans the network for my phone and updates device status to ‘home’ if online, and ‘away’ if offline. **I like Nmap as it is a simple, non-intrusive service that doesn’t require installing an app, and doesn’t track location any further than the house.** That makes it easy to convince my roommates to use it as they don’t have to do anything on their phones, other than take their phones when they leave the house.

I have one goal with these device trackers, which is to update location status before I reach the door. This lets me unlock the door or open the garage door right as I arrive. In my testing, results have been very positive. Status changes happen in less than a minute. Nmap is fast enough to detect when I’m in the garage, and ~ an automation unlocks the door in time.

### The Problems

There’s a few things you should know before using nmap. Tracking from away to home is deadly fast, but leaving home takes a few minutes to update status. This is a design choice that is reversible in settings in order to save battery life on the device.  Nmap is limited to tracking on the home Wi-Fi network, so you can’t track whether someone is at work or school.

Nmap’s accuracy is dependent on the signal strength of your network being able to reach just outside your garage or front door. Using a Wi-Fi mesh system or a powerful network router will make this a non-issue. 

### Installation and Smart Home Integration

The **``Nmap``** component is available on Home Assistant only, but the configuration is incredibly easy to fill out. Once a configuration is added, a Home Assistant sensor will appear:

![Home Assistant:](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1550356635252_device_tracker-nmap-ha.png)



## The Competition

In my process of finding the right device tracker, I’ve tested a few other platforms and shared my thoughts. At least you will know which ones to skip.

|             | Works in SmartThings | in Home Assistant | Time Accuracy      |                                                              |
| ----------- | -------------------- | ----------------- | ------------------ | ------------------------------------------------------------ |
| nmap        |                      | X                 | Less than a minute | Good: Fast status update, no interaction with household members needed. No additional app needed.<br>Bad: Only useful for detecting home/away status. Requires decent Wifi router |
| iCloud      |                      | X                 |                    | Good:<br>Bad: Current Home Assistant implementation requires re-authentication every two months if using two-factor auth. Requires saving iCloud password in text file. |
| iBeacons    |                      | X                 |                    |                                                              |
| Life360     | X                    | X                 | 1 to 2 minutes     | Good: Life360 In Home Assistant, there is only one-minute delay. Can set multiple geofences for home, work, school.<br>Bad: Life360 in SmartThings, I’ve experience a one-hour delay. Provides too much location details. |
| Tile        |                      | X                 | Terrible           | Good: None.<br>Bad: Completely inaccurate. Location update can take hours to days. Provides too much location details. |
| Nest        |                      | X                 | Bad                | Good: None<br>Bad: Requires installation of Nest app and enable ‘Home/Away Assist’ feature to work. Status update ranges from minutes to several hours delay. |
| SmartThings | X                    | X                 | Terrible           | Good: None.<br>Bad: It never detected when I was away. Location does not update AT ALL unless SmartThings app is opened on user’s phone, which is unlikely. |

