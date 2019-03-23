---
layout: article
title: Media Streaming Devices
category: gadgets

---
## Smart Displays
** Published on xx/xx/2019**
**Competitors in this space:** Lenovo, JBL, Google, Amazon, Facebook

I’ve personally tested the following:

- Lenovo Smart Display with Google Assistant

### Overview
Smart displays are a relatively new market in 2018, and I have yet to find what they do best. It is definitely NOT a tablet, for it doesn’t have a web browser or any applications designed for it.  If you think of it as a voice assistant that can visually display search results and as a Chromecast combined, then you can start to appreciate it what it does well. However, it is not an essential item to any smart home yet.

For the right price, I would still prefer a smart display than a dedicated tablet, mainly because of the the better overall voice assistant experience. I have tried using Alexa Hands-free on Fire HD tablets, and the experience is not good. Either the tablet is too slow to respond, or it failed to recognize my voice with its single microphone.

#### Considerations before buying a smart display

- A smart display is not a tablet and never will be. It lacks a web browser and dedicated apps. 
- Home Assistant, SmartThings apps aren’t available, though you can access devices connected to Google Assistant.

#### What you get with a smart display

- A dedicated voice assistant with a visual display for photo frame, clock, weather.
- A Chromecast device to cast videos and music to.
- A digital photo frame that connects to Google Photos.
- Basic control of lighting—anything controllable with Google Assistant works here.
- A basic recipe display from the more popular food recipe sites.

### Lenovo Smart Display 10” with Google Assistant

![](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1546983863630_smart_display-lenovo10-photo.jpg)


The Lenovo Smart Display was the first decent Google Assistant-powered smart display to be released, but with the recent pivot of Android Things platform, the future of the display looks grim. Despite having some useful features like Chromecast Built-in, and a quality display, speaker and microphones, app support is limited and unlikely to come in the future. No developer is going to work on a platform for smart displays only when there are other platforms supporting a wider variety of devices.

There have been some fire sales going on for this 10” display—selling for as low as $120, which is not bad for a nice digital photo frame and quality speakers. As long as you expect the Lenovo display to be a voice assistant and not much more, then that price is a steal. It is a fully functional Chromecast—it works with video and audio apps, including multi-room audio with Google Home speakers.

#### The Problems

I initially had Wi-Fi issues where the display would lose connection and force me to run the setup process again, but I learned the root cause of the issue was with the refurbished TP-Link Onhub router I used. Once I replaced it with a Google Wifi point, I no longer had any trouble streaming videos or maintaining a consistent connection on the display.

I bought this display with the intention to use as a cooking assistant. Setting timers, doing conversion, and reading recipes. It was annoying to say “Okay Google, next step” for every single recipe step. Recipes from lesser known blog sites don’t work, and I have no other way to load my private collection of recipes. As a kitchen assistant, it could definitely be better.

#### Installation and Smart Home Integration
The display is a fully functional Chromecast and is automatically detected in Home Assistant as such. It is the best media player integration I’ve tested so far.

For controlling lights, the display cannot access the Home Assistant UI, but can indirectly control through voice, which will bring up the screen below:


![Image: Lenovo Example of controlling lights with the display. You first must use your voice to control the light.](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1551472873372_smart_display-lenovo-photo01.jpg)


I rarely use this function as it’s not effective as using my voice to turn on lights and other devices.