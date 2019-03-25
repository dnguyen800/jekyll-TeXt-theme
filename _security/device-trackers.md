---
layout: article
title: Device Trackers / Presence Sensors
category: home security

---
# Device Tracker/Presence Sensor
**Published on: xx/xx/2019**
**Competitors in this space: **
Hardware: SmartThings, iBeacons, Bluetooth LE devices
Software: SmartThings, Life360, Tile, iCloud, nmap, so many more.

I’ve personally tested the following:

- SmartThings app
- Life360 app
- Tile app
- iCloud
- nmap

### Overview
Presence detection is the ability to detect whether someone approaches or leaves a specified area, like home, at work, or school. Detection can be simple (home/away) or complex (exact GPS coordinates) and relies on a mobile app or physical device—like a Tile tracker—to determine your location. I mainly use device trackers as another data point to enhance automations (e.g. if I arrive at home and open the door, then turn on the lights), and in a few scenarios, to unlock and lock doors. To me, a reliable device tracker is one that can detect I’m home right before I reach the door.

It took some time to find a capable presence sensor that was timely enough to update (within a minute’s notice), but it exists!

#### Things to consider before adding a device tracker

- When designing automations, make sure to test, test, and test. There are odd issues where for one millisecond, the sensor mistakenly reports you are home and opens the garage to intruders.
- Make sure you have consent before installing a GPS tracking app like Tile or Life360.

#### What you get with a presence detection sensor

- Design automations using geofencing like announcements (Dan is arriving home).
- Tell the difference between someone arriving at home and opening the door, versus opening the door. 


### Nmap
![](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1550287217513_device_tracker-nmap-logo.jpg)


Nmap is a network scanning tool that has many uses, though at a basic level it scans the network for connected devices. In Home Assistant, we repurpose the Nmap component as a device tracker: it scans the network for my phone and updates device status to ‘home’ if online, and ‘away’ if offline. I like Nmap as it is a simple, non-intrusive service that doesn’t require installing an app, and doesn’t track location any further than the house. That makes it easy to convince my roommates to use it as they don’t have to do anything on their phones, other than take their phones when they leave the house.

I have one goal with these device trackers, which is to update location status before I reach the door. This lets me unlock the door or open the garage door right as I arrive. In my testing, results have been very positive. Status changes happen in less than a minute. Nmap is fast enough to detect when I’m in the garage, and ~ an automation unlocks the door in time.

#### The Problems
There’s a few things you should know before using nmap. Tracking from away to home is deadly fast, but leaving home takes a few minutes to update status. This is a design choice that is reversible in settings in order to save battery life on the device.  Nmap is limited to tracking on the home Wi-Fi network, so you can’t track whether someone is at work or school.

Nmap’s accuracy is dependent on the signal strength of your network being able to reach just outside your garage or front door. Using a Wi-Fi mesh system or a powerful network router will make this a non-issue. 

#### Installation and Smart Home Integration
Nmap is compatible with Home Assistant only, but the configuration is incredibly easy to fill out.

![Home Assistant:](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1550356635252_device_tracker-nmap-ha.png)



#### The Competition

In my process of finding the right device tracker, I’ve tested a few other platforms and shared my thoughts. At least you will know which ones to skip.

|             | Works in SmartThings | in Home Assistant | Time Accuracy      |                                                                                                                                                                                                                           |
| ----------- | -------------------- | ----------------- | ------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| nmap        |                      | X                 | Less than a minute | Good: Fast status update, no interaction with household members needed. No additional app needed.<br>Bad: Only useful for detecting home/away status. Requires decent Wifi router                                         |
| iCloud      |                      | X                 |                    | Good:<br>Bad: Current Home Assistant implementation requires re-authentication every two months if using two-factor auth. Each person needs to provide iCloud password in Home Assistant, which most don’t want to do.    |
| iBeacons    |                      | X                 |                    |                                                                                                                                                                                                                           |
| Life360     | X                    | X                 | 1 to 2 minutes     | Good: Life360 In Home Assistant, there is only one-minute delay. Can set multiple geofences for home, work, school.<br>Bad: Life360 in SmartThings, I’ve experience a one-hour delay. Provides too much location details. |
| Tile        |                      | X                 | Terrible           | Good: None.<br>Bad: Completely inaccurate. Location update can take hours to days. Provides too much location details.                                                                                                    |
| Nest        |                      | X                 | Bad                | Good: None<br>Bad: Requires installation of Nest app and enable ‘Home/Away Assist’ feature to work. Status update ranges from minutes to several hours delay.                                                             |
| SmartThings | X                    | X                 | Terrible           | Good: None.<br>Bad: It never detected when I was away. Location does not update AT ALL unless SmartThings app is opened on user’s phone, which is unlikely.                                                               |

