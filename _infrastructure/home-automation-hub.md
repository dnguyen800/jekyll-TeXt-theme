---
layout: article
title: Home Automation Hub
category: Infrastructure

---

## Home Automation Hub

**Published xx/xx/2019**

![img](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1551223210457_security_system-smartthings-photo.jpg)

**Competitors in this space:** Home Assistant, OpenHAB, Samsung Smartthings, Hubitat, Wink, Insteon Hub, Fibaro, Almond, Vera, Abode, and many more.



I’ve personally tested the following:

- Samsung SmartThings v2 hub
- Home Assistant v0.88 using Raspberry Pi 3B+ and GoControl HUSBZB-1 radio


### Overview
I bet there is confusion about the need for a home automation hub, especially if you are already familiar with Google Home and the app. Yes, Google Home and the app can control the lights, outlets and other devices, but you still have to use your voice or the app, and that gets tiring really quick. If you want to reach true laziness — where the lights turn on before you even think about it — a hub is needed. To do more advanced routines like opening the garage automatically when arriving at home, a hub is the only way to do it.


There are a few reasons why a hub is needed, for now). All your devices communicate through protocols—Zigbee, Z-Wave, Wi-Fi, RF, and Bluetooth LE are the most common standards. Also, some devices are fenced off from interacting with devices, but others have application programming interfaces (better known as APIs) to allow for intercommunication. A home automation hub has the hardware and software to send and receive those communications and APIs, and thus becomes like a command center—


1. The hub gets periodic or real-time updates from the devices (“the TV just turned on”) 
2. The hub runs routines if certain conditions are met(“if TV is on and it is after sunset…”) 
3. Then takes action and sends commands to the devices through device APIs or other means (“then turn on the TV lighting”). 


The more devices you connect to the hub, the more control and data points it has for you to design smarter routines and automations. 


Before going out to Best Buy and buying a home automation hub, there is nothing wrong with stopping here and becoming familiar with the smart devices you have. I think it’s a good idea to hold off because the home automation hubs I’ve tested are still not stable enough and could use a few year(s) of development.  In the meantime, look for a sale on Smartthings or Raspberry Pi hardware if you’re willing to test the unstable waters.


