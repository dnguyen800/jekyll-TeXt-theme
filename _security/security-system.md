---
layout: article
title: Security Systems
short_title: Security Systems
excerpt: Something something security system.
category: [security, home automation]
permalink: /security/security-system
key: security-security_system
aside:
  toc: true
banner: assets/images/overlay/security-system.jpg
mode: immersive
header:
  theme: dark
article_header:
  type: overlay
  theme: dark
  background_color: '#203028'
  background_image:
    gradient: 'linear-gradient(135deg, rgba(34, 139, 87 , .4), rgba(139, 34, 139, .4))'
    src: /assets/images/overlay/security-system.jpg

---

<!--more-->

Image: Simplisafe

**Competitors in this space: **Ring Alarm, Nest Secure, Simplisafe, Abode, alarm.com, Frontpoint Security, ADT

I’ve personally tested the following:

|---
| ![](\assets\images\logo\simplisafe.png){:.image--md} |  ![](\assets\images\logo\smartthings.png){:.image--md} 
|:-:|:-:
| **Simplisafe (latest version)** | **SmartThings (DIY Solution)** 



### What you need to know

Like the cord-cutting revolution with cable TV, the home security system market is entering a new era of affordable security monitoring without contracts. Professional installation isn’t needed with these systems unless you are looking to install wired sensors in the house.

Your security system purchase has an impact on home automation, as there are ways to use the security system’s sensors with your home automation platform to avoid duplicate sensors.  Abode and and Ring offer unofficial integrations with Home Assistant, though your home automation platform may not be the most stable with this setup. So choose wisely!

There are few differentiating features between competitors as all professional security systems have the essential features: a 24-hour battery backup, cellular connection (included with monitoring service), and the “smashsafe” feature (if someone smashes a keypad or hub, you’re alerted).  These features are not available with DIY solutions without a clever homemade solution.

I’ve believe there are three categories I cover that will fit most people’s needs around security. If you are just a little bit serious about protecting your home, then I strongly suggest avoid the DIY route and look into an official provider like Ring.

### Considerations before buying a security system

> - Decide on building a DIY or purchasing a professional security system.
> - Decide if you want to use home security sensor with an unstable home automation platform.

### What you get with a security system

> - In theory, you get more reliable sensors that have been thoroughly tested with the security system.
> - 24/7 security monitoring, costing between $10-25 a month.

### Recommended Reading

