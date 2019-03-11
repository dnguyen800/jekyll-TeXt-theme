---
layout: article
title: Smart Bulbs
category: lighting
---
## Smart Bulbs
**Published on: xx/xx/2019**
<pic of a smart bulb>

**Competitors in this space: ** Philips Hue, Ikea Tradfri, Xiaomi, Sengled, Sylvania, TP-Link, Lifx, Eufy

I’ve personally tested the following:

- Philips Hue White A19 4-Pack 60W Equivalent Dimmable LED Smart Bulb
- Sengled Element Classic A19 White bulb
- Sengled Element Classic BR30 White bulb
- TP-Link Kasa Wifi Color Bulb (LB230)
- SYLVANIA LIGHTIFY Full Color A19 light bulb A19C)
- SYLVANIA LIGHTIFY Full Color BR30 light bulbs (BR30C) 

### Overview
For me, smart bulbs was the only way I could start experimenting with smart homes. I was renting at the time and couldn’t make any house modifications, so I bought a smart bulb, a Wi-Fi outlet, and a Google Home speaker to satisfy that itch. What I didn’t realize was that I couldn’t use the light switch and smart bulb at the same time, since the switch cuts off power to the bulb. It was awkward telling my roommates they could no longer use the light switch, but once my lighting automations became reliable, there was no need to use the switch anymore. 

I’m still a renter, so I use smart bulbs around the house. Smart bulbs remain a cheaper, portable lighting solution compared to smart switches. I can mitigate most of the issues with smart bulbs and live with the rest. 

#### Smart Bulbs Acting As Zigbee Repeaters
 I have not personally verified this information but some smart bulbs can act as Zigbee network repeaters, though it varies by brand. Philips Hue bulbs repeat for Hue bulbs only. Sengled bulbs are not repeaters, but the rest are, I think. It goes without saying that if the smart bulb’s power is shut off by a light switch, it no longer functions as a repeater.

#### Things to consider before buying a smart bulb

- Smart bulb won’t respond if its power is cut off by the light switch.
- Most smart bulbs on sale are Zigbee or Wifi. I’ve never seen an Z-Wave bulb on sale.

#### What you get with a smart bulb

- Light bulbs that can be controlled by automations.
- Colored lighting. I haven’t found a good use case for it, unless you’re throwing colorful parties.
- Some smart bulbs can act as zigbee network repeaters, though not many other devices besides light bulbs use zigbee.


### Philips Hue Bulbs

![](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1550950373943_Philips_hue_logo.png)
![](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1550950490439_smart_bulb-philips_hue-photo.png)


**If you don’t mind using adding yet another hub to the network and paying a slight premium, then the Philips Hue series offers consistently high quality smart bulbs that are always available on the market.** Those on a budget don’t need to go with Philips Hue, but it’ll take more research to get a high quality bulb like Philips Hue.  I’ve tried other smart bulbs that range from average to just as good as Philips Hue, but some are no longer available on the market. I recommend these because I know they are good and available on Amazon.

The Philips Hue bulbs pair well with the Hue lightstrips that make up my media center lighting. Watching the living room lights fade out as the TV lightstrips brightens is a very cool transition that easily impresses folks. If you’re not particular about the fade effect or color accuracy, then any cheap Zigbee bulb under $10 should work for you.


https://www.youtube.com/watch?v=39FGJ40vfHs


#### The Problems
Philips Hue bulbs require the Hue bridge because it uses a different profile of Zigbee—called ZLL—that is not compatible with the Zigbee ZHA bulbs on the market. So you can’t normally pair Hue bulbs to SmartThings (though not impossible, see next section). You also don’t get the benefits of repeaters in your network if you’re mix and matching Hue with other Zigbee bulbs. Hue bulbs act as repeaters for Hue lights only and most Zigbee bulbs act as repeaters except for a few brands like Sengled.

#### Using Hue bulbs without the Hue Bridge
It’s possible to flash Hue bulbs to standard Zigbee ZHA bulbs using a Python script called Hue Thief, but I don’t recommend it because of the difficulty in getting it to work and factory resetting bulbs. For starters, the process requires purchasing a Zigbee USB radio, like the GoControl HUSBZB-1, which is redundant if you already have a SmartThings or Hubitat device. Following my tutorial may not work for everyone, as indicated on the forum.

I’ve had issues with flashed Hue lights unpairing from my network and I haven’t found a solution yet, because there isn’t a normal way for the Hue light to enter exclusion mode! I hear it’s possible to factory reset Hue Thief bubs using a Philips dimmer remote, as described here. This seems like a better alternative but I didn’t want to spend another $25 to find out.

#### Installation and Smart Home Integration
Compatibility is not an issue as Philips Hue supports nearly every home automation hub out there. SmartThings, Home Assistant, Hubitat, Alexa, Google Assistant—they are all officially supported. Another plus is that the hub is controllable on the local network, so Home Assistant can control the Hue lights without an internet connection. That is either very forward thinking or lazy of Philips to provide that option. 


![Voice Control Connect Hue service to either SmartThings, Google Home or Alexa for voice control.](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1543622841706_google_assistant.jpg)
![Home Assistant Looks like any paired smart light in HA.](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1550961847931_smart_bulb-philiips_hue-ha.png)

![](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1550961620066_whitespace.png)
![SmartThings (Non-DImmable Switch) A non-dimmable switch looks like this.](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1550961599970_smart_bulb-philips_hue-app.png)
![](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1550961889511_whitespace.png)




### TP-Link LB230 Kasa Wifi Bulb

![](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1550972108428_smart_bulb-kasa-photo.jpg)
![](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1550972355552_whitespace.png)


While the TP-Link Kasa LB230 Wifi bulbs are quite good, I still don’t recommend buying Wi-Fi bulbs due to potential compatibility and security issues.  SmartThings integration using custom device handler is dependent on an internet connection to TP-Link servers, which can go offline in the future. The Kasa app is also using insecure communications according to this study, so I would expect the bulb (which is on your personal network) has potential vulnerabilities too. If TP-Link were to go offline, only Home Assistant would be able to use the bulbs via local communication.   

### Sylvania Lightify Bulb

![](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1550973855180_whitespace.png)
![](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1550973839588_smart_bulb-sylvania-product.jpg)
![](/static/img/pixel.gif)


The Sylvania Osram Lightify Bulbs are the perfect smart bulb for your home automation hub. I would buy more of these if they were still available. It pairs with SmartThings easily, responds instantly and has the fade effect like Hue bulbs. During the last sale, the colored bulbs could be found for $10-15, which is the lowest price for colored bulbs I have ever seen.

### Sengled Element Classic

![](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1550981591656_smart_bulb-sengled-photo.jpg)
![](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1550981600771_whitespace.png)


At $7 each, the Sengled Element Classic bulbs (BR30 and A19 sizes) are cheapest functioning smart bulb I could find, though it lacks nice-to-have features like the fade effect. Not a big deal if you plan on sticking these lights in the garage or an unnoticeable place.  I have not had any problems with pairing or disconnections, so at least they are reliable. I miss the fade effect though, and would gladly pay a few more dollars for a nicer bulb than the Sengled Element. 