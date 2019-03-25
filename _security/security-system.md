---
layout: article
title: Security Systems
category: home security
permalink: /security/security-system
---
## Security Systems
**Published on xx/xx/2019**

**Competitors in this space: **Ring Alarm, Nest Secure, Simplisafe, Abode, alarm.com, Frontpoint Security, ADT

I’ve personally tested the following:

- Simplisafe (latest version)
- SmartThings (DIY solution)

### Overview
Like the cord-cutting revolution with cable TV, the home security system market is entering a new era of affordable security monitoring without contracts. Professional installation isn’t needed with these systems unless you are looking to install wired sensors in the house.

Your security system purchase has an impact on home automation, as there are ways to use the security system’s sensors with your home automation platform to avoid duplicate sensors.  Abode and and Ring offer unofficial integrations with Home Assistant, though your home automation platform may not be the most stable with this setup. So choose wisely!

There are few differentiating features between competitors as all professional security systems have the essential features: a 24-hour battery backup, cellular connection (included with monitoring service), and the “smashsafe” feature (if someone smashes a keypad or hub, you’re alerted).  These features are not available with DIY solutions without a clever homemade solution.

I’ve believe there are three categories I cover that will fit most people’s needs around security. If you are just a little bit serious about protecting your home, then I strongly suggest avoid the DIY route and look into an official provider like Ring.

#### Considerations before buying a security system

- Decide on building a DIY or purchasing a professional security system.
- Decide if you want to use home security sensor with an unstable home automation platform.

#### What you get with a security system

- In theory, you get more reliable sensors that have been thoroughly tested with the security system.
- 24/7 security monitoring, costing between $10-25 a month.


### DIY Security System
![](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1547688004057_smartthings_logo.jpg)
![](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1547500802198_security_system-smartthings-photo.jpg)
![](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1547484662702_security_system-smart_home_monitor-app.png)


You can use your existing SmartThings hub and sensors to create a simple security system with little to no additional investment, but there are several deficiencies that prevent it from being a mostly hands-off experience.  I used the Smart Home Monitor in the SmartThings app and the SHM Delay SmartApp, along with a few devices (Fire tablet, ActionTiles license, Konnected module, power converter, cables) to get it up and running. The amount of work I put into it and the annoyances I’ve yet to fix made me realize it’s worth getting a professional system like Ring. Let’s talk about those annoyances now.

I wanted to use my phone’s location to automatically arm and disarm the system, but the SmartThings presence sensor feature is too unreliable on Android phones due to its battery saver feature. There is a Life360 app integration with SmartThings that is better, but my initial testing show it’s still not fast enough to disarm the system before arriving home. 


![I wall-mounted a tablet where the alarm keypad used to be. Easy to do with less risk compared to directly wiring the tablet to a power source.](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1551496729241_security_system-diy-tablet02.jpg)


Without an automated method to arm and disarm the system, I installed a wall-mounted tablet so I could arm the system before I left the house. I used an old LG  tablet ($35), an ActionTiles license ($25), and some cables and converters ($11) to mount the tablet. 

#### The Problems
The SHM Delay app is critical for a working DIY security system, as the Smart Home Monitor in SmartThings doesn’t have basic features like entry/exit delays (really??). 
I have spent days tweaking the SHM Delay app but still run into false alarms. I’m sure it’s not working correctly due to my mistakes, but the fact that I’m spending hours out of my day  to fix it is enough for me to switch to a professional system.

Once I was able to get a working system in place, I started thinking about the ways the system could fail.  What if the tablet stops responding and I can’t disarm the alarm? What if someone smashes the siren or disconnects SmartThings?  What if SmartThings servers go offline? I eventually realized the harsh truth that these devices aren’t designed to be a security system and don’t have the safeguards to protect my home.  In the end, I disabled the siren and added a camera in the living room. I now rely on my phone for intrusion alerts, which I hope I am awake to respond to it. 

Sidenote: If your home already has a pre-wired security system, you can use a device called Konnected ($89) to use the wired sensors in home automation hubs like SmartThings. The downside is you’re still stuck with the limitations of a DIY security system that I described.



