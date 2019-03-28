---
layout: article
title: Garage Door Openers
short_title: Garage Door
excerpt: If a house had a butt, it would be the garage.
category: [gadgets, home automation]
permalink: /gadgets/garage-door
key: gadgets-garage_door
aside:
  toc: true
banner: assets/images/overlay/garage-door.jpg
mode: immersive
header:
  theme: dark
article_header:
  type: overlay
  theme: dark
  background_color: '#203028'
  background_image:
    gradient: 'linear-gradient(135deg, rgba(34, 139, 87 , .4), rgba(139, 34, 139, .4))'
    src: /assets/images/overlay/garage-door.jpg
---

<!--more-->
<figcaption><b>Image:</b><a href="https://unsplash.com/@ralphkelly"> Ralph Kelly via unsplash.com</a></figcaption>

**Competitors in this space:** Chamberlain/Liftmaster MyQ, Aladdin Genie, Linear GoControl, Gogogate, Garagemate

I personally tested the following:

|---
| ![](\assets\images\logo\chamberlain.png){:.image--xl}
|:-:
| **MyQ Smart Garage Door Opener/Hub (MYQ-G0301)**<br>**MyQ Internet Gateway Garage Door Opener (CIGBU-P)**


### What you need to know
A smart garage door opener is a useful gadget that adds convenience, additional security, and in some cases, saves money. There is less of a chance that you accidentally leave the door open, as the mobile app will alert if that happens. There is a lot of testing involved on your end to make sure the automations work as expected and don’t accidentally open up the door at midnight.

Besides helping with forgetfulness, there are other useful ways to use a connected garage door and a phone. For starters, your phone becomes a garage remote. Going for a neighborhood jog no longer requires bringing along a set of keys since you have your phone with you. It is very convenient to have a smart garage opener, though it also exposes your home to additional risks.

### Security considerations
Before getting into details of garage door automations, it is important to emphasize security and potential exposures when adding a smart garage opener. You are adding an Internet-dependent device (unless you use a local Z-Wave controller) that can remotely open a door to your home. It’s possible that a company IT admin abuses privileges and accesses your account. Or, a hacker could be monitoring your communications or exploiting vulnerabilities found in the garage opener to gain physical access to your home.  Anything is possible, so that is why it is good to have preventative and detective measures in place to reduce these risks. Segregating network devices using VLANs, remove old or unnecessary devices from the network, disable router settings like UPNP, and updating device firmware are some practices I suggest, though it’s better to do your own research as best practices and threats continue to change.

When designing automations using garage openers and presence sensors, I recommend to keep it simple and use app notifications instead of automatically opening and closing the door without intervention. Presence sensors are not always timely, meaning it could take several minutes before noticing you are away and closes the garage. Sometimes it only takes a few minutes for someone to take break into your home.

### Considerations before buying a smart garage opener

- **Consider the security risks added to the benefits gained.** Is it worth it?
- **Check if your garage door is compatible.** Chamberlain and Liftmaster work with MyQ. Genie works with the Aladdin device; other garage doors can use GoControl Z-Wave Opener or Garagemate.

### What you get with a smart garage opener

- No need to buy extra garage remotes.
- Give and revoke access to household members easily through the MyQ app.
- Setup voice and mobile notifications if the garage is open for a period of time, while away, etc.
- Use Google Assistant to open the garage door.
- Open/close garage from any car, as long as you have your phone handy.
- Lock yourself out but have your phone on you? Open the garage!

## Chamberlain MyQ
 ![](\assets\images\product-photo\myq.jpg){:.image--xl.align-left}

**With few reliable options to choose from, the MyQ Smart Garage Hub is your best option if you have a compatible Chamberlain or Liftmaster garage.**  MyQ doesn’t earn my full recommendation because of their nickel-and-dime practices of charging money for basic features like voice assistant. Other than that, the MyQ hub and mobile app works as expected and is easy to install. MyQ is a Chamberlain product, so it works with the majority of Chamberlain and Liftmaster garages commonly found in the U.S.

### The Problems
MyQ relies on an internet connection to work, which opens up additional security risks. The official integration of MyQ with services like IFTTT, Alexa and Google Assistant require a $5/month subscription to MyQ. I use unofficial integrations as a loophole to the fee, but it could stop working at any time.

### Installation and Smart Home Integration
The MyQ app guides you through the physical and software installation of the hub.  Place the MyQ hub near the garage opener, press the ‘learn’ button on the garage opener, and then following instructions on MyQ app.

Official app recently aded the ability to add members to a home, and give access. Now you don't have to share one account to open the garage.

Unofficial integrations with SmartThings and Home Assistant exist, but could stop working if MyQ changes how it handles communications. For SmartThings, a custom device handler an additional tilt sensor is needed to work properly. For Home Assistant, you only need to enter your credentials for access (which is slightly concerning).  It works with voice assistants that are paired with SmartThings and Home Assistant. 

<figure class="figure figure--50">
 <img src="/assets/images/integrations/myq-ha.png" alt="Small picture of a kitten" />
 <figcaption>
 <b>Home Assistant: Good</b><br> As easy as typing in your username and password! Which is a security concern...
 </figcaption>
</figure>

<figure class="figure figure--50">
 <img src="/assets/images/integrations/google-home.png" alt="Small picture of a kitten" style="width: 100%" />
 <figcaption>
 <b>Voice: Okay</b><br>Pair MyQ with Smartthings. Chamberlain charges if fee if connected directly to Google Assistant.
 </figcaption>
</figure>

<figure class="figure figure--50">
 <img src="/assets/images/integrations/myq-st.png" alt="Small picture of a kitten" style="width: 100%; height: 100%" />
 <figcaption>
 <b>SmartThings: Good</b><br>Device Handler needed Requires setup of ST device handler, but works fine after that.
 </figcaption>
</figure>

<figure class="figure figure--50">
 <img src="/assets/images/integrations/myq-app.png" alt="Small picture of a kitten" style="width: 100%" />
 <figcaption>
 <b>Native App: Good</b><br>Setup notifications easily. Can now share access with other accounts.
 </figcaption>
</figure>
