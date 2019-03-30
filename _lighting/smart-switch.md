---
layout: article
title: Smart Switches
short_title: Smart Switches
excerpt: something something smart switches
category: [lighting, home automation]
permalink: /lighting/smart-switch
key: lighting-smart_switch
aside:
  toc: true
banner: assets/images/overlay/smart-switch.jpg
mode: immersive
header:
  theme: dark
article_header:
  type: overlay
  theme: dark
  background_color: '#203028'
  background_image:
    gradient: 'linear-gradient(135deg, rgba(34, 139, 87 , .4), rgba(139, 34, 139, .4))'
    src: /assets/images/overlay/smart-switch.jpg
---

<!--more-->

**Competitors in this space:** TP-Link, GoControl, Zooz, GE/Jasco, Leviton, Lutron, Innovelli, Insteon

##### I personally tested the following:

|---
| ![](\assets\images\logo\lutron.png){:.image--lg} |  ![](\assets\images\logo\leviton.png){:.image--lg} 
|:-:|:-:
| **Caseta Wireless Dimmer Switch (PD-6WCL-WH)** | **Decora 600-Watt Z-Wave Dimmer Switch (VB2-DZ6HD)**<br>**Decora Dimmer Remote (DD0SR-DLZ)**<br>**Decora Z-Wave 15A Switch (VB5-DZ15S)**

### What you need to know

Smart light switches are the ideal lighting solution in every home. Replacing one light switch connected to six light bulbs is cheaper than replacing with six smart bulbs. Smart switches function physically like regular switches, with the added benefit of being controlled remotely through voice, app, or an automation.  It’s too bad that I’m a renter, otherwise I would have smart switches everywhere. 

Most wireless light switches use Z-Wave Plus, but some use Wi-Fi or other technology. I wouldn’t use Wi-Fi switches unless I trust that the company will be around in the next ten years. That is why I’m comfortable recommending the Lutron Caseta brand, mainly because the company makes good products and has been around for decades.  

<figure style="width: 65%;" >
 <img src="\assets\images\other\switch-install.jpg" alt="" />
 <figcaption>
This Z-Wave switch was a difficult install—there was literally no room left to squeeze in the switch and the four wires.
 </figcaption>
</figure>

Smart switches, especially Z-Wave switches, are difficult **(and potentially dangerous)** to install for DIYers like me. They are bulky—leaving little room in the already tiny electrical box to fit the switch and its wires. Z-Wave switches also require identification of the line (hot), load, traveler, neutral and ground wires, as each wire must be connected with its designated screw on the switch. A regular single-pole light switch install is much simpler—as long as you connect the line and load wires to any of the two black wires, as well as the ground wire, the switch will work.

<figure class="figure figure--33">
 <img src="/assets/images/other/smart-switch-03.jpg" alt="" style="width: 100%" />
 <figcaption>
Fitting 3 switches and 14 wires in one box was not fun.
 </figcaption>
</figure>
<figure class="figure figure--33">
 <img src="/assets/images/other/smart-switch-02.jpg" alt="" style="width: 100%" />
 <figcaption>
Comparison between a Z-Wave regular light switch.
 </figcaption>
</figure>
<figure class="figure figure--33">
 <img src="/assets/images/other/smart-switch-01.jpg" alt="" style="width: 100%" />
 <figcaption>
The size difference makes it a much more difficult install.
 </figcaption>
</figure>

. In a 3-way switch, the process becomes slightly more complicated as you also need to purchase a separate auxiliary Z-Wave switch and it must replace the switch directly connected to the line (hot). If you replace the light switch connected to load with an auxiliary switch, then you’ve made a mistake.

There is some good news that the upcoming Z-Wave switches are looking easier to install. The upcoming Innovelli switches no longer require a neutral wire, which opens the door for older homes to be outfitted with smart switches. If companies can make a smaller Z-Wave switch and simplify the 3-way switch installation, then Z-Wave switches will finally be a match for Lutron Caseta switches—my current recommendation.

