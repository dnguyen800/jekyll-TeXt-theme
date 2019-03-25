---
layout: article
title: Home Theater
short_title: Home Theater
excerpt: Home theater shit!!!!
category: [media, home theater, home automation]
permalink: /media/home-theater
key: media-home_theater
aside:
  toc: true
banner: assets/images/overlay/home-theater.jpg
mode: immersive
header:
  theme: dark
article_header:
  type: overlay
  theme: dark
  background_color: '#203028'
  background_image:
    gradient: 'linear-gradient(135deg, rgba(34, 139, 87 , .4), rgba(139, 34, 139, .4))'
    src: /assets/images/overlay/home-theater.jpg
---

<!--more-->
<figcaption><b>Image:</b><a href="https://unsplash.com/@jenskreuter"> Jens Kreuter</a></figcaption>


**Quick Links:**
<div class="grid-container">
  <div class="grid grid--p-2">
    <div class="cell cell--3"><a href="/media/home-theater#smart-tvs"><div><div class="card">
      <div class="card__image">
        <img class="image" src="/assets/images/grid/smart-tv.jpg"  />
      </div>
    </div></div></a></div>
    <div class="cell cell--3"><a href="/media/home-theater#video-game-consoles"><div><div class="card">
      <div class="card__image">
        <img class="image" src="/assets/images/grid/videogame.jpg"/>
      </div>
    </div></div></a></div>
    <div class="cell cell--3"><a href="/media/home-theater#av-receivers"><div><div class="card">
      <div class="card__image">
        <img class="image" src="/assets/images/grid/av-receiver.jpg"/>
      </div>
    </div></div></a></div>
    <div class="cell cell--3"><a href="/media/home-theater#media-streaming-devices"><div><div class="card">
      <div class="card__image">
        <img class="image" src="/assets/images/grid/media-streaming-devices.jpg"/>
      </div>
    </div></div></a></div>    
  </div>
</div>

# Smart TVs

**Competitors in this space:** LG, Samsung, Sony, Vizio, TCL, Philips, Sharp, Toshiba

I’ve personally tested the following:

|---
| ![](\assets\images\logo\vizio.png){:.image--md} |  ![](\assets\images\logo\lg-webos.png){:.image--md} | ![](\assets\images\logo\sony-bravia.png){:.image--md} | ![](\assets\images\logo\samsung.png){:.image--md}
|:-:|:-:|:-:|:-:
| **P-Series 65” (2015)** | **OLED65C8PUAP 65” (2017)** | **XBR900F 55” (2018)** | **UN55J620DAF 55” (2016)**

### What you need to know

My goal is to keep things simple in life, but that can be hard to achieve with a home theater. I’m still working on reducing the number of remotes down to one, but I’m getting close with the help of two features you likely didn’t realize existed in your TV: **``HDMI-CEC``** and **``HDMI ARC (Audio Return Channel)``**. 

Let’s start with **``HDMI-CEC``**, which goes by several  names: Samsung Anynet+, LG SimpLink, and Sony Bravia Sync. You need to enable this feature in the TV settings, as most TVs have it disabled by default. Any CEC-compatible device connected to the TV has the ability to turn on the TV and change TV inputs. You may have noticed this when powering on a Playstation 4 and the TV automatically turns on and switches to the PS4 input. That is CEC in action. **``HDMI-CEC``** works with AV receivers (in theory) to change HDMI input to the active device.  Unfortunately, CEC implementation is finicky and requires a lot of testing to get it working properly. I was able to do it though, so don’t give up!

![Image: Denon.jp](\assets\images\overlay\av-receiver.jpg)

If you have a TV and AV receiver or soundbar that are ARC compatible, then you can finally put away your AV receiver remote for good. ARC allows the TV to send audio to the soundbar or AV receiver using a single HDMI cable, and subsequently, AV receiver volume is controllable with the TV remote. There are limitations as ARC doesn’t support every audio format, but that is resolved by connecting the device directly to the AV receiver. 

