---
layout: article
title: Home Automation Hub
short_title: Home Automation Hub
excerpt: One of the most critical infrastructure components to your smart home.
category: [infrastructure, home automation]
permalink: /infrastructure/home-automation-hub
key: infrastructure-home_automation_hub
aside:
  toc: true
banner: assets/images/overlay/home-automation-hub.jpg
mode: immersive
header:
  theme: dark
article_header:
  type: overlay
  theme: dark
  background_color: '#203028'
  background_image:
    gradient: 'linear-gradient(135deg, rgba(34, 139, 87 , .4), rgba(139, 34, 139, .4))'
    src: /assets/images/overlay/home-automation-hub.jpg
---

<!--more-->

**Competitors in this space:** Home Assistant, OpenHAB, Samsung Smartthings, Hubitat, Wink, Insteon Hub, Fibaro, Almond, Vera, Abode, and many more.



I’ve personally tested the following:

|---
| ![](\assets\images\logo\smartthings.png){:.image--lg} |  ![](\assets\images\logo\home-assistant.png){:.image--sm} 
|:-:|:-:
| **SmartThings v2** | **Home Assistant 0.90 (Hass.io version)** 


## What you need to know
I bet there is confusion about the need for a home automation hub, especially if you are already familiar with Google Home and the app. Yes, Google Home and the app can control the lights, outlets and other devices, but you still have to use your voice or the app, and that gets tiring really quick. If you want to reach the point of true laziness — where the lights turn on before you even think about it — a hub is needed. To do more advanced routines like opening the garage automatically when arriving at home, a hub is the only way to do it, for now.


There are a few reasons why a home automation hub is still needed, for now. All your devices communicate through protocols—Zigbee, Z-Wave, Wi-Fi, RF, and Bluetooth LE are the most common standards. Also, some devices are fenced off from interacting with devices, but others have application programming interfaces (better known as APIs) to allow for intercommunication. A home automation hub has the hardware and software to send and receive those communications and interact with APIs, and thus becomes like a command center. At a basic level, the hub performs the following:


> 1. The hub gets periodic or real-time updates from the devices (“the TV just turned on”) 
> 2. The hub checks against its automations if certain conditions are met(“if the TV is on and it is after sunset…”) 
> 3. Then takes action and sends commands to the devices through device APIs or other means (“then turn on the TV lighting”). 


The more devices you connect to the hub, the more control and data points it has for you to design smarter routines and automations. 


Before going out to Best Buy and buying a home automation hub, there is nothing wrong with stopping here and becoming familiar with the smart devices you have. I think it’s a good idea to hold off because the home automation hubs I’ve tested are still not stable enough and could use a few year(s) of development.  In the meantime, look for a sale on Smartthings or Raspberry Pi hardware if you’re willing to go further. 

