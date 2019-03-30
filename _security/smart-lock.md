---
layout: article
title: Smart Locks
short_title: Smart Locks
excerpt: Now you'll never be locked out of the house, unless you forget your phone.
category: [security, home automation]
permalink: /security/smart-lock
key: security-smart_lock
aside:
  toc: true
banner: assets/images/overlay/smart-lock.jpg
mode: immersive
header:
  theme: dark
article_header:
  type: overlay
  theme: dark
  background_color: '#203028'
  background_image:
    gradient: 'linear-gradient(135deg, rgba(34, 139, 87 , .4), rgba(139, 34, 139, .4))'
    src: /assets/images/overlay/smart-lock.jpg

---

<!--more-->



**Competitors in this space:** August, Schlage, Next x Yale

*I’ve personally tested the following:*

|---
| ![](\assets\images\logo\august.png){:.image--lg} 
|:-:
| **August Smart Lock Pro** 

### What you need to know

**Whenever people ask me about smart locks, I ask them why they think it’s needed.** The lack of an immediate response shows they haven’t considered the benefits or, more importantly, the risks that come with adding a smart lock to your home. It is easy to forget that the lock may be the only security measure standing between your home and an intruder, so don’t just buy a lock without a plan! Let’s start by learning what smart locks can do.

Like with most smart home items, the main draw of smart locks is convenience. Imagine never having to lock the door as it locks itself after you leave the house. There are times when I left the door unlocked and wished I had a smart lock, instead of stressing out over a potential break-in. Smart locks can be useful when you need to provide temporary access to dog walkers, visiting relatives and friends.  Like with smart garage door openers, smart locks can grant peace of mind that the door will always be locked. 

A smart lock adds convenience but also risks. If you do end up getting a smart lock, be sure to add a security camera as an extra detective measure for unauthorized entries. If someone unexpected arrives and bypasses the lock (maybe he snuck in right as you left the house, before the lock activated), the camera should alert of his presence. Here are some plausible scenarios where a smart lock adds risk to your home:

> - The house remains unlocked for a period of time due to an automation, hub or presence sensor issue.
> - The smart lock is physically unlocked but reports as locked. 
> - Someone gains unauthorized access to SmartThings or Home Assistant (through a security vulnerability, or improperly exposing instance to the internet) and can control the lock.

<figure style="width: 65%;" >
 <img src="\assets\images\other\august-install.jpg" />
 <figcaption>
Removing the latch of a single bolt lock.<i>| August</i>
 </figcaption>
</figure>

All smart locks require some disassembly of the current lock, so renters will need permission before making changes. The August Lock is the least intrusive installation, as it replaces only the thumb latch found on the door facing inside the home. Your landlord won’t notice the change unless he/she regularly enters your apartment—just remember to re-install the original parts when you move out.

### Considerations before buying a smart lock

> - Ask yourself whether a lock is worth the additional risk.
> - A lock may not properly lock due to the door jamming from weatherstripping or strike plate alignment. 
> - **Does it support Z-Wave or require an additional hub?** Using another hub presents additional security risks, and the app may go unsupported in the future. 
> - **Will it fit your door?** Check if single bolt or double bolt configuration. Is the door handle on the left or right side?
> - Do you have additional security measures in case your smart lock is compromised?
> - Thoroughly test automations if you plan to automate locking/unlocking.

### What you get with a smart lock

> - Unlock the door with your phone. Now you can go jogging without your keys.
> - Get alerts of doors left unlocked.
> - Give guests temporary access to the house with their own unique code or account.
> - Lock your door automatically when you leave the neighborhood.

### Recommended Reading
> - ?
 

## August Locks
![](\assets\images\product-photo\august.jpg){:.image--lg.align-left}

**If you want to try out a smart lock but don’t own a home, then August locks might be the solution for you.** Keep in mind that some disassembly of the current lock is required, so it is your responsibility to follow the rental agreements. August locks only require replacement of the thumb latch, so the lock replacement is unnoticeable from the outside and your (and landlord’s) existing keys will continue to work. I recommend the August Lock Pro for its **``Z-Wave support``**, so you can avoid using the poorly-reviewed August app and Connect Wi-Fi Bridge.

