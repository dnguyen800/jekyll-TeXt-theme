---
layout: article
title: AV Receivers
category: media

---

## AV Receivers
![Image: Denon.jp](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1551422856236_av_receiver-denon.jpg)


**Competitors in this space:** Onkyo, Pioneer, Sony, Denon, Yamaha, Marantz

I’ve personally tested the following:

- Pioneer VSX-1131 (2016)
- Onkyo TX-NR509 (2011)

### Overview
These days, most people don’t own AV receivers and the massive speakers that accompany them. They are bulky and tend to dominate the living room space, so I usually recommend customers invest in a good sound bar for home theater quality sound. If you still want or already have a receiver, you might as well integrate it with the rest of the smart home. Luckily, the latest AV receivers are easy to integrate into Home Assistant!

There aren’t many AV receiver brands out there, which is good because it’s easier to add support to Home Assistant for the few remaining receivers out there. There is a compatibility list for some integrations, like Denon, but the only way to find out if a specific model works is to try it yourself. If the AV receiver doesn’t have network capabilities, then a universal remote like the Logitech Harmony can achieve some integration, but lacks features like state awareness (i.e. knowing if a device is on or off).

Voice control is possible if you set up the Home Assistant Cloud with Google Assistant or Alexa, but that shouldn’t be necessary as powering on and changing AV receiver inputs should be handled automatically through HDMI-CEC and ARC.

A friend recently asked for AV receiver recommendations, which made me realize how easy it is to buy the wrong AV receiver. From my experience, there are several considerations before buying an AV receiver and HDMI cables:

#### Considerations before buying an AV receiver

- The receiver should have at least FOUR HDCP 2.2 ports, which is necessary for 4K video. Not all HDMI ports on the receiver are HDCP 2.2. compatible, even the expensive receivers.
- The receiver and TV should support HDMI ARC (Audio Return Channel) or eARC, which allows the TV to send audio to the soundbar or AV receiver with a single HDMI cable. This is important if you use the TV’s smart apps and want surround sound. 
- The receiver and TV should support HDMI-CEC, also called: Samsung Anynet+, LG  SimpLink, and Sony Bravia Sync. CEC lets devices control the TV and AV receiver inputs automatically. It also allows the TV to automatically turn on the AV receiver.
- HDMI cables must be rated at 18gbps to support 4K resolution at 60 frames-per-second. 10gbps is not 4K. In-wall cables should be rated as CL2 to CL3. It’s a safety thing.
- Check the Home Assistant component page to see if your brand AVR is supported.

#### What you get with a network-enabled AV receiver

- Get rid of remotes since HDMI ARC, CEC can turn on the TV and change inputs for you.
- Universal remote control of the media center in Home Assistant.
- More specific automations (if Chromecast Audio is playing, then turn on the receiver).


### Onkyo Receivers
![](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1546919338766_avr-onkyo-logo.png)


My 2011 Onkyo TX-NR509 receiver is an ancient relic, but surprisingly, it is fully compatible with Home Assistant. Thanks to those folks who reverse-engineered Onkyo’s API, the receiver correctly reports the power and input state instantly in Home Assistant, and I can remotely turn on change inputs within the UI. Installation is a breeze—find the receiver’s IP address and you’re basically done.

#### Installation and Smart Home Integration
In the AV receiver settings, turn off any power saving mode, and enable network standby option. This is necessary for Home Assistant to remotely turn on the receiver.

![Google Assistant: It works Technically works through Home Assistant, but I never need to use it.](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1551423197899_google_assistant.jpg)
![Home Assistant Every integrated receiver looks like this in Home Assistant. We have full control, including power and input.](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1546917636813_avr-onkyo-ha.PNG)


### Pioneer
![](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1546919347016_avr-pioneer-logo.png)

As of 2014, Pioneer and Onkyo are effectively the same company! I tested the 2016 Pioneer VSX-1131 receiver and found out that it uses the same network tech as Onkyo, making it fully controllable with Home Assistant. Another plus is that the receiver can be powered on over Wi-Fi, which is not always true for every receiver. 

#### Installation and Smart Home Integration
In the AV receiver settings, turn off any power saving mode, and enable network standby option. This is necessary for Home Assistant to remotely turn on the receiver.

#### Recommended Reading

- HDMI CEC, ARC, and eARC Explained 
- Home Assistant Onkyo Component