> - The Wirecutter’s security system [recommendation](https://thewirecutter.com/reviews/the-best-home-security-system/)
> - Ring admin security [breach](https://gizmodo.com/amazons-ring-security-cameras-may-have-let-employees-sp-1831658669)



## DIY Security System using SmartThings
![](\assets\images\logo\smartthings.png){:.image--xl.align-left}

**You can use your existing SmartThings hub and sensors to create a simple security system with little to no additional investment, but there are several deficiencies that prevent it from being a mostly hands-off experience.**  I used the Smart Home Monitor and SHM Delay SmartApps, along with a few devices (Fire tablet, ActionTiles license, Konnected module, power converter, cables) to get a makeshift system. The amount of work I put into building and testing the system, and the annoyances I’ve yet to fix made me realize the worth of a professional security system like Ring. 

{:.info}
The arming and disarming of a security system can be automated with a presence sensor. Please check out my section on Sensors for more info.


<figure style="width: 100%;" >
 <img src="\assets\images\other\diy-security.jpg" alt="" />
 <figcaption>
I wall-mounted a tablet where the alarm keypad used to be. Easy to do with less risk compared to directly wiring the tablet to a power source.
 </figcaption>
</figure>

Without an automated method to arm and disarm the system, I installed a wall-mounted tablet so I could arm the system before I left the house. I used an old LG  tablet ($35), an ActionTiles license ($25), and some cables and converters ($11) to mount the tablet. 

### The Problems

The **``SHM Delay``** app is critical for a working DIY security system, as the Smart Home Monitor in SmartThings doesn’t have basic features like entry/exit delays (really??). 
I spent days tweaking the **``SHM Delay``** app but still run into false alarms. I’m sure it’s not working correctly due to my mistakes, but the fact that I’m spending hours out of my day  to fix it is enough for me to switch to a professional system.

Once I was able to get a working system in place, I started thinking about the ways the system could fail.  What if the tablet stops responding and I can’t disarm the alarm? What if someone smashes the siren or disconnects SmartThings?  What if SmartThings servers go offline? I eventually realized the harsh truth that these devices aren’t designed to be a security system and don’t have the safeguards to protect my home.  In the end, I disabled the siren and added a camera in the living room. I now rely on my phone for intrusion alerts, which I hope I am awake to respond to it. 

{:.info}
*If your home already has a pre-wired security system, you can use a device called Konnected ($89) to use the wired sensors in home automation hubs like SmartThings. The downside is you’re still stuck with the limitations of a DIY security system that I described.*

### Installation and Smart Home Integration

It's possible to connect the SmartThings security solution and Home Assistant together using MQTT and this [SmartApp](https://ethitter.com/2016/08/smartthings-smart-home-monitor-shm-mqtt-home-assistant/) from user @ethitter.


<figure class="figure figure--25">
 <img src="/assets/images/integrations/diy-security-ha.png" alt="" />
 <figcaption>
  <b>Home Assistant: Good</b><br>Several steps requiring developer account, edit config file, browser authorization.
 </figcaption>
</figure>
<figure class="figure figure--25">
 <img src="/assets/images/integrations/google-home.png" alt="Small picture of a kitten" style="width: 100%" />
 <figcaption>
 <b>Voice: Great</b><br>Spotify works perfectly with Google Assistant.
 </figcaption>
</figure>

<figure class="figure figure--25">
 <img src="/assets/images/integrations/diy-security-st.png" alt="Small picture of a kitten" style="width: 100%" />
 <figcaption>
 <b>SmartThings: None</b><br> Integration does not exist.
 </figcaption>
</figure>
<figure class="figure figure--25">
 <img src="/assets/images/integrations/diy-security-app.png" alt="Small picture of a kitten" style="width: 100%" />
 <figcaption>
 <b>Native App: Okay</b><br>Amazing!
 </figcaption>
</figure>



## Self Installation with Professional Monitoring
### Simplisafe
![](\assets\images\product-photo\simplisafe.jpg){:.image--xl.align-left}

**If you don’t mind having duplicate sensors for home automation and security, then a dedicated security system is the most reliable way to securing your home.** My friend was looking for such a system, so I suggested Simplisafe, based on the [Wirecutter’s recommendation](https://thewirecutter.com/reviews/the-best-home-security-system/). If I were to do it all over again, I’d try out Ring Alarm, but my experience with Simplisafe has been nothing but excellent—besides the expensive monitoring cost.  

Simplisafe offers a security camera which works as described, but isn’t useful without their $25/month monitoring service, as you don’t have access to the mobile app to view the camera feed.  Visual verification is an exclusive feature to Simplisafe that allows the monitoring center to access your camera feed and verify an intrusion, though it maybe not worth the privacy risk, especially after the recent [Ring incident](https://gizmodo.com/amazons-ring-security-cameras-may-have-let-employees-sp-1831658669). The variety of security sensors available is unmatched—you can buy an (really loud 105db) siren, key fob, keypad, panic button, glass break sensor—which aren’t available on Ring yet. 

I haphazardly tested a few features based on what I could reasonably test without setting off police alerts. Upon unplugging the hub, an e-mail alert was sent within seconds—that is insanely fast!  The door sensors have been accurate so far, and the motion sensors are more responsive than the Z-wave ones I use—it even detected motion while I was crawling on the floor. If you don’t want pets to set off the alarm, you can rotate the sensor upside-down so the sensor can only sees straight ahead and towards the ceiling.

### The Problems

Where Simplisafe fails is the high monthly price for critical functions. Yes, it was a dick move to hide access to the mobile app behind the $25/month tier. Simplisafe is trying to increase the value of the tier by including free camera storage, but that is a ploy to purchase their unproven indoor and doorbell cameras.  The price tag stings even more when compared to Ring’s $10/month service, which offers the same 24/7 monitoring, cellular backup, plus free storage of camera footage history.

I also wish someone figured out how to use Simplisafe sensors with Home Assistant. They operate on a proprietary RF frequency and only communicate to the Simplisafe hub, unfortunately.

### Installation and Smart Home Integration
Installation is a breeze as the included sensors are already paired with your system if you purchase a set. The box that holds the sensor has a serial # listed, which will help you identify the sensor in the system and rename it to something more appropriate, like **``Front Door``**.

<figure style="width: 50%;" >
 <img src="\assets\images\other\simplisafe-ha.png" alt="" />
 <figcaption>
Simplisfe HA integration is limited to alarm control panel, which will look something like this.
 </figcaption>
</figure>

Home Assistant integration exists with Simplisafe but is limited to a virtual alarm control panel, which not very useful as you can you have many other options (key fob, keypads) to disable the alarm.

Google Assistant integration exists to arm the system. Disarming through voice command is not allowed for security reasons. You don’t want a burglar breaking in and using his voice to disarm the system.

<figure class="figure figure--25">
 <img src="/assets/images/other/simplisafe-ha.png" alt="" />
 <figcaption>
  <b>Home Assistant: Okay</b><br>Cannot use Simplisafe sensors, only control panel.
 </figcaption>
</figure>
<figure class="figure figure--25">
 <img src="/assets/images/integrations/google-home.png" alt="Small picture of a kitten" style="width: 100%" />
 <figcaption>
 <b>Voice: Okay</b><br>You can arm the system, but not disarm through voice. 
 </figcaption>
</figure>

<figure class="figure figure--25">
 <img src="/assets/images/integrations/na.png" alt="Small picture of a kitten" style="width: 100%" />
 <figcaption>
 <b>SmartThings: None</b><br> Integration does not exist.
 </figcaption>
</figure>
<figure class="figure figure--25">
 <img src="/assets/images/integrations/simplisafe-app.png" alt="Small picture of a kitten" style="width: 100%" />
 <figcaption>
 <b>Native App: Okay</b><br>Standard app.
 </figcaption>
</figure>


## The Competition
### Abode
![](\assets\images\product-photo\abode.jpg){:.image--xl.align-left}

There are professional security systems that can integrate with Home Assistant, but the home automation platform will be unstable using Home Assistant. If this is still the route for you, one option is to pair the Abode security system with Home Assistant, allowing Abode’s sensors to be recognized as Home Assistant entities. The **``Abode``** component communicates over the internet but hasn’t caused noticeable delays, according to a Reddit user I spoke with. The problem with this approach is that it relies on Home Assistant as the home automation platform, which isn’t stable enough to be left unattended. 

<figure style="width: 50%;" >
 <img src="\assets\images\other\abode-ha.png" alt="" />
 <figcaption>
Here is how Abode’s sensors will look like in HA. Like any other sensor.
 </figcaption>
</figure>

If you plan to start with simple lighting automations, then look into Abode’s recently released automation engine, **``Cue``**. It seems simple and easy to use, though I wouldn’t expect it to handle complex automations. The downside is that your Z-Wave devices must be compatible with Abode, which is not always the case.


### Ring Alarm
![](\assets\images\product-photo\ring.png){:.image--xl.align-left}

And the wait is over! After a lawsuit from ADT that delayed the release of Ring's alarm system, it is finally here. And just recently, some Home Assistant users developed a [**``Hass.io add-on``**](https://community.home-assistant.io/t/ring-alarm-mqtt-discovery-alarm-integration/88070) that integrates Ring's contact and motion sensors with Home Assistant. That means you can use Ring sensors for any home automation. I have trouble finding reliable Z-Wave sensors, so I would gladly go with Ring sensors.

Ring is the best home security system--it is the most affordable security system available and has most, if not all the key features that consumers need. Glass break sensors aren’t available with Ring, but using the new Alexa Guard feature with current-generation Amazon Echos can replicate that ability. Professional 24/7 monitoring starts at $10/month, which is the lowest price in the market.