There are more things I haven’t mentioned that can go wrong. It’s not easy, but not impossible as long as you take the time to read instructions, watch tutorials, ask questions and be patient with the install.  My general rule is if I have any uncertainty with any step of the process, then I’m not ready.

{:.warning}
*Installation of smart switches can be the most daunting part of a smart home. If you are unsure if what you’re doing, take the safe route and call an electrician. Don’t risk burning the house down because of your pride. That is why my recommendation is the one to take seriously, as it is one of the safest switch installations you can do.*

### Considerations before buying a smart light switch

> - **Check if your house has neutral wires in each of the electrical boxes.** This is needed for most Z-Wave and Wi-Fi switches. Newer houses are required to have neutral wires installed, but most older houses do not have them.
> - **Identify the 3 or 4-way light switches in your home**, as these may require auxiliary switches (if using Z-Wave).
> - **Decide on using dimmer switches or not.** Dimmer switches require dimmable bulbs.
> - **Identify wall plate sizes to purchase**, unless your house already uses rocker-style switches. 
> - If there is a light switch you rarely use, then don’t replace it with a smart one.

### What you get with a smart light switch

> - Gives you the ability to remotely control lights using voice, app, or automation. 
> - Design automations that control lighting at different brightness levels. I set brightness levels to 10% for any automations that run between midnight and sunrise.
> - Vacation mode lighting. Write an automation that turns the lights on and off to simulate activity.

### Recommended Reading
> - ?

## Lutron Caseta
 ![](\assets\images\product-photo\lutron-caseta.jpg){:.image--lg.align-left}

**For a safe and hassle-free installation, I highly recommend Lutron Caseta switches.** Adding yet another hub to your smart home goes against my advice, but the simplicity of installation, lack of neutral wire requirement, and its overall reliability makes this the only smart switch I can recommend for DIYers to install without professional help. The cost of a starter kit seems high, but know that you can use the included Lutron Pico remote as an auxiliary switch in a 3-way switch, which will keep the price in line with other smart switches.

I was surprised at the number of official integrations are supported by Lutron Caseta. SmartThings, Home Assistant, Google Assistant, and Amazon Alexa can be connected with a few clicks in an app. Even though the Caseta bridge and SmartThings are using internet instead of local communication, I didn’t notice any significant delay when turning on the light. Hubitat is also “supported,” but requires the more expensive Lutron SmartBridge Pro for local communication. I became aware of this recently and had to decide against purchasing Hubitat as I didn’t want to buy yet another $120 to gain nothing meaningful in return. 

### The Problems

The Lutron Caseta bridge needs a wired ethernet connection to your router, though connecting to a wireless network bridge also works. The light switches use Lutron’s proprietary **Clear Connect** wireless control protocol, which have no issues in a 2,000 sq. ft home. I think most homes will be fine using Caseta and a plug-in dimmer (which doubles as a repeater), but I would have doubts using Lutron Caseta in a very large home (4,000 sq ft). 

I’m not a fan of the look of the Caseta switch and Pico remotes. I like the rocker switches that is on the Leviton Decora, but that’s my preference.

### Installation and Smart Home Integration

Out of all the products listed here, light switches are the most difficult to install, except for Lutron Caseta switches--it is as easy as installing a regular light switch. The size of a Caseta switch is only slightly larger than a regular switch. A neutral wire isn’t required to power the switch. There is no need to identify load and line wires (unless it is a 3-way switch) to install. There’s no need to buy auxiliary switches specifically for a 3-way switch configuration either.

For 3-way switches, the recommended installation is to reverse the 3-way wiring back to a single-pole setup and use a Pico remote as the auxiliary switch. On the outside, it functions and looks like a regular light switch.

Connecting Lutron Caseta to SmartThings is easy, but connecting to Home Assistant is a more difficult due to the need to create ~ certificate, but a Hass.io add-on exists to automate this task.

Lutron Caseta works with SmartThings as it is an official integration. Home Assistant requires some works to generate a certificate for authentication, but it’s easy to do now with the Lutron Hass.io add-on. Once this certificate is created, you never have to touch the Lutron configuration again. Any new switches are automatically added in Home Assistant.



