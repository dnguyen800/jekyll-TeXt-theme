---
layout: article
title: Garage Door Opener
category: gadgets
---
## Garage Door Opener
**Published on: xx/xx/2019**
![Image: myq.com](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1551204735526_garage_door-front__page.png)

**Competitors in this space: **Chamberlain/Liftmaster MyQ, Aladdin Genie, Linear GoControl, Gogogate, Garagemate

I personally tested the following:

- Chamberlain MyQ Smart Garage Door Opener/Hub (MYQ-G0301)
- Chamberlain MyQ Internet Gateway Garage Door Opener (CIGBU-P)

### Overview
A smart garage door opener is a useful gadget that adds convenience, additional security, and in some cases, saves money. There is less of a chance that you accidentally leave the door open, as the mobile app will alert if that happens. There is a lot of testing involved on your end to make sure the automations work as expected and don’t accidentally open up the door at midnight.

Besides helping with forgetfulness, there are other useful ways to use a connected garage door and a phone. For starters, your phone becomes a garage remote. Going for a neighborhood jog no longer requires bringing along a set of keys since you have your phone with you. It is very convenient to have a smart garage opener, though it also exposes your home to additional risks.

#### Security
Before getting into details of garage door automations, it is important to emphasize security and potential exposures when adding a smart garage opener. You are adding an Internet-dependent device (unless you use a local Z-Wave controller) that can remotely open a door to your home. It’s possible that a company IT admin abuses privileges and accesses your account. A hacker could be monitoring your communications or exploiting vulnerabilities found in the garage opener to gain physical access to your home.  Anything is possible, so that is why it is good to have preventative and detective measures in place to reduce these risks. Segregating network devices using VLANs, remove old or unnecessary devices from the network, disable router settings like UPNP, and updating device firmware are some practices I suggest, though it’s better to do your own research as best practices and threats continue to change.

When designing automations using garage openers and presence sensors, I recommend to keep it simple and use app notifications instead of automatically opening and closing the door without intervention. Presence sensors are not always timely, meaning it could take several minutes before noticing you are away and closes the garage. Sometimes it only takes a few minutes for someone to take break into your home.

#### Considerations before buying a smart garage opener

- Consider the security risks added to the benefits gained. Is it worth it?
- Check for garage door compatibility. Chamberlain and Liftmaster work with MyQ. Genie works with the Aladdin device; other garage doors can use GoControl Z-Wave Opener or Garagemate.

#### What you get with a smart garage opener

- No need to buy extra garage remotes.
- Give and revoke access to household members easily through the MyQ app.
- Setup voice and mobile notifications if the garage is open for a period of time, while away, etc.
- Use Google Assistant to open the garage door.
- Open/close garage from any car, as long as you have your phone handy.
- Lock yourself out but have your phone on you? Open the garage!

### Chamberlain MyQ
![](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1551204678543_myq_logo.png)
![](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1551204690679_garage_door-myq-photo.jpg)

**With few reliable options to choose from, the MyQ Smart Garage Hub is your best option if you have a compatible Chamberlain or Liftmaster garage.**  MyQ doesn’t earn my full recommendation because of their nickel-and-dime practices of charging money for basic features like voice assistant. Other than that, the MyQ hub and mobile app works as expected and is easy to install. MyQ is a Chamberlain product, so it works with the majority of Chamberlain and Liftmaster garages commonly found in the U.S.

#### The Problems
MyQ relies on an internet connection to work, which opens up additional security risks. The official integration of MyQ with services like IFTTT, Alexa and Google Assistant require a $5/month subscription to MyQ. I use unofficial integrations as a loophole to the fee, but it could stop working at any time.

#### Installation and Smart Home Integration
The MyQ app guides you through the physical and software installation of the hub.  Place the MyQ hub near the garage opener, press the ‘learn’ button on the garage opener, and then following instructions on MyQ app.

Unofficial integrations with SmartThings and Home Assistant exist, but could stop working if MyQ changes how it handles communications. For SmartThings, a custom device handler an additional tilt sensor is needed to work properly. For Home Assistant, you only need to enter your credentials for access (which is slightly concerning).  It works with voice assistants that are paired with SmartThings and Home Assistant. 


![Voice Pair MyQ with Smartthings or Home Assistant, which is connected to your voice assistant.](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1543622841706_google_assistant.jpg)
![Home Assistant: Unofficial Integration As easy as typing in your username and password!](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1551203688672_garag_door-myq-ha.png)

![SmartThings: Device Handler needed Requires setup of ST device handler, but works fine after that.](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1551203220908_garage_door-myq-smartthings.png)
![MyQ App Straightforward to use. Setup notifications easily. Cannot share access with others unless you share your account.](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1551203209897_garage_door-myq-app.png)


