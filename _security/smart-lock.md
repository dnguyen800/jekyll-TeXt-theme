---
layout: article
title: Smart Locks
category: home security
permalink: /security/smart-lock

---
## Smart Locks
**Published on xx/xx/2019**
<front page banner here>

**Competitors in this space:** August, Schlage, Next x Yale

I’ve personally tested the following:

- August Smart Lock Pro with Connect Wi-Fi Bridge

### Overview
Whenever people ask me about smart locks, I ask them why they think it’s needed. The lack of an immediate response shows they haven’t considered the benefits or, more importantly, the risks that come with adding a smart lock to your home. It is easy to forget that the lock may be the only security measure standing between your home and an intruder, so don’t just buy a lock without a plan! Let’s start by learning what smart locks can do.

Like with most smart home items, the main draw of smart locks is convenience. Imagine never having to lock the door as it locks itself after you leave the house. There are times when I left the door unlocked and wished I had a smart lock, instead of stressing out over a potential break-in. Smart locks can be useful when you need to provide temporary access to dog walkers, visiting relatives and friends.  Like with smart garage door openers, smart locks can grant peace of mind that the door will always be locked. 

A smart lock adds convenience but also risks. If you do end up getting a smart lock, be sure to add a security camera as an extra detective measure for unauthorized entries. If someone unexpected arrives and bypasses the lock (maybe he snuck in right as you left the house, before the lock activated), the camera should alert of his presence. Here are some plausible scenarios where a smart lock adds risk to your home:


- The house remains unlocked for a period of time due to an automation, hub or presence sensor issue.
- The smart lock is physically unlocked but reports as locked. 
- Someone gains unauthorized access to SmartThings or Home Assistant (through a security vulnerability, or improperly exposing instance to the internet) and can control the lock.


![Image: August](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1551547842481_smart_lock-august-install.jpg)
![](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1551547850466_whitespace.png)


All smart locks require some disassembly of the current lock, so renters will need permission before making changes. The August Lock is the least noticeable installation, as it replaces the the thumb latch found on the door facing inside the home. Your landlord won’t notice unless he/she regularly enters your apartment—just remember to keep the original parts when you move out.

#### Considerations before buying a smart lock

- Ask yourself whether a lock is worth the additional risk.
- A lock may not properly lock due to the door jamming from weatherstripping or strike plate alignment. 
- Does it support Z-Wave or require an additional hub? Using another hub presents additional security risks, and the app may go unsupported in the future. 
- Will it fit your door? Check if single bolt or double bolt configuration. Is the door handle on the left or right side?
- Do you have additional security measures in case your smart lock is compromised?
- Thoroughly test automations if you plan to automate locking/unlocking.

#### What you get with a smart lock

- Unlock the door with your phone. Now you can go jogging without your keys.
- Get alerts of doors left unlocked.
- Give guests temporary access to the house with their own unique code or account.
- Lock your door automatically when you leave the neighborhood.

### August Locks
![](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1551548245683_august_logo.png)
![Image: August](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1551548259556_smart_lock-august-photo.jpg)


If you want to try out a smart lock but don’t own a home, then August locks might be the solution for you. Keep in mind that some disassembly of the current lock is required, so it is your responsibility to follow the rental agreements. August locks only require replacement of the thumb latch, so the lock replacement is unnoticeable from the outside and your (and landlord’s) existing keys will continue to work. I recommend the August Lock Pro for its Z-Wave support, so you can avoid using the poorly-reviewed August app and Connect Wi-Fi Bridge.


![Image: August](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1551550807859_august_compatibility.png)
![](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1551550829478_whitespace.png)


August locks only work on single bolt locks. I wasn’t familiar with the term, but luckily August has a nice illustration (see above) to explain the difference.

i hear on deals and home automation forums that the battery life on August locks are poor, lasting around x months. This would be bad normally, but it uses four AA batteries that are easily interchangeable by removing the front cover. I prefer this approach because the replacement is so easy, but maybe not good for residences that don’t see much traffic for months.

#### The Problems
I never tested the included August Connect Wi-Fi bridge, which lets you use its mobile app and the bluetooth on your phone to unlock. I’ve only read bad reviews about it, so I ended up selling it after I had the Z-Wave connection working with the August Pro. 

For security reasons, I don’t automatically lock/unlock the door based on my location. Instead, I use SmartThings notifications as a shortcut to open the app and unlock the door. I haven’t run into any issues with the door unlocking when it wasn’t supposed to, but I only tested for a few days. 

#### Installation and Smart Home integration
I installed an August Lock Pro on the garage entry door and it took about ~ two hours for a first-time install. Pairing to Home Assistant took another 10 minutes. Designing automations in Home Assistant  took much more time to get it right, as I had to find a timely and accurate presence sensor first. 

Check if your lock is a single bolt lock, as that is the only lock type compatible with August locks.  You should also check your door area for any potential jamming from weather stripping or strike plate misalignment. If you need to nudge the door forward or wiggle the key a certain way before closing the door, then the August lock will have issues.

The August Lock Pro supports Z-Wave, so I’m able to control the lock with SmartThings and Home Assistant. Google Assistant is supported through the Connect bridge or by association through SmartThings and Home Assistant integration.  Say “lock the front door in 5 minutes”


![Voice](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1543622841706_google_assistant.jpg)
![Home Assistant Z-Wave locks in Home Assistant](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1551550444139_smart_lock-august-ha.png)

![SmartThings: Official Works with SmartThings as it supports Z-Wave](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1543439973594_st-nest.png)
![Product App Simple, easy-to-use](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1543441089611_nest-app.png)


#### Recommended Reading


### Schlage Keypad Locks

![](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1551549479795_schlage_logo.png)
![](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1551549266302_smart_lock-schlage_keypad_lock-product.JPG)


Schlage Keypad Locks can offer most of the conveniences of a smart lock, but avoids certain risks and is slightly cheaper. A four-digit code is all that’s needed to unlock, and you have the multiple key codes available for guests. It’s inconvenient to revoke access by changing the keycode, but that is a problem most people will rarely deal with.

You don’t have to worry about remotely locking the door, as the door always locks when closed. You lose the ability to receive notifications when the door is unlocked, but that can be replaced with a camera or door sensor.

#### Installation and Smart Home Integration
If you’re a renter, you can’t install the lock as it replaces the entire door handle and requires a new set of keys.  The lock is powered by a 9V battery that lasts quite long—my battery is going strong for over a year.