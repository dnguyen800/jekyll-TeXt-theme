---
layout: article
title: Door Sensors
category: home security

---

## Door (Contact) Sensors
**Published on: xx/xx/2019**
![](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1550726877810_door_sensor-front_page.png)


**Competitors in this space:** Dome, Monoprice, Visonic, SmartThings, Ecolink, Aeon Labs, and no-name brands.

I’ve personally tested the following:

- Dome Z-Wave Plus Door Sensors (DMWD1)
- Monoprice Z-Wave Plus Door and Window Sensor, No Logo
- Visonic Door Sensor (MCT-340E)
- Konnected Alarm Panel

### Overview
Contact sensors consists of two pieces: a magnet piece, and a piece that holds the wireless radio that communicates to the hub. Sensor are incredibly easy to install on doors and windows—just mount the pieces next to each other on a flat surface.  There is usually a gap between the door and door frame, but some sensors allow for a gap as large as one inch (check your product details). 

It seems like door sensors are the easiest to get right, as all of my sensors work as expected without any disconnect issues. Even the cheapest sensors work reliably. Still, I’ve noticed whenever SmartThings notifies me of opened doors, there may be a several minute delay. I don’t think it is a sensor issue, but an issue with Android’s battery saver function. 

Some sensors handle this better than others, but the sensitivity of door sensors is quite low—so the door can be slightly open, but the sensor reports it as closed. I tried using a sensor on a refrigerator door, but it failed to report the door as open when the door was open by as much as one fourth of an inch. Needless to say, the electricity bill did not go down that month.

I have my recommendation of contact sensors listed below, but there are plenty of sensors out there that work just fine and are probably cheaper. 

#### Things to consider before buying a door sensor

- When installing the sensor, don’t place it on the door where the battery cover is blocked. 
- Select a contact sensor that uses a battery type you commonly have. Monoprice uses AAA batteries, Dome is CR14250 (rare), and Visonic is CR2032.

#### What you get with a door sensor

- Know when people arrive or leave home. The lights can turn on right as you open the front door. 
- Use sensors as a part of a DIY security system.


### Dome Z-Wave Plus Door Sensors (DMWD1) 
![](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1550608575800_dome-logo.png)
![](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1550608739204_door_sensor-dome-photo01.jpg)

I was able to snag the Dome Z-Wave Plus Door Sensors (DMWD1) during a sale from domeha.com and it was a good purchase at the time. But no matter how good the Dome DMWD1 sensor is, the irregular battery size is a huge drawback as no one wants to buy a pair of batteries for one device. Heck, it even uses a different battery size than the Dome motion sensor (CR123A)! I prefer a lower cost than a smaller sensor size, and I would have not purchased this if I had paid more attention to the battery size.

I used these sensors with SmartThings and a custom device handler by @krlaframboise and haven’t run into any issues with pairing or general use. Detection happens nearly instantly, though not noticeably faster or slower than the other sensors I used. The sensors include double-sided tape to easily mount on the door.


![Home Assistant This is what any contact sensor looks like in HA.](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1550681880637_door_sensor-monoprice-app.png)
![SmartThings App](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1550625246873_door_sensor-dome-app.png)
![](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1550625260999_whitespace.png)

#### The Problems
I’ll bring up the issue with the odd battery size (CR14250) again, because in a market with reliable contact sensors, I can find a better sensor. I use these sensors on windows that are rarely opened, so changing batteries won’t be an issue until a year or two from now. 

### Monoprice Z-Wave Plus Door Sensors (No Logo)

![](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1550608566931_monoprice-logo.PNG)
![](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1550608615357_door_sensor-monoprice-photo01.jpg)


The Monoprice Z-Wave Plus Door Sensors are a bit pricey, but they work as advertised and are a great way to use my spare AAA batteries. The sensors won’t win any awards for design—these are the bulkiest door sensors I have and and can be an eyesore. If you’re looking for hidden sensors, then look into Monoprice’s recessed sensors. Make sure not to buy the Stitch version (Monoprice’s new line of WiF smart devices) as they are not compatible with any of the home automation hubs.

For $20, I was expecting a low-profile sensor, but the sensors are reliable and that is most important. 

#### Installation and Smart Home Integration
The maximum gap between the sensor and magnet is 0.4”, which is slightly smaller than the other door sensors I tested. If you plan to use this sensor with the garage door, that is unlikely to go well without workarounds. 

Pairing the sensors is straightforward in SmartThings and Home Assistant, so I won’t go over it here. There is a tamper switch located on the back of the sensor, but is only usable with a SmartThings device handler that is locked behind a paywall. Device handlers are nice to have to access more details (like battery level), but not necessary.

![SmartThings Door sensors typically look like this in ST.](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1550701653225_door_sensor-monoprice-STapp.png)
![Home Assistant This is how a door sensor looks like in HA](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1550701436096_door_sensor-monoprice-app.png)


### Visonic Door Sensor (MCT-340E) 
![](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1550703237012_visonic-logo.jpg)
![](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1550703247184_door_sensor-visonic-photo01.jpg)


I bought the Visonic Door Sensor (MCT-340E) on a whim because they were so cheap ($10), but the small profile, battery size (CR2032), and reliability convinced me that this would make a solid budget recommendation. The sensor also monitors temperature, though I have never received an accurate reading. If you don’t have any issues with your Zigbee network, then I would recommend giving these sensors a try.

Sidenote: the sensor is $5 cheaper at mydigitaldiscount.com, where I originally bought it for $10.

I have a Wi-Fi mesh network and a small Zigbee network of smart bulbs—both operating on the 2.4ghz frequency—but haven’t run into any connection issues. I would worry about connectivity in a much larger home, but for medium-sized homes and condos, range is not going to be a concern.

#### Installation and Smart Home Integration
Pairing these sensors with Home Assistant can get a little messy (the sensor reports contact and temperature), but pairing with SmartThings is easy. It is one reason I still recommend SmartThings over Home Assistant, where pairing devices is much more straightforward. 


### Konnected
![](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1550617870171_konnected-logo02.png)
![](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1550617804802_door_sensor-konnected-photo.jpg)


If you already have wired sensors installed from a security system in your home, you should check out the Konnected board, which can reuse those sensors with home automation hubs like SmartThings, Home Assistant and Hubitat. I installed one at a friend’s house and was able to connect four door sensors, a siren, a piezo buzzer, and used the 12V port to power a wall-mounted tablet. Be warned that it is a product with bugs—I spent two days trying to figure out an issue that was eventually resolved with a firmware update.

The cost of a Konnected module ($89) is high, but when you factor in the cost of purchasing wireless sensors at $20-30 each, then the module pays for itself with five wired sensors. I also like the fact that I can use a Honeywell wired siren with Konnected because it’s much louder and effective at scaring off intruders than any wireless siren I’ve tried.


![](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1550723621794_door_sensor-konnected-st_app01.png)
![SmartThings Four Konnected sensors and a siren connected in ST.](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1550723611172_door_sensor-konnected_st_app02.png)
![SmartThings  I frequent the Konnected status page for troubleshooting issues.](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1550712892207_door_sensor-konnected-st_app.png)


#### Installation and Smart Home Integration
This is an advanced DIY installation and requires some study of your previous alarm system. Not every system is compatible, so it’s important to read through the Konnected Support section before purchasing. The Konnected Facebook group is also a friendly group to ask questions—I received responses within an hour of asking, though none of the advice solved my issue. Experience with electrical wiring, voltage, and a lot of patience is needed.