As you can tell, there is a lot of automation you can do to cut down to one remote, but it will come with a lot of restrictions. I recommend trying out **``HDMI-CEC``** and **``ARC``** with your existing setup, and whatever doesn’t work, we address with Home Assistant, Logitech Harmony or new AV gear.

Anyways, back to smart homes and smart TVs. If your TV is 2016 or newer, I have good news for you! Your TV can integrate with Home Assistant to support some very useful universal remote functions and lighting automations. We can do everything a Logitech Harmony remote can do and more, now that we have the ability to detect the TV’s state.

<figure style="width: 100%;" >
 <img src="\assets\images\other\homeassistant-media.jpg" alt="An example of the universal remote control function I created in Home Assistant" />
 <figcaption>
An example of the universal remote control function I created in Home Assistant. Buttons light up depending on TV input.
 </figcaption>
</figure>

I find it easier using a tablet to navigate through my media center controls. People can use it without much explanation—in the screenshot above, I can already tell the TV and receiver is on and the Playstation 4 is playing by looking at the green highlighted buttons on the UI.

For lighting automations, we can use the TV’s state to determine whether to dim the lights, though it is more accurate to design automations around the media devices themselves (Roku, Xbox One, etc).

 ![](\assets\images\other\logitech-harmony.jpg){:.image--xl.align-left}

If your TV doesn’t have **``HDMI-CEC``**, **``ARC``** or any integration with Home Assistant, then a universal remote like the Logitech Harmony hub can achieve a similar effect and reduce the number of remotes you need. The main downside is that it cannot detect whether a device is on or off, so some devices might get turned off accidentally. 

People are going to buy the TV they can want, regardless of my recommendations. So instead of my usual format, I’ll highlight my experiences working with different TV brands and how well they integrate with Home Assistant. 

### Considerations before buying a smart TV

> - The brand you select will limit your media service options. Fire TVs don’t support Youtube and Youtube TV. Roku TVs seems to support everything.
> - Does the TV support HDMI-CEC and ARC or its successor, eARC? Does it support advanced CEC functions, like arrow keys, or play/pause?

### What you get with a Smart TV

> - Use the tablet as a stylish universal remote
> - Pair media center lighting with TV power state (“if TV is on, turn on TV lighting)

### Recommended Reading

> - LG WebOS Home Assistant component
> - Connect LG TV with Google Assistant and Amazon Alexa article

## LG WebOS TVs

 ![](\assets\images\logo\lg-webos.png){:.image--xl.align-left}

I was lucky enough to test one of the 2018 LG OLED TVs and was pleasantly surprised to see how mature the WebOS platform has become. The interface is snappy and responsive, the gyroscopic remote controls make it as easy as possible for anyone to pick up a remote and intuitively browse through the TV’s wide selection of apps. All popular video apps are supported and load instantly, and Home Assistant integration is easy to do and fully supports media controls. The only downsides that are the ‘Power On’ function doesn’t work reliably without a wired network connection, and apps like Youtube don’t display any video details. Other than that, there is no need to get a Chromecast or Fire TV stick if you have a LG WebOS TV.

Google Assistant integration exists, allowing you to turn on the TV or change the volume with your voice. It’s a nice unused feature to have.

### Installation and Smart Home Integration

#### Integrations 

<figure class="figure figure--25">
 <img src="/assets/images/integrations/lg-webos-ha.png" alt="Small picture of a kitten" />
 <figcaption>
 <b>Home Assistant: Good</b><br>Several steps to complete on HA and the TV.
 </figcaption>
</figure>

<figure class="figure figure--25">
 <img src="/assets/images/integrations/google-home.png" alt="Small picture of a kitten" style="width: 100%" />
 <figcaption>
 <b>Voice: Great</b><br>Pair the TV using the Google Home app.
 </figcaption>
</figure>

<figure class="figure figure--25">
 <img src="/assets/images/integrations/na.png" alt="Small picture of a kitten" style="width: 100%; height: 100%" />
 <figcaption>
 <b>SmartThings: None</b><br> Integration does not exist.
 </figcaption>
