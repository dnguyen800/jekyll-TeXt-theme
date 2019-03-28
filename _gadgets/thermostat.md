---
layout: article
title: Thermostats
short_title: Thermostats
excerpt: If I had something interesting to say about thermostats, I would say it here.
category: [gadgets, home automation]
permalink: /gadgets/thermostat
key: gadgets-thermostat
aside:
  toc: true
banner: assets/images/overlay/thermostat.jpg
mode: immersive
header:
  theme: dark
article_header:
  type: overlay
  theme: dark
  background_color: '#203028'
  background_image:
    gradient: 'linear-gradient(135deg, rgba(34, 139, 87 , .4), rgba(139, 34, 139, .4))'
    src: /assets/images/overlay/thermostat.jpg
---

<!--more-->

**Competitors in this space:** Nest, Ecobee, Honeywell, Emerson

I’ve personally tested the following:

|---
| ![](\assets\images\logo\nest.png){:.image--md} |  ![](\assets\images\logo\ecobee.png){:.image--md} 
|:-:|:-:
| **Nest 3rd Gen** | **Ecobee 3**<br>**Ecobee 4** 


### What you need to know

I can count on one hand the number of times my smart thermostat showed its value, but for those times it felt invaluable tool. As I was about to drive home on a cold night after dinner,  I realized I could open the Nest app on my phone and crank up the thermostat temperature. That feeling of entering a warm house after spending hours in the cold is like taking a hot a shower after days of sweaty hiking—it was amazing—the very definition of comfort.

I rarely use a smart thermostat to its full potential, but I can see the value for others. For people who regularly use the furnace, a smart thermostat will warm up the house  at the right times and electricity cost will be slightly less than without a smart thermostat. If you live in a colder climate where chilly nights are frequent, then the thermostat’s value definitely shows. For instance, you can use a Nest thermostat to heat up the house and prevent pipes from freezing and bursting. If you’re a frugal person who never turns on the thermostat in the first place, then there is no benefit to be gained here.

Smart thermostats like Nest and Ecobee regularly go on sale so it’s easy to snag one at a reasonable price of $170.

### Considerations Before Buying A Smart Thermostat

> - Use the Nest compatibility checker to see if your home’s existing wiring is compatible. 
> - If you have two thermostats and two separate zones, you may need two smart thermostats. Some furnaces cannot maintain dual temperatures that vary too widely.. Having the first floor at 60F and the second floor at 70F may put too much strain on your system.

### What You Get With a Smart Thermostat

> - Warm up or cool down the house before arriving home.
> - Forget about adjusting the thermostat—the home/away assist feature turns off the thermostat for you.
> - Safety alerts and reminders, like extreme cold weather, to turn on heating.
> - Learning specific behaviors, like warming up the house when you wake up.
> - Give roommates access via app, if they cannot physically access it.
> - Change the thermostat temperature while still in bed.

### Recommended Reading

> - Nest Online Compatibility Checker to see if your home is compatible.
> - NST Manager - Smartthings Nest Unofficial Integration
> - Home Assistant Nest Component

## Nest Thermostats
 ![](\assets\images\product-photo\nest-thermostat.png){:.image--xl.align-left}

**I recommend any smart thermostat currently on sale, which is usually the Nest E. It has all important features of the Nest 3rd Gen, but regularly goes on sale for $130 or less.** Get the Nest 3rd Gen if you want a nicer looking, metal finish on your thermostat. Ecobees are just as good as Nest, so there is no wrong choice here.

