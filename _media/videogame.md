---
layout: article
title: Video Game Consoles
category: media

---
## Video Game Consoles

**Published xx/xx/2019**

![Image: Fabian Albert on Unsplash](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1551412484922_videogame-front_page.jpg)


**Competitors in this space:** Microsoft, Sony, Nintendo

I've personally tested the following:

- Microsoft Xbox One X
- Sony Playstation 4 Pro
- Nintendo Switch
- Windows PC

### Overview
Video game consoles have always been a part of my media center, so it would be a glaring omission if I couldn’t include them in my smart home automations. I use them as blu-ray players for those rare occasions I revisit an old movie. The Xbox One makes for a noteworthy media streaming device—even segregated apps Youtube TV, Amazon Video is available. If I had to choose only one device connected to my TV, it would likely be a videogame console because it plays games, blu-rays, and most major apps.

Consoles aren’t known to be open platforms, but several clever people developed ways to connect the Xbox One and Playstation 4 consoles to Home Assistant. These are unofficial methods that Sony or Microsoft could discontinue in the future, but I’ll give it a couple of years before that happens.

With these Home Assistant integrations, I can see the game currently playing (see examples below). Not exactly useful, but it sure looks nice on the UI. The other benefit is that my TV lighting automations will be even more precise, now that I can detect when a game is playing.


#### Considerations before buying a video game console

- Nothing to report.

#### What you get with integrating a video game console

- Create more accurate lighting automations (e.g. turn on the lights when a game is playing).
- Use as a blu-ray player (4K for XboxOne S & X).
- Supports video and music apps like Hulu, Spotify, Netflix.
- Integration looks cool on Home Assistant.

### Microsoft Xbox One

![Image: Microsoft](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1546884407984_videogame-xboxone-logo.png)


The original Xbox One was supposed to be the ultimate media center where you could play games and watch TV—all on the same screen! Well, that idea failed horribly but the Xbox One gained some awesome features recently, like a 4K bluray player and plenty of video apps (Youtube TV, Hulu, Spotify). Smart home integration was recently added in the form of a Home Assistant (Hass.io) add-on and it’s quite impressive, with the ability to display the game currently playing in Home Assistant—all without any manual intervention. Status updates to Home Assistant are quick—within one to two seconds—so lighting automations are instant when I start playing a game.


![Voice: Works with Alexa Alexa now works on XboxOne to launch games and apps, which gives me hope that Google Assistant will work on it one day.](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1550033393033_voice_assistant-amazon_echo-product.jpg)
![Home Assistant: Unofficial Integration Once installed, the XboxOne media player works great. Powering on remotely also works.](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1546902071999_videogame-xboxone-ha-enc2.gif)


#### The Problems
I’ve run into a few issues, like having to re-authenticate my Xbox account from time to time. It’s not a completely hands-off integration, but it’s not a critical component that I can survive without it working. 

#### Installation and Smart Home Integration
The initial setup is only difficult if you don’t read the instructions.  Install the Hass.io addon and authenticate to Xbox Live per the add-on instructions. Find your Xbox One’s device ID (see instructions again), then add the Xbox One media player platform and device ID in your configuration.yaml file. Be sure to read the instructions thoroughly!


### Sony Playstation 4
![Image: Sony](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1546884506627_videogame-ps4-logo.png)

As of Home Assistant 0.89, the Playstation 4 is supported with the same features as the XboxOne add-on. It is even easier to authenticate using the new Home Assistant integration process, which makes this an easy recommendation if you already have a PS4. Remotely powering on now works, so you can now use voice control for that. Cover art works on some but not all games.  I’m happy that more people can use this integration and show off the game playing, and design lighting automations based on the PS4’s state.


![Voice: Not Supported No voice control available.](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1550074899637_not_available.png)
![Home Assistant: Unofficial Integration Very difficult setup process. Manual downloading of game covers required. Once setup, there are no issues (for me at least).](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1546905064973_videogame-ps4-ha.gif)


#### Installation and Smart Home Integration
I haven’t had any authentication issues with the Playstation 4 add-on like I did with the Xbox One. With the new component added to Home Assistant 0.89, installation is a breeze compared to the old method. For reference, here is the tutorial from Home Assistant user @cheynespc for directions to install the old Playstation 4 Hass.io add-on.



### Nintendo Switch

![Image: Nintendo](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1551422774263_videogame-nintendo-logo.png)


No integration exists for the Nintendo Switch and it’s not likely to happen in the future. If you need a method to detect if the Switch is connected to the dock, I would use a LAN adapter connected to the the Switch dock and Home Assistant’s nmap device tracker to detect the LAN adapter’s presence. If the Switch uses a dedicated HDMI port and your TV and/or AV receiver is connected to Home Assistant, then create an automation that detects if that HDMI port is currently selected.

#### Recommended Reading

- Use Alexa on XboxOne support article
- Link to my Home Assistant configuration for Playstation 4 media player
- Playstation 4 Home Assistant custom component
- Xbox One Hass.io add-on
- Playstation 4 Hass.io add-on tutorial by user @cheynespc