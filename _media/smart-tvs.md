---
layout: article
title: Smart TVs
category: media

---
## Smart TVs

Published xx/xx/2019

![Image: Jens Kreuter @ Unsplash](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1551307746560_smart_tv-front_page-jens-kreuter-85328-unsplash.jpg)


**Competitors in this space:** LG, Samsung, Sony, Vizio, TCL, Philips, Sharp, Toshiba

I’ve personally tested the following:

- Vizio P-Series 65” 2015 model
- LG OLED65C8PUAp 65” (2017 model)
- Sony XBR900F 55”
- Samsung UN55J620DAF 55” (2016)

### Overview
My goal is to keep things simple in life, but that can be hard to achieve with a home theater. I’m still working on reducing the number of remotes down to one, but I’m getting close with the help of two features you likely didn’t realize existed in your TV: HDMI-CEC and HDMI ARC (Audio Return Channel). 

Let’s start with HDMI-CEC, which goes under the following names: Samsung Anynet+, LG SimpLink, and Sony Bravia Sync. You need to enable this feature in the TV settings, as most TVs have it disabled by default. Any CEC-compatible device connected to the TV has the ability to turn on the TV and change TV inputs. You may have noticed this when powering on a Playstation 4 and the TV automatically turns on and switches to the PS4 input. That is CEC in action. CEC also works with AV receivers (in theory) to change HDMI input to the active device.  Unfortunately, CEC implementation is finicky and requires a lot of testing to get it working properly. I was able to do it though, so don’t give up!


![Image: Denon.jp](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1551399991739_av_receiver-denon.jpg)


If you have a TV and AV receiver or soundbar that are ARC compatible, then you can finally put away your AV receiver remote for good. ARC allows the TV to send audio to the soundbar or AV receiver using a single HDMI cable, and subsequently, AV receiver volume is controllable with the TV remote. There are limitations as ARC doesn’t support every audio format, but that is resolved by connecting the device directly to the AV receiver. 

As you can tell, there is a lot of automation you can do to cut down to one remote, but it will come with a lot of restrictions. I recommend trying out HDMI-CEC and ARC with your existing setup, and whatever doesn’t work, we address with Home Assistant, Logitech Harmony or new AV gear.

Anyways, back to smart homes and smart TVs. If your TV is 2016 or newer, I have good news for you! Your TV can integrate with Home Assistant to support some very useful universal remote functions and lighting automations. We can do everything a Logitech Harmony remote can do and more, now that we have the ability to detect the TV’s state.


![An example of the universal remote control function I created in Home Assistant. Buttons light up depending on TV input.](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1551316748133_home_assistant-media.jpg)


I find it easier using a tablet to navigate through my media center controls. People can use it without much explanation—in the screenshot above, I can already tell the TV and receiver is on and the Playstation 4 is playing by looking at the green highlighted buttons on the UI.

For lighting automations, we can use the TV’s state to determine whether to dim the lights, though it is more accurate to design automations around the media devices themselves (Roku, Xbox One, etc).


![](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1551404586938_whitespace.png)
![Image: Bestbuy](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1551404556505_smart_tv-harmony-photo02.jpg)
![](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1551404569540_whitespace.png)


If your TV doesn’t have HDMI-CEC, ARC or any integration with Home Assistant, then a universal remote like the Logitech Harmony hub can achieve a similar effect and reduce the number of remotes you need. The main downside is that it cannot detect whether a device is on or off, so some devices might get turned off accidentally. 

People are going to buy the TV they can want, regardless of my recommendations. So instead of my usual format, I’ll highlight my experiences working with different TV brands and how well they integrate with Home Assistant. 

#### Considerations before buying a smart TV

- The brand you select will limit your media service options. Fire TVs don’t support Youtube and Youtube TV. Roku TVs seems to support everything.
- Does the TV support HDMI-CEC and ARC or its successor, eARC? Does it support advanced CEC functions, like arrow keys, or play/pause?

#### What you get with a Smart TV

- Use the tablet as a stylish universal remote
- Pair media center lighting with TV power state (“if TV is on, turn on TV lighting)

### LG WebOS TVs

![](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1546815630656_tv-lg_webos-logo.png)


I was lucky enough to test one of the 2018 LG OLED TVs and was pleasantly surprised to see how mature the WebOS platform has become. The interface is snappy and responsive, the gyroscopic remote controls make it as easy as possible for anyone to pick up a remote and intuitively browse through the TV’s wide selection of apps. All popular video apps are supported and load instantly, and Home Assistant integration is easy to do and fully supports media controls. The only downsides that are the ‘Power On’ function doesn’t work reliably without a wired network connection, and apps like Youtube don’t display any video details. Other than that, there is no need to get a Chromecast or Fire TV stick if you have a LG WebOS TV.

Google Assistant integration exists, allowing you to turn on the TV or change the volume with your voice. It’s a nice unused feature to have.

#### Installation and Smart Home Integration


![Voice: Official Integration Easy to setup through Google Home.](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1543622841706_google_assistant.jpg)
![Home Assistant: Unofficial Integration Pairs easily after enabling settings and entering token code. HA shows image of currently playing app.](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1551316789026_smart_tv-webos-ha.PNG)

![SmartThings: N/A](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1551316824303_not_available.png)
![LG TV App Basically an LG remote on your phone.](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1551317037895_smart_tv-lg-app01.png)


#### Recommended Reading

- LG WebOS Home Assistant component
- Connect LG TV with Google Assistant and Amazon Alexa article


### Sony Bravia TVs

![](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1546816698857_tv-sony_bravia-logo.png)

I briefly tested the Sony Bravia XBR X900F, which has Android TV, Google Assistant, and Chromecast Built-in. You would think that with all these Google parts inside, it should be some kind of sentient mega TV, but it isn’t. Chromecast works as expected, but Google Assistant doesn’t work unless the TV is on. I can’t turn on the TV with my voice unless I have another Google Home speaker nearby.  Android TV is still a slow, dull user interface, but it’s not bad enough to the point where a media streaming device is needed. 

#### Installation and Smart Home Integration
Besides those minor complaints, the TV integrates with Home Assistant using the Bravia TV component easily. Powering on, changing inputs, and reporting power state works, though it takes a few seconds to update state.