<figure class="figure figure--50">
 <img src="/assets/images/integrations/lutron-ha-02.png" alt="Small picture of a kitten" />
 <figcaption>
 <b>Home Assistant: Good</b><br>Need to create certificate during setup.
 </figcaption>
</figure>

<figure class="figure figure--50">
 <img src="/assets/images/integrations/google-home.png" alt="Small picture of a kitten" style="width: 100%" />
 <figcaption>
 <b>Voice: Great</b><br>Pair the TV using the Google Home app.
 </figcaption>
</figure>

<figure class="figure figure--50">
 <img src="/assets/images/integrations/lutron-st.png" alt="" style="width: 100%; height: 100%" />
 <figcaption>
 <b>SmartThings: TBD</b>
 </figcaption>
</figure>

<figure class="figure figure--50">
 <img src="/assets/images/integrations/lutron-app.png" alt="" style="width: 100%" />
 <figcaption>
 <b>Native App: Great</b>
 </figcaption>
</figure>

## Leviton Decora Z-Wave Plus Dimmer Switches

 ![](\assets\images\product-photo\leviton.png){:.image--md.align-left}

When I first started planning my smart home purchases, I was adamant on sticking with Z-Wave devices to create the most optimal robust Z-Wave network. That lead me to the Leviton Decora Z-Wave Plus Dimmer Switches, which I purchased and installed at a friend’s house. **The Leviton Decora Z-Wave switches (DZ6HD) have been performing solid for the past year, but the painful installation process and the neutral wire requirement make it difficult to recommend when there are better options like the Lutron Caseta switches.** If you don’t mind a challenge and your home has a neutral wire, then give these a shot.

Issues with Z-Wave devices are not uncommon from the forums I read, but I’ve had no such problem with the dozen Leviton Decora switches. The switch doubles as a Z-Wave signal repeater, which makes these perfect in a large house (3,000 sq. ft or greater). I also like the rocker-style switch design compared to the Lutron Caseta look. 

### The Problems

The Leviton Decora switch requires a neutral wire to work, so newer or remodeled houses that have these wires are compatible. The bulky size of the switch makes the installation challenging, especially when installing three switches in one box. At the current price on Amazon ($51), I would rather risk trying the upcoming switches from Innovelli or Lutron Caseta, which are a similar price.

### Installation and Smart Home Integration

I remember having minor issues pairing with SmartThings, mainly with getting the device handler by user @jasonxh to load, and getting the SmartThings hub physically close enough to pair the switch.  That effort required using some long network cables to pair the first switches.

I can’t comment on the difficulty of pairing directly with Home Assistant, as I used SmartThings in this particular setup.. After pairing, the switches have been rock solid with no issues whatsoever for over a year.


<figure class="figure figure--50">
 <img src="/assets/images/integrations/leviton-ha.png" alt="Small picture of a kitten" />
 <figcaption>
 <b>Home Assistant: Good</b><br>Several steps to complete on HA and the TV.
 </figcaption>
</figure>

<figure class="figure figure--50">
 <img src="/assets/images/integrations/google-home.png" alt="Small picture of a kitten" style="width: 100%" />
 <figcaption>
 <b>Voice: Great</b><br>Connect the switch to SmartThings and you will get voice control in Alexa or Google.
 </figcaption>
</figure>

<figure class="figure figure--50">
 <img src="/assets/images/integrations/leviton-dimmer-st.png" alt="Small picture of a kitten" style="width: 100%; height: 100%" />
 <figcaption>
 <b>SmartThings: Good</b><br> Using device handler will show a few extra commands.
 </figcaption>
</figure>

<figure class="figure figure--50">
 <img src="/assets/images/integrations/leviton-st.png" alt="Small picture of a kitten" style="width: 100%" />
 <figcaption>
 <b>Native App: Great</b><br>A non-dimmable switch looks like this.
 </figcaption>
</figure>