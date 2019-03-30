---
layout: article
title: Smart Bulbs
short_title: Smart Bulbs
excerpt: something something smart bulbs
category: [lighting, home automation]
permalink: /lighting/smart-bulb
key: lighting-smart_bulb
aside:
  toc: true
banner: assets/images/overlay/smart-bulb.jpg
mode: immersive
header:
  theme: dark
article_header:
  type: overlay
  theme: dark
  background_color: '#203028'
  background_image:
    gradient: 'linear-gradient(135deg, rgba(34, 139, 87 , .4), rgba(139, 34, 139, .4))'
    src: /assets/images/overlay/smart-bulb.jpg
---

<!--more-->

**Competitors in this space:** Philips Hue, Ikea Tradfri, Xiaomi, Sengled, Sylvania, TP-Link, Lifx, Eufy

##### *I’ve personally tested the following:*

|---
| ![](\assets\images\logo\philips-hue.png){:.image--sm} |  ![](\assets\images\logo\sengled.png){:.image--md} | ![](\assets\images\logo\tplink.png){:.image--lg} | ![](\assets\images\logo\osram.png){:.image--sm}
|:-:|:-:|:-:|:-:
| **White A19 60W** | **Element Classic A19 White**<br>**Element Classic BR30 White** | **Wifi Color (LB230)** | **Full Color (A19C)**<br>**Full Color (BR30C)**


## What you need to know
For me, smart bulbs was the only way I could start experimenting with smart homes. I was renting at the time and couldn’t make any house modifications, so I bought a smart bulb, a Wi-Fi outlet, and a Google Home speaker to satisfy that itch. What I didn’t realize was that I couldn’t use the light switch and smart bulb at the same time, since the switch cuts off power to the bulb. It was awkward telling my roommates they could no longer use the light switch, but once my lighting automations became reliable, there was no need to use the switch anymore. 

I’m still a renter, so I use smart bulbs around the house. Smart bulbs remain a cheaper, portable lighting solution compared to smart switches. I can mitigate most of the issues with smart bulbs and live with the rest. 

### Smart Bulbs Acting As Zigbee Repeaters

 I have not personally verified this information but some smart bulbs can act as Zigbee network repeaters, though it varies by brand. Philips Hue bulbs repeat for Hue bulbs only. Sengled bulbs are not repeaters, but the rest are, I think. It goes without saying that if the smart bulb’s power is shut off by a light switch, it no longer functions as a repeater.

### Considerations before buying a smart bulb

> - Smart bulb won’t respond if its power is cut off by the light switch.
> - Most smart bulbs on sale are Zigbee or Wifi. I’ve never seen an Z-Wave bulb on sale.

### What you get with a smart bulb

> - Light bulbs that can be controlled by automations.
> - Colored lighting. I haven’t found a good use case for it, unless you’re throwing colorful parties.
> - Some smart bulbs can act as zigbee network repeaters, though not many other devices besides light bulbs use zigbee.

### Recommended Reading
> - ?


## Philips Hue
![Photo](\assets\images\product-photo\philips-hue.png){:.image--lg.align-left}

**If you don’t mind using adding yet another hub to the network and paying a slight premium, then the Philips Hue series offers consistently high quality smart bulbs that are always available on the market.** Those on a budget don’t need to go with Philips Hue, but it’ll take more research to get a high quality bulb like Philips Hue.  I’ve tried other smart bulbs that range from average to just as good as Philips Hue, but some are no longer available on the market. I recommend these because I know they are good and available on Amazon.

The Philips Hue bulbs pair well with the Hue lightstrips that make up my media center lighting. Watching the living room lights fade out as the TV lightstrips brightens is a very cool transition that easily impresses folks. If you’re not particular about the fade effect or color accuracy, then any cheap Zigbee bulb under $10 should work for you.

<div>{%- include extensions/youtube.html id='39FGJ40vfHs' -%}</div>


### The Problems
Philips Hue bulbs require the Hue bridge because it uses a different profile of Zigbee—called ZLL—that is not compatible with the Zigbee ZHA bulbs on the market. So you can’t normally pair Hue bulbs to SmartThings (though not impossible, see next section). You also don’t get the benefits of repeaters in your network if you’re mix and matching Hue with other Zigbee bulbs. Hue bulbs act as repeaters for Hue lights only and most Zigbee bulbs act as repeaters except for a few brands like Sengled.

