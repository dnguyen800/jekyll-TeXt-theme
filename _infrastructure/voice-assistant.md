---
layout: article
title: Voice Assistant
short_title: Voice Assistant
excerpt: One of the most critical infrastructure components to your smart home.
category: [infrastructure, home automation]
permalink: /infrastructure/voice-assistant
key: infrastructure-voice_assistant
aside:
  toc: true
banner: assets/images/overlay/voice-assistant.jpg
mode: immersive
header:
  theme: dark
article_header:
  type: overlay
  theme: dark
  background_color: '#203028'
  background_image:
    gradient: 'linear-gradient(135deg, rgba(34, 139, 87 , .4), rgba(139, 34, 139, .4))'
    src: /assets/images/overlay/voice-assistant.jpg
---

<!--more-->

**Competitors in this space:** Google Assistant, Amazon Alexa, Apple Siri 

I’ve personally tested the following:

| Google Assistant| Amazon Alexa | Apple Siri |
|:-------:|:--------:|:---------:|
| ![Google Assistant](\assets\images\logo\google-assistant.jpg){:.image--lg} | ![Alexa](\assets\images\logo\alexa.png){:.image--md} | ![siri](\assets\images\logo\siri.jpg){:.image--md} |



## What you need to know
A voice assistant paired with a smart home—what do you get with it?  Besides asking about the weather and setting timers, voice assistants offer another convenient way to control the lights and TV—which can be very useful when your hands are full—like when carrying groceries. 

Things get more interesting when voice assistants are linked to media services like Youtube TV, Netflix and Hulu, but then you start to see the disparities between Google Assistant and Alexa. Though one thing that all voice assistants have in common is the amount of yelling needed for your voice to be recognized. And that’s okay—I don’t expect microphones to be any better than human ears, which already have trouble hearing me. If you factor in background noise from music, television or the kitchen, it’s a wonder that my voice is recognized at all. 

When you get into the details of the supported integrations with voice assistants, you’ll quickly learn that most are not direct integrations. For example, most integrations support Actions on Google, which requires saying “Hey Google, ask Harmony…” to get anything done. Direct integrations are slowly being added, like Logitech Harmony, so things will get better. My point is that training is needed on your end to learn specific phrases to use voice assistants, whether it’s using Google, Alexa, or Siri.

When testing voice control with lighting, I realized that naming convention of devices is important to avoid confusion. If I have a light strip named “TV,” a Chromecast called “living room TV”, and an Android TV in the living room, there’s going to be some confusion when saying “turn off the TV.” 

### Considerations before choosing a voice assistant
> - **Test out the voice assistants yourself** by purchasing a cheap mini speaker or using your phone. 
> - **Search for key words like “direct integration”** to learn if your product supports voice assistant directly.
> - **Consider privacy implications of including always-on voice assistants.**

### What you get with a voice assistant
> - A hands-free way to control your lights.
> - A basic kitchen assistant for setting timers, converting units, and more.

### Recommended Reading

> - Google routines with alarm clock
> - Home Assistant integration with Homekit & Siri opens up the platform to many unsupported devices
> - How Apple anonymizes Siri requests and personal information

## Google Assistant
![Google Assistant logo](\assets\images\logo\google-assistant.jpg){:.image--xl.align-left}


**If you are an Android user, it makes sense to stick with Google Assistant because of its tight integration with the Android OS, ever expanding features and device compatibility.**  Google is ahead of the pack with its very useful Google Home app, which also has a streamlined UI that can be displayed on a tablet or phone. It is slowly replacing the functions of my SmartThings hub, though it still can’t perform any real automations that utilize sensors. One feature I love is using the **``Good Morning``** Google Routine and tying it to my phone’s alarm app. I’ve been waiting for something like that for ages!

<figure style="width: 100%;" >
 <img src="\assets\images\other\google_home_app.png" alt="" />
 <figcaption>
The revamped Google Home app. It’s not customizable, but at least it’s easy on the eyes.
 </figcaption>
</figure>

Controlling the lights with Google Assistant works as you would expect if you say the full name of the light, like “living room light.” Google Assistant offer direct integration with SmartThings, so every device in SmartThings can be voice controlled by Assistant, except certain actions like the disarming of alarms and locks. Things get murky when more context is needed before performing an action, but Google has a room assignment feature that helps with that. 