</figure>

<figure class="figure figure--25">
 <img src="/assets/images/integrations/lg-webos-app.png" alt="Small picture of a kitten" style="width: 100%" />
 <figcaption>
 <b>Native App: Great</b><br>It's an LG remote on your phone!
 </figcaption>
</figure>



## Sony Bravia TVs

 ![](\assets\images\logo\sony-bravia.png){:.image--xl.align-left}

I briefly tested the Sony Bravia XBR X900F, which has Android TV, Google Assistant, and Chromecast Built-in. You would think that with all these Google parts inside, it should be some kind of sentient mega TV, but it isn’t. Chromecast works as expected, but Google Assistant doesn’t work unless the TV is on. I can’t turn on the TV with my voice unless I have another Google Home speaker nearby.  Android TV is still a slow, dull user interface, but it’s not bad enough to the point where a media streaming device is needed. 

### Installation and Smart Home Integration

Home Assistant sees the Bravia TV as two separate entities: a Chromecast and Android TV media player. Using the **``Bravia TV component``** is easy to connect. Powering on, changing inputs, and reporting power state works, though it takes a few seconds to update state. 

The TV has Chromecast Built-In, which is detected automatically in Home Assistant using the **``Discovery``** component. It works just like the [Chromecast](\media\home-theater#chromecast).


# Video Game Consoles
<figure style="width: 100%;" >
 <img src="\assets\images\overlay\videogame.jpg" alt="An example of the universal remote control function I created in Home Assistant" />
 <figcaption>
<b>Image:</b> Fabian Albert on <a href="https://unsplash.com/@serumfabian">Unsplash</a>
 </figcaption>
</figure>

**Published xx/xx/2019**

**Competitors in this space:** Microsoft, Sony, Nintendo

I've personally tested the following:

|---
| ![](\assets\images\logo\xboxone.png){:.image--lg} |  ![](\assets\images\logo\sony-ps4.png){:.image--lg} | ![](\assets\images\logo\nintendo.png){:.image--lg} 
|:-:|:-:|:-:
| **Xbox One X** | **Playstation 4 Pro** | **Nintendo Switch** 


## What you need to know

Video game consoles have always been a part of my media center, so it would be a glaring omission if I couldn’t include them in my smart home automations. I use them as blu-ray players for those rare occasions I revisit an old movie. The Xbox One makes for a noteworthy media streaming device—even segregated apps like Youtube TV, Amazon Video are available. If I had to choose only one device connected to my TV, it would likely be a videogame console because it plays games, blu-rays, and most major apps.

Consoles aren’t known to be open platforms, but several clever people developed ways to connect the Xbox One and Playstation 4 consoles to Home Assistant. These are unofficial methods that Sony or Microsoft could discontinue in the future, but I’ll give it a couple of years before that happens.

With Home Assistant integrations, I can see the game currently playing (see examples below). Not exactly useful, but it sure looks nice on the UI. The other benefit is that my TV lighting automations will be even more precise, now that I can detect if a game is playing.

### Considerations before buying a video game console

> - Only the Xbox One S and X support 4K Blu-ray. Playstation 4 Pro can play regular Blu-rays only.
> - If you use it as a media streaming device, you should purchase a media remote or use a Logitech Harmony remote.

### What you get with integrating a video game console

> - Create more accurate lighting automations (e.g. turn on the lights when a game is playing).
> - Use as a blu-ray player (XboxOne S & X supports 4K).
> - Supports video and music apps like Hulu, Spotify, Netflix.
> - Integration looks cool on Home Assistant.

### Recommended Reading

> - Use Alexa on XboxOne support article
> - Link to my Home Assistant configuration for Playstation 4 media player
> - Playstation 4 Home Assistant custom component
> - Xbox One Hass.io add-on
> - Playstation 4 Hass.io add-on tutorial by user @cheynespc

## Microsoft Xbox One
 ![](\assets\images\product-photo\xboxone.png){:.image--xl.align-left}

When the Xbox One launched in 2013, it was supposed to be the ultimate media center where you could play games and watch TV—all on the same screen! Well, that idea failed horribly but the Xbox One gained some awesome features recently, like a 4K bluray player and plenty of video apps (Youtube TV, Hulu, Spotify). Smart home integration was recently added in the form of a Home Assistant (Hass.io) add-on and it’s quite impressive, with the ability to display the game currently playing in Home Assistant—all without any manual intervention. 

### The Problems

I’ve run into a few issues, like having to re-authenticate my Xbox account from time to time. It’s not a completely hands-off integration, but it’s not a critical component that I can survive without it working. 

### Installation and Smart Home Integration

The initial setup on Home Assistant is only difficult if you don’t read the instructions.  Install the Hass.io addon and authenticate to Xbox Live per the add-on instructions. Find your Xbox One’s device ID (see instructions again), then add the Xbox One media player platform and device ID in your configuration.yaml file. Be sure to read the instructions thoroughly!

Xbox status updates to Home Assistant are quick—within one to two seconds—so lighting automations are instant when I start playing a game. Videogame cover art appears automatically when a game is playing, which is a nice touch.

<figure class="figure figure--25">
 <img src="/assets/images/integrations/xboxone-ha.gif" alt="Small picture of a kitten" />
 <figcaption>
 <b>Home Assistant: Difficult</b><br>Can be hard to install.
 </figcaption>
</figure>

<figure class="figure figure--25">
 <img src="/assets/images/integrations/amazon-echo.jpg" alt="Small picture of a kitten" style="width: 100%" />
 <figcaption>
 <b>Voice: Great</b><br>Alexa works,  Google Assistant is coming.
 </figcaption>
</figure>

<figure class="figure figure--25">
 <img src="/assets/images/integrations/na.png" alt="Small picture of a kitten" style="width: 100%; height: 100%" />
 <figcaption>
 <b>SmartThings: None</b><br> Integration does not exist.
 </figcaption>
</figure>

<figure class="figure figure--25">
 <img src="/assets/images/integrations/xboxone-app.png" alt="Small picture of a kitten" style="width: 100%" />
 <figcaption>
 <b>Native App: Average</b><br>Basic controls, no context.
 </figcaption>
</figure>


## Sony Playstation 4

 ![](\assets\images\product-photo\playstation4.png){:.image--xl.align-left}

As of Home Assistant 0.89, the Playstation 4 is supported with the same features as the XboxOne add-on. It is even easier to authenticate using the new Home Assistant integration process, which makes this an easy recommendation if you already have a PS4. Most of the popular streaming video apps are available on PS4--even  Plex! Remotely powering on the PS4 now works, so you can now use voice control for that. I’m happy that more people can use this integration and show off the game playing, and design lighting automations based on the PS4’s state.

### Installation and Smart Home Integration

I haven’t had any authentication issues with the Playstation 4 add-on like I did with the Xbox One. With the new component added to Home Assistant 0.89, installation is a breeze compared to the old method. For reference, here is the tutorial from Home Assistant user @cheynespc for directions to install the old Playstation 4 Hass.io add-on.

Video game cover art works on some but not all games. 

<figure class="figure figure--25">
 <img src="/assets/images/integrations/playstation4-ha.gif" alt="Small picture of a kitten" />
 <figcaption>
 <b>Home Assistant: Difficult</b><br>Easier to install than before, though requires using PS4 mobile app.
 </figcaption>
</figure>

<figure class="figure figure--25">
 <img src="/assets/images/integrations/google-home.png" alt="Small picture of a kitten" style="width: 100%" />
 <figcaption>
 <b>Voice: Average</b><br> Works through PS4>>HA>>Google Assistant. Basic commands work.
 </figcaption>
</figure>

<figure class="figure figure--25">
 <img src="/assets/images/integrations/na.png" alt="Small picture of a kitten" style="width: 100%; height: 100%" />
 <figcaption>
 <b>SmartThings: None</b><br> Integration does not exist.
 </figcaption>
</figure>

<figure class="figure figure--25">
 <img src="/assets/images/integrations/playstation4-app.png" alt="Small picture of a kitten" style="width: 100%" />
 <figcaption>
 <b>Native App: Average</b><br>Basic controls, no context.
 </figcaption>
</figure>

## Nintendo Switch

 ![](\assets\images\product-photo\nintendo-switch.jpg){:.image--xl.align-left}

No integration exists for the Nintendo Switch and it’s not likely to happen in the future. If you need a method to detect if the Switch is connected to the dock, I would connect a LAN adapter to the the Switch dock and Home Assistant’s **``nmap device tracker``** to detect the LAN adapter’s presence. If the Switch uses a dedicated HDMI port and your TV and/or AV receiver is connected to Home Assistant, then create an automation that detects if that HDMI port is currently selected.


# AV Receivers

<figure style="width: 100%;" >
 <img src="\assets\images\overlay\av-receiver.jpg" alt="" />
 <figcaption>
<b>Image:</b>  <a href="https://denon.jp">Denon.jp</a>
 </figcaption>
</figure>


**Competitors in this space:** Onkyo, Pioneer, Sony, Denon, Yamaha, Marantz

I’ve personally tested the following:

|---
| ![](\assets\images\logo\pioneer.png){:.image--md} |  ![](\assets\images\logo\onkyo.png){:.image--md} 
|:-:|:-:
| **VSX-1131 (2016)** | **Onkyo TX-NR509 (2011)** 

### What you need to know

These days, most people don’t own AV receivers and the massive speakers that accompany them. They are bulky and tend to dominate the living room space, so I usually recommend customers invest in a good sound bar for home theater quality sound. If you still want or already have a receiver, you might as well integrate it with the rest of the smart home. Luckily, the latest AV receivers are easy to integrate into Home Assistant!

There aren’t many AV receiver brands out there, which is good because it’s easier to add support to Home Assistant for the few remaining receivers out there. There is a compatibility list for some integrations, like Denon, but the only way to find out if a specific model works is to try it yourself. 

{:.info}
If the AV receiver doesn’t have network capabilities, then a universal remote like the Logitech Harmony can achieve some integration, but lacks features like state awareness (i.e. knowing if a device is on or off).

Voice control is possible if you set up the Home Assistant Cloud with Google Assistant or Alexa, but that shouldn’t be necessary as powering on and changing AV receiver inputs should be handled automatically through **``HDMI-CEC``** and **``ARC``**.

A friend recently asked for AV receiver recommendations, which made me realize how easy it is to buy the wrong AV receiver. From my experience, there are several considerations before buying an AV receiver and HDMI cables:

### Considerations before buying an AV receiver

> - **The receiver should have at least FOUR HDCP 2.2 ports,** which is necessary for 4K video. Not all HDMI ports on the receiver are HDCP 2.2. compatible, even the expensive receivers.
> - **The receiver and TV should support HDMI ARC (Audio Return Channel) or eARC**, which allows the TV to send audio to the soundbar or AV receiver with a single HDMI cable. This is important if you use the TV’s smart apps and want surround sound. 
> - **The receiver and TV should support HDMI-CEC**, also called: Samsung Anynet+, LG  SimpLink, and Sony Bravia Sync. CEC lets devices control the TV and AV receiver inputs automatically. It also allows the TV to automatically turn on the AV receiver.
> - **HDMI cables must be rated at 18gbps to support 4K resolution at 60 frames-per-second.** 10gbps is not 4K. In-wall cables should be rated as CL2 to CL3. It’s a safety thing.
> - Check the Home Assistant [Component page](https://www.home-assistant.io/components/) to see if your brand AVR is supported.

### What you get with a network-enabled AV receiver

> - Get rid of remotes since HDMI ARC, CEC can turn on the TV and change inputs for you.
> - Universal remote control of the media center in Home Assistant.
> - More specific automations (if Chromecast Audio is playing, then turn on the receiver).

### Recommended Reading

> - HDMI CEC, ARC, and eARC Explained 
> - Home Assistant Onkyo Component


## Onkyo Receivers
![](\assets\images\product-photo\onkyo.png){:.image--xl.align-left}

My 2011 Onkyo TX-NR509 receiver is an ancient relic, but surprisingly, it is fully compatible with Home Assistant. Thanks to those folks who reverse-engineered Onkyo’s API, the receiver correctly reports the power and input state instantly in Home Assistant, and I can remotely turn on change inputs within the UI. Installation is a breeze—find the receiver’s IP address and you’re basically done.

#### Installation and Smart Home Integration
In the AV receiver settings, turn off any power saving mode, and enable network standby option. This is necessary for Home Assistant to remotely turn on the receiver.

<figure class="figure figure--25">
 <img src="/assets/images/integrations/onkyo-ha.png" alt="Small picture of a kitten" />
 <figcaption>
 <b>Home Assistant: Great</b><br>Easy to setup. Instant status, full media control. 
 </figcaption>
</figure>

<figure class="figure figure--25">
 <img src="/assets/images/integrations/google-home.png" alt="Small picture of a kitten" style="width: 100%" />
 <figcaption>
 <b>Voice: Average</b><br> Works through Onkyo>>HA>>Google Assistant. Basic commands work.
 </figcaption>
</figure>

<figure class="figure figure--25">
 <img src="/assets/images/integrations/na.png" alt="Small picture of a kitten" style="width: 100%; height: 100%" />
 <figcaption>
 <b>SmartThings: None</b><br> Integration does not exist.
 </figcaption>
</figure>

<figure class="figure figure--25">
 <img src="/assets/images/integrations/playstation4-app.png" alt="Small picture of a kitten" style="width: 100%" />
 <figcaption>
 <b>Native App: Average</b><br>Basic controls, no context.
 </figcaption>
</figure>


## Pioneer
![](\assets\images\product-photo\pioneer.png){:.image--xl.align-left}

As of 2014, Pioneer and Onkyo are effectively the same company! I tested the 2016 Pioneer VSX-1131 receiver and found out that it uses the **``Onkyo Component``** in Home Assistant, and thus provides full media control and responds instantly~. Another plus is that the receiver can be powered on over Wi-Fi, which is not always true for every receiver. 

### Installation and Smart Home Integration
In the AV receiver settings, turn off any power saving mode, and enable network standby option. This is necessary for Home Assistant to remotely turn on the receiver.



# Media Streaming Devices

![](\assets\images\overlay\media-streaming.jpg)

** Published on xx/xx/2019**

**Competitors in this space:** Google Chromecast, Amazon Fire TV, Roku, Apple TV, Android TV

I’ve personally tested the following:

|---
| ![](\assets\images\logo\chromecast.png){:.image--lg} |  ![](\assets\images\logo\roku.png){:.image--md} | ![](\assets\images\logo\amazon.png){:.image--sm} | ![](\assets\images\logo\apple.png){:.image--sm}
|:-:|:-:|:-:|:-:
| **Chromecast Ultra <br> Chromecast (1080p)<br>Chromecast (720p)** | **Roku Streaming Stick+<br> Roku Premiere** | **Amazon Fire TV 2 (2016)<br>Fire TV Stick (2014)** | **Apple TV 2**

### What you need to know
The new lineup of media streaming devices continues to impress every year. With more features like 4K, voice control, and HDR added into physically smaller devices, I feel like I can constantly upgrade my old TV at a cheap price. Indeed, my 2015 Vizio TV is more useful with a Roku Streaming Stick+ so I no longer have to browse through a slow, ancient web interface. 

{:.info}
Though media streaming devices are capable of impressive feats, I’ve found that the best TV watching experience lies with a high-end smart TV like the LG OLED series.  The gyroscopic remote controls make it as easy as possible for anyone to pick up a remote and intuitively browse through the TV’s wide selection of apps. The LG OLED TVs are really impressive, if you can afford it. See my TV Section to learn more.

### Considerations before buying a media streaming device

> - **A media streaming device may not be necessary** if your TV or video game console supports the same video apps.
> - **Companies sell 1080p and 4K versions of their products.** I recommend future-proofing by purchasing the 4K version.
> - **Beware: When you use a media streaming device or service, your TV viewing data is being collected.** There’s a reason why these devices are so cheap: the companies are collecting data on the videos you watch, and possibly selling the information to third parties, like advertisers.

### What you get with a media streaming device

> - Upgrade an outdated TV with new features like voice control, and a faster browsing experience.
> - Remotely switch HDMI ports using emulated Roku feature on Home Assistant
> - Integrated smart home automations, as nearly all devices are supported by Home Assistant
> - Move devices to different TVs.

### Recommended reading

> - The Wirecutter’s Best Streaming Device Recommendation

## Roku
![](\assets\images\product-photo\roku-ultra.png){:.image--lg.align-left}

I recently switched over to the Roku Streaming Stick+, and agree with the Wirecutter that it is the best media streaming device available today. It supports both Google Assistant and Amazon Alexa, as well as Youtube TV and Amazon Prime Video—all without any workarounds. Normally when you try to be a jack of all trades, you end up being good at nothing. In this case, Roku ends up being good enough for my needs, and I haven’t found anything missing besides deeper integration with voice assistants. I just hope Google and Amazon don’t take away their respective apps from Roku and create more segregated market.

I find the Roku voice search function on the remote is much more useful with the ability to search for a title through multiple apps. I never purchase TV shows or movies, so I like Roku’s search function because it highlights the free or subscription options first. Google Assistant and Alexa are officially supported, though it is limited to opening apps, powering on TV or changing volume. Voice commands aren’t as deeply integrated at the application level, compared to the Fire TV or even the Chromecast.

On the premium Roku products like the **``Streaming Stick+``**, the remote includes extra nifty features like TV power and volume control buttons. This also works in tangent with HDMI ARC to control the AV receiver or soundbar volume. With this, I’m able to dump my old TV remote. Though it lacks an Input Change button, I have HDMI-CEC working so rarely do I need it.

### The Problems
The casting feature on Roku is supported on some apps, but not as many as Chromecast. I did a quick test and found that casting works on Netflix, Youtube, Youtube TV, but not Hulu or Plex. It seems like a weird oversight as Roku can easily cast videos as Chromecast. There are times when I miss the casting to Chromecast. So I decided—why not use both? As both devices support HDMI-CEC, I don’t have to worry about switching TV inputs. Though if I’m paying for two devices, I should consider purchasing an Android TV like the Nvidia Shield TV.

### Installation and Smart Home Integration
Roku is easily detected and automatically integrated with Home Assistant as a media player and remote. It offers full media controls, shows state information—like the currently playing app—but also has standard remote functions so you can create a Roku remote card like @iantrich. 

The Roku media player integration is sufficient for lighting automations, though I wish it could detect whether a video is playing or paused. Home Assistant can only detect whether you opened an app on the Roku. The media player status takes 2-3 seconds to update in Home Assistant.

<figure class="figure figure--25">
 <img src="/assets/images/integrations/roku-ha.png" alt="Small picture of a kitten" />
 <figcaption>
 <b>Home Assistant: Great</b><br>Automatically detected in HA..
 </figcaption>
</figure>

<figure class="figure figure--25">
 <img src="/assets/images/integrations/google-home.png" alt="Small picture of a kitten" style="width: 100%" />
 <figcaption>
 <b>Voice: Average</b><br> Works,but no deep integration with apps like Youtube TV
 </figcaption>
</figure>

<figure class="figure figure--25">
 <img src="/assets/images/integrations/roku-app-01.jpg" alt="Small picture of a kitten" style="width: 100%; height: 100%" />
 <figcaption>
 <b>SmartThings: None</b><br> Integration does not exist.
 </figcaption>
</figure>

<figure class="figure figure--25">
 <img src="/assets/images/integrations/roku-app-02.jpg" alt="Small picture of a kitten" style="width: 100%" />
 <figcaption>
 <b>Native App: Great</b><br>Standard controls, browse videos, and listen to TV audio through phone’s headphone jack.
 </figcaption>
</figure>


## Chromecast
![](\assets\images\product-photo\chromecast.jpg){:.image--lg.align-left}

Even though I use Chromecast in my home, I find it difficult to recommend as the sole media device in your home because it lacks a TV user interface and remote. I believe most people want a remote to browse videos, so I recommend trying a Roku, Android TV, or both Roku and Chromecast for these features. My roommates prefer to ignore the Chromecast altogether for the lack of a remote.

I initially liked the Chromecast because it would show video thumbnails on Home Assistant when watching Hulu and Youtube. I thought this feature worked on all apps, but further testing shows the feature doesn’t work on Netflix, Plex, or anything else. Casting from a web browser works, unlike my experiences with Miracast. 

<figure style="width: 100%;" >
 <img src="\assets\images\other\google-media-integration.png" alt="" />
 <figcaption>
Available services that integrate with Chromecast. Youtube and Youtube TV (not listed) also work.
 </figcaption>
</figure>

Though Chromecast is supported by a crazy amount of apps, the Google Assistant integration with Chromecast is severely lacking. 

### Installation and Smart Home Integration

Out of all the devices I tested, Chromecast has the best integration with Home Assistant. Status updates are instant, and episode thumbnails show when using Youtube and Hulu--though not for any other app. Home Assistant can also detect pause/play, which the Roku and Amazon Fire TV cannot do. It's not a deal breaker in any way, but I got a kick ~out of it when the lights turned on after pausing the movie.

Voice control on Chromecast is only useful for the deeper integration with Youtube TV, Netflix, HBO, Starz, and Viki, but not available on Hulu, Prime Video, Dramafever, or Vudu.

<figure class="figure figure--25">
 <img src="/assets/images/other/chromecast-ha.gif" alt="Small picture of a kitten" />
 <figcaption>
 <b>Home Assistant: Great</b><br>Easy to setup. Instant status, full media control. Thumbnails only work on Hulu and Youtube.
 </figcaption>
</figure>

<figure class="figure figure--25">
 <img src="/assets/images/integrations/google-home.png" alt="Small picture of a kitten" style="width: 100%" />
 <figcaption>
 <b>Voice: Average</b><br> Only a few apps support deep voice integration.
 </figcaption>
</figure>

<figure class="figure figure--25">
 <img src="/assets/images/integrations/na.png" alt="Small picture of a kitten" style="width: 100%; height: 100%" />
 <figcaption>
 <b>SmartThings: None</b><br> Integration does not exist.
 </figcaption>
</figure>

<figure class="figure figure--25">
 <img src="/assets/images/integrations/chromecast-tv-app.png" alt="Small picture of a kitten" style="width: 100%" />
 <figcaption>
 <b>Native App: Average</b><br>Basic controls, no context.
 </figcaption>
</figure>




## Amazon Fire TV

![](\assets\images\product-photo\amazon-firetv.jpg){:.image--lg.align-left}

If you’re using Amazon Echo and Alexa, then the Amazon Fire 4K TV sticks are hard to pass up for its low price, but the lack of Youtube support makes this a non-contender. Voice control is impressive, supporting Hulu and some other network TV apps — why can’t Chromecast support Hulu as well?

### Installation and Smart Home Integration
Fire TVs are moderately difficult to setup in Home Assistant, requiring install of ADB and using command-line interface. Home Assistant integration is sufficient for lighting automations, though I wish it could detect whether a video is playing or paused — it only detects whether an app is opened. Player status takes 5 to 10 seconds to update in Home Assistant. There are also slight delays when sending pause/play commands from Home Assistant. Keep in mind, I tested a first generation Amazon Fire TV stick, which is the slowest Fire TV device.