### Using Hue bulbs without the Hue Bridge

It’s possible to flash Hue bulbs to standard Zigbee ZHA bulbs using a Python script called **``Hue Thief``**, but I don’t recommend it because of the difficulty in getting it to work and factory resetting bulbs. For starters, the process requires purchasing a Zigbee USB radio, like the **``GoControl HUSBZB-1``**, which is redundant if you already have a SmartThings or Hubitat device. Following my tutorial may not work for everyone, as indicated on the forum.

I’ve had issues with flashed Hue lights unpairing from my network and I haven’t found a solution yet, because there isn’t a normal way for the Hue light to enter exclusion mode! I hear it’s possible to factory reset Hue Thief bubs using a **Philips dimmer remote**, as described here. This seems like a better alternative but I didn’t want to spend another $25 to find out.

### Installation and Smart Home Integration

Compatibility is not an issue as Philips Hue supports nearly every home automation hub out there. SmartThings, Home Assistant, Hubitat, Alexa, Google Assistant—they are all officially supported. Another plus is that the hub is controllable on the local network, so Home Assistant can control the Hue lights without an internet connection. That is either very forward thinking or lazy of Philips to provide that option. 

<figure class="figure figure--50">
 <img src="/assets/images/integrations/phlips-hue-ha.png" alt="Small picture of a kitten" />
 <figcaption>
 <b>Home Assistant: Great</b><br> Press a button on the Hue hub to pair with HA. Super easy. 
 </figcaption>
</figure>

<figure class="figure figure--50">
 <img src="/assets/images/integrations/google-home.png" alt="Small picture of a kitten" style="width: 100%" />
 <figcaption>
 <b>Voice: Great</b><br>Connect Hue to either SmartThings, Google Home or Alexa for voice control.
 </figcaption>
</figure>

<figure class="figure figure--50">
 <img src="/assets/images/integrations/philips-hue-na.png" alt="Small picture of a kitten" style="width: 100%; height: 100%" />
 <figcaption>
 <b>SmartThings: Great</b><br> A non-dimmable switch looks like this.
 </figcaption>
</figure>

<figure class="figure figure--50">
 <img src="/assets/images/integrations/philips-hue-app.png" alt="Small picture of a kitten" style="width: 100%" />
 <figcaption>
 <b>Native App: Great</b><br>It's an LG remote on your phone!
 </figcaption>
</figure>


## The Competition
### TP-Link LB230 Kasa Wifi 

![](\assets\images\product-photo\kasa.jpg){:.image--md.align-left}

**While the TP-Link Kasa LB230 Wifi bulbs are quite good--they respond quickly and are compatible with Home Assistant and Google Assistant--I still don’t recommend buying Wi-Fi bulbs due to potential compatibility and security issues.**  SmartThings integration using a custom device handler is dependent on an internet connection to TP-Link servers, which can go offline in the future. The Kasa app is also insecure according to this study, so I would expect the bulb (which is on your personal network) has potential vulnerabilities too. If TP-Link were to go offline, only Home Assistant would be able to use the bulbs via local communication.   

### Sylvania Lightify

![](\assets\images\product-photo\osram.jpg){:.image--md.align-left}

**The Sylvania Osram Lightify Bulbs are the perfect smart bulbs for your home automation hub--I would buy more of these if they were still available.** They are Zigbee bulbs and pair with SmartThings easily, responds instantly and has the fade effect like Hue bulbs. During the last sale, the colored bulbs could be found for $10-15, which is the lowest price for colored bulbs I have ever seen. The only reason I would not buy this is if the Zigbee network is unreliable in your home.

### Sengled Element Classic

![](\assets\images\product-photo\sengled.jpg){:.image--md.align-left}

**At $7 each, the Sengled Element Classic bulbs (BR30 and A19 sizes) are the cheapest functioning smart bulbs I could find, though it lacks nice-to-have features like the fade effect.** Though that is not a big deal if you plan on sticking these lights in the garage or some unnoticeable place.  These bulbs are Zigbee and I haven't had any problems with pairing or disconnections, so at least they are reliable. I miss the Hue fade effect though, and would gladly pay a few more dollars for a nicer bulb than the Sengled Element. 