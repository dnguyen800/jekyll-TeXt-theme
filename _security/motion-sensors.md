---
layout: article
title: Motion Sensors
category: home security

---
## Motion Sensors
#### Kind of like a camera (but less creepy)
**Published on: xx/xx/2019**

![](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1550450592892_motion_sensor-front_page.png)


**Competitors in this space:** Dome, Zooz, Monoprice, SmartThings, Ecolink, GE, Fibaro, Besense, Aeon Labs

I’ve personally tested the following:

- Dome Z-Wave Plus Motion Sensor (DMMS1)
- Zooz Z-Wave Plus Motion Sensor (ZSE18)
- General Electric Z-Wave Plus Smart Motion Sensor (34193)
- Ecobee Room Sensors

### Overview
I’m very surprised at the lack of quality motion sensors on the market today. A quick glance through Amazon shows only three motion sensors with 4-star ratings—the rest don’t make the cut. It seems hard to make a reliable sensor with good battery life and USB charging capability. It’s not cheap either—having to pay $35-40 adds up quickly for a basic but necessary sensor in your smart home.

With these high prices, I always remind people to think of alternatives, like installing simple motion-sensing light switches where possible. Not only are they significantly cheaper, but they double as a light switch and motion sensor. Guest bathrooms, closets, garage, and pantry areas make the most sense for these switches. ~ See section: <??~Light switches??>

I’ve tested a few motion sensors and I found a few that I like. All of them happen to be Z-Wave Plus sensors, which is also my recommended wireless standard. I can’t promise you that the ones listed are the best sensors out there, but I can promise they are good for specific scenarios.

#### Things to consider before buying a motion sensor

- Read reviews before buying. Common issues with pairing and disconnecting from the hub.
- Motion sensor response is not instant—it takes about two seconds for the light to turn on from a detection.
- Thoroughly test sensors and isolate failures in your automations. It’s possible to receive defective sensors.
- Check that the battery type is common. My sensors all use CR123 batteries, though yours may be different.

#### What you get with a motion sensor

- Lighting that turns on as you walk around the house.
- Lights remain on as long as a room is occupied.


### Dome Home Automation Z-Wave Plus (DMMS1) sensor
![Source: domeha.com](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1550446314845_motion_sensor-dome-photo01.jpg)
![](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1550446234465_dome-logo.png)
![](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1550448947395_motion_sensor-dome-photo02.jpg)


My first motion sensor was the Dome Home Automation Z-Wave Plus (DMMS1) sensor, and I can say it is the most reliable motion sensor I used and repurchased over the years. I use them in stairways, hallways, entrances—mainly low to medium traffic areas where I absolutely need the light to turn on. Walking down the stairs in the dark shouldn’t happen in a smart home and Dome motion sensors haven’t failed me in this regard.

The detection range is better than most sensors, with objects reliably detected at 30 feet, and even further using higher sensitivities (and likely more false positives). In the living room, I use one sensor to detect someone entering from the opposite end of the room—about 30 feet. 

The sensors can’t be powered by micro-USB, so I don’t use them in high-traffic areas that will drain batteries quickly. I don’t have battery life benchmarks, but in real use, I change batteries every 3 to 6 months in medium traffic areas. 

#### The Problems
The design of the base makes it impossible to mount on wall corners, so I place them right above the door or on a bookshelf for similar coverage. 

#### Installation and Smart Home Integration
Right out of the box, Dome sensors can be paired with SmartThings and Home Assistant, but sensitivity settings cannot be adjusted without installing the SmartThings custom device handler created by @krlaframboise. 

Pairing in Home Assistant is messy, as the sensor adds motion and ambient light entities, and some other values I’m not sure what to do with, like “burglar.” Motion detected is represented as a number value, not as a true/false value, so you would need to create a template sensor to simplify things.

### Zooz Z-Wave Plus Motion Sensor (ZSE18)

![](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1550450769579_motion_sensor-zooz-logo.png)
![](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1550450918076_motion_sensor-zooz-photo.png)