### Self Installation with Professional Monitoring
### Abode
![Image: Ring](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1551497444750_security_system-ring-product02.jpg)
![](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1551497396949_home_assistant_logo.png)
![Image: Abode](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1551497811836_security_system-abode-photo02.jpg)


There are professional security systems that can integrate with Home Assistant, but the home automation platform will be unstable with this solution. One option is to pair the Abode security system with Home Assistant, allowing Abode’s sensors to be recognized as sensors in Home Assistant. The integration communicates over the internet but hasn’t caused noticeable delays, according to a Reddit user I spoke with. The problem with this approach is that it relies on Home Assistant as the home automation platform, but it isn’t stable enough to be left unmanaged.  


![Here is how Abode’s sensors will look like in HA. Like any other sensor.](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1547704990261_security_system-abode-ha.png)
![](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1551498126992_whitespace.png)

If you plan to start with simple lighting automations, then look into Abode’s recently released automation engine, Cue. It seems simple and easy to use, though I wouldn’t expect it to handle complex automations. The downside is making sure your devices are compatible with Abode. 


### Ring
![](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1551498917111_security_system-ring-product02.jpg)
![](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1551498903761_whitespace.png)


The wait is over! The Ring Alarm integrates with Home Assistant with the still work-in-progress Hass.io add-on. Ring is the best option for the future, as it is the most affordable security system available and has most, if not all the key features that consumers need. Glass break sensors aren’t available with Ring, but using the new Alexa Guard feature with current-generation Amazon Echos can replicate that ability. Professional monitoring starts at $10/month, which is the lowest price in the market.


### Simplisafe
![](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1551499324232_simplisafe_logo.jpg)
![Simplisafe](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1551499338046_security_system-simplisafe-photo03.jpg)


If you don’t mind having duplicate sensors for home automation and security, then a dedicated security system is the most reliable way to securing your home. My friend was looking for such a system, so I suggested Simplisafe, based on the Wirecutter’s recommendation. If I were to do it all over again, I’d try out Ring Alarm, but my experience with Simplisafe has been nothing but excellent—besides the expensive monitoring cost.  

Simplisafe offers a security camera which works as described, but isn’t useful without their $25/month monitoring service, as you don’t have access to the mobile app.  Visual verification is an exclusive feature that allows the monitoring center to access your camera feed and verify an intrusion, though it maybe not worth the privacy risk, especially after the recent Ring incident. The variety of security sensors available is unmatched—you can buy an (really loud 105db) siren, key fob, keypad, panic button, glass break sensor—which aren’t available on Ring. 

I haphazardly tested a few features based on what I could reasonably test without setting off police alerts. Upon unplugging the hub, an e-mail alert was sent within seconds—that is insanely fast!  The door sensors have been accurate so far, and the motion sensors are more responsive than the Z-wave ones I use—it even detected motion while I was crawling on the floor. If you don’t want pets to set off the alarm, you can rotate the sensor upside-down so the sensor can only sees straight ahead and towards the ceiling.

Where Simplisafe fails is the high monthly price for critical functions. Yes, it was a dick move to hide access to the mobile app behind the $25/month tier. Simplisafe is trying to increase the value of the tier by including free camera storage, but that is a ploy to purchase their unproven indoor and doorbell cameras.  The price tag stings even more when compared to Ring’s $10/month service, which offers the same 24/7 monitoring, cellular backup, plus free storage of camera footage history.


![Simplisfe HA integration is limited to alarm control panel, which will look something like this.](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1547685566938_security_system-simplisafe-ha.png)


#### Installation and Smart Home Integration
Installation is a breeze as the included sensors are already paired with the system if you purchase a kit.

Home Assistant integration exists with Simplisafe but is limited to a virtual alarm control panel, which not very useful as you can you have many other options (key fob, keypads) to disable the alarm.

Google Assistant integration exists to arm the system. Disarming is not allowed for security reasons. You don’t want a burglar breaking in and using his voice to disarm the system.

#### Recommended Reading

- The Wirecutter’s security system recommendation