**August locks only work on single bolt locks.** I wasn’t familiar with the term, but luckily August has a nice illustration (see below) to explain the difference.

<figure style="width: 65%;" >
 <img src="\assets\images\other\august-compatibility.png" />
 <figcaption>
August locks can only be installed on single bolt doors. <i>| August</i>
 </figcaption>
</figure>

I've read on deal and home automation forums that the battery life on August locks are poor, lasting only a few months. This would normally be bad, but the lock uses four AA batteries that are easily interchangeable by removing the front cover. I prefer this approach becausebattery replacement is so easy, but maybe not good for residences that aren't within driving distance.

### The Problems

I never tested the included August Connect Wi-Fi bridge, which lets you unlock from anywhere with an internet connection.  I’ve only read bad reviews about it, so I ended up selling it after I had the Z-Wave connection working with the August Pro. 

For security reasons, I don’t automatically lock/unlock the door using geolocation. Instead, I use SmartThings notifications as a shortcut to open the app and unlock the door. I haven’t run into any issues with the door unlocking when it wasn’t supposed to, but I only tested for a few days. 

### Installation and Smart Home integration

**Check if your lock is a single bolt lock, as that is the only lock type compatible with August locks.** You should also check your door area for any potential jamming from weather stripping or strike plate misalignment. If you need to nudge the door forward or wiggle the key a certain way before closing the door, then the August lock will have issues. I installed an August Lock Pro on the garage entry door and it took one hour two hour for a first-time install. 

The Smart Lock Pro supports **``Z-Wave``**, so connecting to SmartThings was incredibly easy--I won't explain how to do it here. Connecting to Home Assistant took several hours of researching, because I had not defined a network key on my Z-Wave device to do secure inclusions and so the lock was detected as an unknown device. Designing automations in Home Assistant took much more time to get it right, as I had to first find a timely and accurate presence sensor first. Read about it [here!](http://localhost:4000/security/sensor#presence-sensordevice-tracker)

Google Assistant is supported through the Connect bridge or by association through SmartThings and Home Assistant integration.  

Say “lock the front door in 5 minutes”


<figure class="figure figure--50">
 <img src="/assets/images/integrations/august-lock-ha.png" alt="Small picture of a kitten" />
 <figcaption>
 <b>Home Assistant: Average</b><br>Quite difficult to setup. Required searching on forums for a solution. 
 </figcaption>
</figure>

<figure class="figure figure--50">
 <img src="/assets/images/integrations/google-home.png" alt="Small picture of a kitten" style="width: 100%" />
 <figcaption>
 <b>Voice: Great</b><br>Pair the TV using the Google Home app.
 </figcaption>
</figure>

<figure class="figure figure--50">
 <img src="/assets/images/integrations/august-st.png" alt="Small picture of a kitten" style="width: 100%; height: 100%" />
 <figcaption>
 <b>SmartThings: Great</b><br> Easily connects to SmartThings
 </figcaption>
</figure>

<figure class="figure figure--50">
 <img src="/assets/images/integrations/august-app.png" alt="Small picture of a kitten" style="width: 100%" />
 <figcaption>
 <b>Native App: Great</b><br>Simple, easy-to-use
 </figcaption>
</figure>


## Schlage Keypad Locks

![](\assets\images\product-photo\schlage-keypad.jpg){:.image--xl.align-left}

Schlage Keypad Locks can offer most of the conveniences of a smart lock, but avoids certain risks and is slightly cheaper. A four-digit code is all that’s needed to unlock, and you have the multiple key codes available for guests. It’s inconvenient to revoke access by changing the keycode, but that is a problem most people will rarely deal with.

You don’t have to worry about remotely locking the door, as the door always locks when closed. You lose the ability to receive notifications when the door is unlocked, but that can be replaced with a camera or door sensor.

### Installation and Smart Home Integration
If you’re a renter, you can’t install the lock as it replaces the entire door handle and requires a new set of keys.  The lock is powered by a 9V battery that lasts quite long—my battery is going strong for over a year.