If a sensor only works 90% of the time, is it worth buying? The Zooz Z-Wave Plus Motion Sensor (ZSE18) is one of the cheapest motion sensors on the market ($20-23) but after testing for months and running into several issues, I can’t recommend these for any use.  With a reduced range (around 15-20ft) and less than 100% reliability, I can’t use the sensor in areas where I absolutely need the light to turn on, so I relegated it to less critical areas like the bedroom or office. If I could return them, I would and purchase some reliable sensors instead.

The sensor’s design is my favorite out of all that I’ve tested. It uses a magnetic base like the Dome sensors, but has the micro-USB port accessible from the outside of the case. This lets me position the sensor in a way that doesn’t create tension on the cable and keep the sensor steady. 

#### The Problems
My first batch of sensors turned out to be faulty—the default sensitivity settings were way too low to be useful in any scenario. Luckily, I received a replacement but the sensors continue to exhibit different issues. 10% of the time, the motion sensor reports active motion but remains as active indefinitely, which breaks my lighting automations and keeps the lights on. Once I walk by the sensor, it reports active motion again, though it has already been reporting active for several hours! The same issue happens with reporting inactive motion, though the issue is fixed by walking near the sensor and waking it up. My theory is that the sensor goes into sleep mode, but forgets to update status before doing so. It’s a frustrating hardware flaw that is unlikely to be fixed.

#### Installation and Smart Home Integration
Connecting to SmartThings is hit-or-miss for me. I’m never able to pair the sensor on the first try. I have also had to reconnect the sensor to SmartThings once a month, on average.

### GE Z-Wave Plus Motion Sensors

![](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1550451996449_ge-logo.png)
![](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1550521236419_motion_sensor-ge-photo03.jpg)
![](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1550525001559_whitespace.png)


I continue to buy GE Z-Wave Plus Motion Sensors for its excellent range and USB power, but since it’s no longer being sold at retailers, I can’t recommend it. I sometimes find deals on eBay for under $30, which is a fair price as the sensor isn’t perfect (poor battery life and limited mounting options come to mind). These sensors are great in high traffic and large areas, but only if you can power the sensors with a USB cable.


![](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1550521146746_whitespace.png)
![](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1550521069640_motion_sensor-ge-range.jpg)
![](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1550521136426_whitespace.png)


I can vouch that the range is really good, around 35 to 40 feet. I use these sensors in the living room and dining room and it always detect motion as expected, whether in light or darkness. Response is not instant—I experience about a 1-2 second lag from detecting motion to turning on the light. If you’re running around the house in the dark, you will definitely beat the lights. 

#### Installation and Smart Home Integration
Pairing in SmartThings is easy, but Home Assistant is a little more difficult as it creates five entities (though only one is useful), and spits out number values instead of an on/off value. I ended up creating a template sensor to simplify automations.


### BeSense Ceiling Motion Sensor
![](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1550524946863_besense-logo.png)
![](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1550524957449_motion_sensor-besense-photo01.jpg)


The BeSense ceiling motion sensor is a new sensor on the market that caught my eye on Amazon. I haven’t tested it, but the good reviews, use of AA batteries and affordable price made me curious. It is a ceiling sensor so it is best used in small rooms, hallways and condos where the ceiling isn’t so high. If I ever buy it, I’ll report my findings here.


### Ecobee Sensors
![](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1550522096256_ecobee-logo.png)
![](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1550522236114_motion_sensor-ecobee-photo01.jpg)


Ecobee thermostats come with room sensors that monitor temperature, but did you know that it can also be used as a motion sensor? I would never buy purchase Ecobee sensors as dedicated motion sensors, but they are nice to have as secondary sensors to confirm if a room is truly empty.

Some important info about the sensors: they can be used only if you have an Ecobee thermostat installed as it uses an proprietary method to communicate. The sensor’s battery can last for over a year using a single CR2032 battery—the same ones used in most car key fobs. 

#### The Problems
Motion detection is not timely, at all. It takes more than several minutes to report occupancy, andan empty room. I couldn’t think of many useful automations using this as a motion sensor, except as additional confirmation that no one is present in a room. 

#### Installation and Smart Home Integration
If you integrate the Ecobee thermostat with Smartthings or Home Assistant, then these sensors are automatically added to your setup. 