By assigning the light and Google Home speaker locations to their proper rooms, you can say something vague like **``turn off the lights``** and the closest Google Home speaker will turn off the lights in the room where the speaker is located in. This feature doesn’t work when using Google Assistant on your phone, as it doesn’t know what room it is currently in. There are other limitations to deal with, like adding a light to multiple rooms, but can be addressed using SmartThings scenes and Home Assistant groups. To get a better sense of what happens when you say a command, here is my understanding of Google Assistant’s logic when processing light commands:


> - **``Turn off the lights``** turns off the lights in the room where the Google Home speaker is located.
> - **``Turn off the living room lights``** turns off the lights in the Google room titled “Living Room”, or the light named “living room.”
> - **``Turn off all the lights``** turns off all the lights in the home where the Google Home is located.
> - **``Turn off the lights upstairs``** will turn off a group of lights titled “Upstairs” or any lights with the word “upstairs” in their name. The group must be defined in Home Assistant or SmartThings (as a scene) if lights in this group are already assigned to rooms in the Google Home app.

### The Problems
Google and Amazon continue to add new features at a rapid pace, making it a futile effort for me to do any detailed comparison between the two. One area where Google lacks is integration with video services like Hulu, Playstation Vue, and Prime Video. With Google, you can say **``Play Castlevania on Netflix``**, but not **``play The Good Place on Hulu.``** To my surprise, Amazon Alexa is much better at voice control, supporting Netflix, Hulu, Playstation Vue, Prime Video, and other smaller channels. Voice control in media services is not a deal breaker for me, since it doesn’t work on most of the apps I use anyways. 

<figure style="width: 100%;" >
 <img src="\assets\images\other\google-media-integration.png" alt="" />
 <figcaption>
The limited number of media integrations that Google Assistant supports. Not listed is Youtube TV, which works amazingly well with Google Assistant.
 </figcaption>
</figure>

Google Assistant is directly integrated into the home screen of phones running the latest stock Android, yet my phone still has trouble responding to the **``OK Google``** phrase, even when the phone is charging or on the home screen where Google Assistant is active. I was expecting better integration than this, but I understand phones can’t always be listening. That would be getting creepy anyways.

Google and Amazon’s voice assistants work best when there is only one user to recognize. Google supports voice matching and multiple accounts, but in practice, I found little success with Google Home differentiating between my roommate and my voice. It is not a problem for controlling lights and TV, but becomes a problem when playing music on Spotify—Google would end up playing music on the wrong Spotify account and Spotify terminates my active music session. I haven’t tested Amazon Echo and Alexa Household feature either, but their multi-user support is limited to two people. Again, this is an annoyance when playing music, but not controlling lights. 


## Amazon Alexa
![Alexa](\assets\images\logo\alexa.png){:.image--lg.align-left}

If you already have Amazon Echo speakers and Fire TVs, then Amazon Alexa is sufficient for basic control of lights, and will likely catch up in feature set with Google soon. Alexa is much better at voice control with video services than Google and its Fire 4K TV sticks are of great value, making it an almost perfect pairing for media.  The only missing features I can think of are: Youtube (not a big deal), Youtube TV (a bigger deal) and using multi-room audio with your local music library via Plex. I still don’t think it’s worth switching ecosystems if you are already invested in one. There is one feature on newer Amazon Echo devices unique to Alexa, and that is Alexa Guard, which can detect the sound of windows breaking from a burglary.

## Siri
![siri](\assets\images\logo\siri.jpg){:.image--lg.align-left}

Siri and Homekit can’t do much more than basic controls of lights, media, and that’s okay because it doesn’t need to do more. I use a voice assistant mainly to turn on the lights or set a scene, and Siri can do that just fine. Apple deserves credit for pushing privacy as a feature of their products, including Siri. Normally, I wouldn’t recommend Siri for use in any smart home, but now it is possible for Home Assistant to integrate with Homekit (and by association, Siri) to any light, switch, thermostat, lock, garage door, or media player that Home Assistant supports. Device compatibility is no longer an issue in this case.