Honestly, there is not much to rave or complain about--the Nest is what you expect out of a smart thermostat. The Nest app is straightforward to use, and according to [this security study](https://www.tomsguide.com/us/smart-home-leaky-apps,news-29319.html) of smart home apps, Nest is one of the few apps that encrypts communication between thermostat, even when on the same local network. 

### The Problems

There aren't any major problems with Nest, but the Home/Away Assist feature can be very slow to detect presence changes. I've compared Nest times to actual times and have seen hour-long gaps in detection. I've also arrived home to see that the Nest cameras remained on (should be off when someone is home) and the thermostat not adjusted. If you want to come home to a warm house, the most reliable way is to use the Nest app before heading home.

### Installation and Smart Home Integration

Physical installation is not difficult, but you need to use the Nest compatibility checker if your home’s existing wiring is compatible. I had to call tech support once because there were more wires in my existing installation than what was covered in the installation guide. Physical installation requires some basic do-it-yourself **``DIY``** skills like drilling holes and basic electrical wiring.

Connecting the Nest to SmartThings uses an unofficial SmartApp called [NST Manager](https://community.smartthings.com/t/release-nst-manager-v5-0/83228). It's not difficult to setup, but requires creating a Nest developer account,  ~. As an unofficial integration, it's quite impressive to have the thermostat, ~ cameras working in SmartThings. Kudos to them

Nest thermostats come with a wall plate to ~


Voice control - The Home/Away Assist feature on the Nest app is not timely, so the other option you have is to use voice control, say, in the car driving home, to warm up the house before you arrive. I haven't tested this feature but ~. Nest and GOogle Assistant work well ~ and work remotely, when you're not connected to the home network.

Very rarely do I need to change the temperature, so home automation integration is not all that important to me. I find that using the app is the most convenient way to fiddle with the thermostat. But it is very easy to connect the Nest to Home Assistant. SmartThings requires installation of a device handler, but that’s not too hard.

<figure class="figure figure--50">
 <img src="/assets/images/integrations/nest-thermostat-ha.png" alt="Small picture of a kitten" />
 <figcaption>
 <b>Home Assistant: Good</b><br>Create a developer account, client ID and key, then add to your HA configuration. Looks great!
 </figcaption>
</figure>

<figure class="figure figure--50">
 <img src="/assets/images/integrations/google-home.png" alt="Small picture of a kitten" style="width: 100%" />
 <figcaption>
 <b>Voice: Great</b><br>Really easy to setup through Google Home. Pointless feature though!
 </figcaption>
</figure>

<figure class="figure figure--50">
 <img src="/assets/images/integrations/nest-thermostat-st.png" alt="Small picture of a kitten" style="width: 100%; height: 100%" />
 <figcaption>
 <b>SmartThings: Good</b><br> Tedious one-time setup. Requires developer account and device handler setup.
 </figcaption>
</figure>

<figure class="figure figure--50">
 <img src="/assets/images/integrations/nest-thermostat-app.png" alt="Small picture of a kitten" style="width: 100%" />
 <figcaption>
 <b>Native App: Great</b><br> Simple, easy-to-use.
 </figcaption>
</figure>


## Ecobee Thermostats
 ![](\assets\images\product-photo\ecobee-thermostat.png){:.image--xl.align-left}

I have a confession to make: I only purchased the Ecobee instead of Nest because it was currently on sale. I read comparison articles but didn't find much notable differences between the two, so I went ahead and bought it. 

Works just as well. Same level of integration. Actually supports SmartThings officially.

Ecobee includes room sensors, which can also act as really slow room occupancy sensors. In a large house where temperature varies greatly, I can see this being useful, but ~ this is more of a nice-to-have.

Both the Ecobee 3 and Ecobee 4 are available for sale. The only difference I noted was the inclusion of Amazon Alexa, which I found to be a useless feature. The location of my thermostats are in low traffic areas (hallways, stairs), and there was rarely a time when I needed Alexa to do something while standing in the hallway. If I do, I end up yelling ~and the wrong Echo speaker picks up my request.  You will have to yell at your thermostat to get attention. I'm not sure why I paid extra money for that.

### The problems

I haven't encountered any major problems to note. I have not tested the accuracy of the Home/Away feature, but I don't think it will be any better than Nest, so expect delayed updates up to an hour. If you want to come home to a warm house, you will need to use the app.

### Installation and Smart Home Integration

The installation process is just as easy as Nest--all steps are covered in the app. Labels are included for the thermostat wires. There is a compatibility checker section on the Ecobee app to guide Physical installation requires some basic do-it-yourself **``DIY``** skills like drilling holes and basic electrical wiring.

Connecting the sensors to the Ecobee is incredibly easy. Just remove the tape from the battery and the thermostat will detect the sensor and confirm with you to add to your home.

Ecobee is officially supported by SmartThings and integrates easily using a SmartThings SmartApp.

Comes with a wall plate to hide the hole or any visible wires.

<figure class="figure figure--50">
 <img src="/assets/images/integrations/ecobee-ha.png" alt="Small picture of a kitten" />
 <figcaption>
 <b>Home Assistant: Good</b><br>Create a developer account, client ID and key, then add to your HA configuration. Looks great!
 </figcaption>
</figure>

<figure class="figure figure--50">
 <img src="/assets/images/integrations/google-home.png" alt="Small picture of a kitten" style="width: 100%" />
 <figcaption>
 <b>Voice: Great</b><br>Really easy to setup through Google Home. Pointless feature though!
 </figcaption>
</figure>

<figure class="figure figure--50">
 <img src="/assets/images/integrations/ecobee-st.png" alt="Small picture of a kitten" style="width: 100%; height: 100%" />
 <figcaption>
 <b>SmartThings: Great</b><br> Official integration, easy to set up.
 </figcaption>
</figure>

<figure class="figure figure--50">
 <img src="/assets/images/integrations/ecobee-app.png" alt="Small picture of a kitten" style="width: 100%" />
 <figcaption>
 <b>Native App: Great</b><br> Simple, easy-to-use.
 </figcaption>
</figure>