There are many home automation hubs to choose from that perform similar functions, but the implementation is very different for each. There is no way to know what hub is best for you unless you do the research and watch some demonstrations on Youtube. Even the Wirecutter, who previously recommended SmartThings, redacted their article about because they couldn’t agree on a recommendation. [Tom’s Guide](https://www.tomsguide.com/us/best-smart-home-hubs,review-3200.html) recommends SmartThings, but I don't think it is a thorough analysis that covers the cons. 

### What to Consider Before Buying a Hub

> - **Internet reliance.** SmartThings is heavily reliant on an Internet connection to function. If internet connectivity is spotty in your area, consider a hub that can operates locally, like Home Assistant or Hubitat.
> - **Device compatibility** **with the big name IoT devices** like thermostats, security cameras, TVs, media centers, smart assistants. Some hubs have only a few, but tested integrations. The hubs that advertise 100+ integrations are likely unofficial that can break at any time (see [Logitech Harmony breaking XMPP integration](https://www.theverge.com/circuitbreaker/2018/12/20/18150011/logitech-harmony-hub-remote-setup-security-update-broken-third-party-local-api)) or difficult to setup. 
> - **Sensor Compatibility.** Buying a Z-Wave or Zigbee sensor doesn’t guarantee that it will work with your Z-Wave compatible hub.  SmartThings and Home Assistant have the highest compatibility, but it is still a good idea to research online before buying a sensor.
> - **Having a mobile app** is important for getting notifications and remote control of your smart devices. If you don’t mind having separate apps for thermostat, lighting, then this app is not as critical.
> - **Product Support.** Is the product still sold in stores or being actively developed by the  community? If not, the hub likely won’t support any new integrations or security updates.



### What you get with a home automation hub

> - True home automation! A smart home where things happen without having to use your voice or flip a switch. 
> - A way to control your lights and other connected devices remotely.
> - A nice looking user interface, if you use Home Assistant.

### Recommended Reading

> - Purchase SmartThings through amazon.com
> - SmartThings device handlers
> - [WebCoRE for SmartThings](https://wiki.webcore.co/) lets users build complex automations. The tool is almost as easy as writing English.
> - Forum post detailing integration of SmartThings with Home Assistant using MQTT, written by yours truly!
> - [Get started with Home Assistant!](https://www.home-assistant.io/getting-started/) Learn how to install and configure it, or just be overwhelmed. 
> - [My Home Assistant configuration](https://github.com/dnguyen800/home-assistant-configuration-example) —great as a learning tool for building the UI.




## Samsung SmartThings and Home Assistant

![Home Assistant logo](\assets\images\logo\ha-st.png){:.image--lg.align-left}


**Using Samsung SmartThings and Home Assistant together provides the functionality I need to do a proper media-focused smart home, but I hope to remove SmartThings eventually.** I first started off using SmartThings, then tried Home Assistant, and eventually decided to use both hubs together to leverage their strengths and mitigate weaknesses. 


In my solution, __SmartThings__ is the reliable one __(I know, debatable)__ that handles communications between most devices and performs basic light automations. I can pair door and motion sensors, the Philips Hue hub, MyQ garage door opener, Ecobee thermostat and Google Assistant to SmartThings easily enough. 

One of the major selling points for me (and problem for others) with SmartThings is that most features can work remotely out of the box--I get notifications on my phone when something is happening in the house and can remotely control the lights while away. Home Assistant and Hubitat can't do this so easily as SmartThings, though I expect new developments in 2019 from Home Assistant Cloud in the future.

<figure style="width: 100%;" >
 <img src="\assets\images\other\smartthings-app.jpg" alt="An example of the universal remote control function I created in Home Assistant" />
 <figcaption>
The SmartThings Classic UI in tablet mode.
 </figcaption>
</figure>

The UI on the SmartThings Classic app is basic, but it works. You can create the most basic of basic automations through the app, but at least those will always work. There is a new SmartThings app (with a nicer UI) available, but I was unable to get most of my connected devices working with it.

### SmartThings' Problems

But that’s about all that SmartThings can do well. There is no product roadmap nor any interesting product developments or integrations in the past year, besides releasing a cheaper, slightly less functional hub. New official product integrations are non-existent. SmartThings would be a terrible product today if it weren't for the SmartThings community creating workarounds to make up for SmartThings' shortcomings. WebCoRE adds the ability to create advanced automations with conditional statements, but relies on an internet connection to work.

I've also noticed that SmartThings notifications can be delayed when using the latest Android OS—as much as 15 minutes! There is no way I can use SmartThings as a security system with these delays. I’ll keep the hub around until I get Home Assistant running stable.

<figure style="width: 100%;" >
 <img src="\assets\images\other\homeassistant-02.jpg" alt="" />
 <figcaption>
The Home Assistant web interface. It tooks months of learning to get it to this state.
 </figcaption>
</figure>

Speaking of __Home Assistant__, it is an amazing, unstable platform that I use for its slick UI, hundreds of integrations, and advanced media automations. It is open source and can be run on cheap hardware like a Raspberry Pi 3B+, but nothing slower than that. Though not every integration is easy to set up, Home Assistant works with the latest and greatest products--from TVs and AV receivers to robot vacuums, lights, and homemade hardware. Without Home Assistant, I would have given up on home automation altogether, after being disappointed by SmartThings’ inability to do anything I would consider “smart.”

Home Assistant is necessary to do media automations that can show off the home theater. In my setup, Home Assistant acts like a universal remote, but much smarter — it knows what devices are powered on and what they’re currently doing.  Google Assistant integration with Home Assistant also allows provides much better voice control over media devices. I have several example of how Home Assistant has automated a few things in my home:

> - Home Assistant can broadcast a message on Chromecast Built-In speakers if someone is arriving home, a door is unlocked, or whatever you can think of.
> - Chromecast Audio cannot turn on an AV receiver on its own, but Home Assistant can detect when the Audio is playing music and turn on the receiver automatically. 
> - The Xbox One cannot turn on the TV on its own, but using Home Assistant, I can detect when the Xbox One is on, and turn on the TV accordingly.
> - The dashboard can shows music currently playing on Spotify, Plex, or any Chromecast speaker, along with media controls and cover art.

<figure style="width: 100%;" >
 <img src="\assets\images\other\homeassistant-media.jpg" alt="" />
 <figcaption>
Media-focused Home Assistant dashboard I created.
 </figcaption>
</figure>

If you're still curious about Home Assistant, start off by purchasing a Raspberry Pi 3B+ or Asus Tinkerboard S, a high-endurance SD card (for rPi only) and install Hass.io (a more restricted version of Home Assistant) by following this [guide](https://www.home-assistant.io/getting-started/). If you're an IT guru and have an existing server and Docker platform ready, then you can install Home Assistant or Hass.io as a service or Docker container.

I've shared my [Home Assistant configuration](https://github.com/dnguyen800/home-assistant-configuration-example) on Github as a learning example for beginners, though it's already become outdated after only a few weeks. Still, I explain how every Lovelace card and component is used.

### Home Assistant's Problems

Home Assistant is an amazing piece of software, but it is absolutely not for tech novices. The learning curve is high and the limited documentation is difficult for newcomers to grasp. Setting up the UI is difficult at first if editing YAML files directly, though the team is working on improving the UI editor.

When Home Assistant crashes (and it will), a technical person needs to be present to fix it. The instability is one of the reasons I keep SmartThings around, so at least the lighting will continue to work if Home Assistant is down. I say give Home Assistant another year of development and it will be even more user-friendly to use.

To achieve integration with SmartThings and Home Assistant, I use **``MQTT``**, a lightweight messaging protocol that translate messages between the two platforms. Once it is set up, any devices in SmartThings appear as native Home Assistant entities. I wrote a [tutorial](https://community.home-assistant.io/t/anyone-integrated-smartthings-into-hassio-yet/25324/7) for an older version of Home Assistant, but it’s still usable.

{:.info}
As of Home Assistant 0.90, it is possible to use the Home Assistant Cloud and the newly developed SmartThings [integration](https://www.home-assistant.io/components/smartthings/)  to easily connect SmartThings and Home Assistant together. Home Assistant Cloud is not free ($5/month), and I'm sure there are bugs to fix, but it's a good start.


## The Competition
![Hubitat logo](\assets\images\logo\hubitat.png){:.image--lg.align-left}

I’ve been looking into a new Smartthings competitor called Hubitat. In-depth reviews aren’t common for Hubitat, but I gather it is a better version of SmartThings, but missing a few things like a proper mobile app and support for some cloud-based services like Lutron Caseta. I decided against ordering Hubitat as it didn’t support the standard Lutron Caseta bridge, which I currently use at my house. There also aren't any Hass.io add-ons or  integrations to connect with Home Assistant, so I wouldn't be able to use it with my Hass.io instance.