There are many home automation hubs to choose from that perform similar functions, but the implementation is very different for each. There is no way to know what hub is best for you unless you do the research and watch some demonstrations on Youtube. Even the Wirecutter, who previously recommended SmartThings, redacted their article about because they couldn’t agree on a recommendation. [Tom’s Guide](https://www.tomsguide.com/us/best-smart-home-hubs,review-3200.html) recommends SmartThings, but it’s not a thorough analysis, nor does it talk much about the cons. 


#### What to Consider Before Buying a Hub

- **Internet reliance.** SmartThings is heavily reliant on an Internet connection to function. If internet connectivity is spotty in your area, consider a hub that can operates locally, like Home Assistant or Hubitat.
- **Device compatibility** **with the big name IoT devices** like thermostats, security cameras, TVs, media centers, smart assistants. Some hubs have only a few, but tested integrations. The hubs that advertise 100+ integrations are likely unofficial that can break at any time (see [Logitech Harmony breaking XMPP integration](https://www.theverge.com/circuitbreaker/2018/12/20/18150011/logitech-harmony-hub-remote-setup-security-update-broken-third-party-local-api)) or difficult to setup. 
- **Sensor Compatibility.** Buying a Z-Wave or Zigbee sensor doesn’t guarantee that it will work with your Z-Wave compatible hub.  SmartThings and Home Assistant have the highest compatibility, but it is still a good idea to research online before buying a sensor.
- **Having a mobile app** is important for getting notifications and remote control of your smart devices. If you don’t mind having separate apps for thermostat, lighting, then this app is not as critical.
- **Product Support.** Is the product still sold in stores or being actively developed by the  community? If not, the hub likely won’t support any new integrations or security updates.



#### What you get with a home automation hub

- True home automation! A smart home where things happen without having to use your voice or flip a switch. 
- A way to control your lights and other connected devices remotely.
- A nice looking user interface, if you use Home Assistant.





### Samsung SmartThings and Home Assistant

![img](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1545950128785_home_assistant_logo.png)![img](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1545950253055_smartthings_logo.png)

**Using** **Samsung SmartThings and Home Assistant together provides the functionality I need to do a proper media-focused smart home, but I hope to remove SmartThings eventually.** I first started off with SmartThings, then tried Home Assistant, and eventually decided to use both hubs together to leverage their strengths and mitigate weaknesses. 


In my solution, SmartThings became the reliable one (I know, debatable) that handles communications between most devices and performs basic light automations. I paired sensors, the Philips Hue hub, MyQ garage door opener, Ecobee thermostat and Google Assistant to SmartThings pretty easily. The SmartThings mobile app handles notifications and remote access to my devices. It’s fairly easy to setup these features, which is why I recommend SmartThings to beginners who don’t have experience with setting up port forwarding, DNS, reverse proxies, SSL encryption, and so on.

![img](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1551238686170_smartthings_app.PNG)

#### The Problems

But that’s about all that SmartThings can do well. There is no product roadmap nor any interesting product developments or integrations in the past year, besides releasing a cheaper, slightly less functional hub. SmartThings notifications are more delayed when using the latest Android OS—as much as a 15 minutes! There is no way I can use SmartThings as a security system with these delays. I’ll keep the hub around until I get  Home Assistant running stable.



![img](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1551238960653_homeassistant02.jpg)

Speaking of Home Assistant, it is an amazing, unstable platform that I use for its slick UI, hundreds of integrations, and advanced media automations. It is open source and can be run on cheap hardware like a Raspberry Pi 3B+, but nothing slower than that. Though not every integration is easy to set up, Home Assistant works with the latest and greatest products, from TVs and AV receivers to robot vacuums, lights, and homemade hardware. Without Home Assistant, I would have given up on home automation altogether, after being disappointed by SmartThings’ inability to do anything I would consider “smart.”


Home Assistant is necessary to do media automations that can show off the home theater. In my setup, Home Assistant acts like a universal remote, but much smarter — it knows what devices are powered on and what they’re doing.  Google Assistant integration with Home Assistant also allows provides much better voice control over media devices. I have several example of how Home Assistant has automated a few things in my home:


- Home Assistant can broadcast a message on Chromecast Built-In speakers if someone is arriving home, a door is unlocked, or whatever you can think of.
- Chromecast Audio cannot turn on an AV receiver on its own, but Home Assistant can detect when the Audio is playing music and turn on the receiver. 
- The Xbox One cannot turn on the TV on its own, but using Home Assistant, I can detect when the Xbox One is on, and turn on the TV accordingly.
- The dashboard can shows music currently playing on Spotify, Plex, or any Chromecast speaker, along with media controls and cover art.


#### The Problems

Home Assistant is amazing software, but it’s not for beginners. The learning curve is high; with lots of text editing and YAML syntax required. The limited documentation is difficult for newcomers to grasp. When Home Assistant crashes (and it will), a technical person needs to be there to fix it. The instability is one of the reasons I keep SmartThings around, so the at least lighting continue to work if Home Assistant is down. I say give Home Assistant another year of development and it will be even more user-friendly to use.

 
To achieve integration with SmartThings and Home Assistant, we use MQTT, a lightweight messaging protocol that translate messages between the two platforms. Once it is set up, any devices in SmartThings appear as native Home Assistant entities. I wrote a [tutorial](https://community.home-assistant.io/t/anyone-integrated-smartthings-into-hassio-yet/25324/7) for an older version of Home Assistant, but it’s still usable. As of Home Assistant version 0.87, there is an [integration](https://www.home-assistant.io/components/smartthings/) with SmartThings that makes it even easier to connect, though it requires exposing your Home Assistant instance to the internet.



#### The Competition

I’ve been looking into a new Smartthings competitor called Hubitat. Detailed reviews aren’t common for Hubitat, but I gather it is a better version of SmartThings, but missing a few things like a proper mobile app. I decided against ordering Hubitat as it didn’t support the standard Lutron Caseta bridge, which I use at my house.



#### Recommended Reading

- SmartThings amazon.com link
- Device handlers
- WebCoRE for SmartThings lets users build complex automation ~. The tool is almost as easy as English.
- Forum post detailing integration of SmartThings with Home Assistant using MQTT, written by yours truly!
- Home Assistant website. Learn how to install and configure it, or just be overwhelmed. 
- My Home Assistant configuration—great for viewing automation and Lovelace UI examples

