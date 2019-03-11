---
layout: article
title: Media Streaming Devices
category: media

---
## Media Streaming Devices
** Published on xx/xx/2019**
![](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1551423657096_media_streaming-front_page.jpg)


**Competitors in this space:** Google Chromecast, Amazon Fire TV, Roku, Apple TV, Android TV

I’ve personally tested the following:

- Google Chromecast Ultra, 2nd gen, 1st gen
- Roku Streaming Stick+, Premiere
- Apple TV 2
- Amazon Fire TV 2, TV stick (1st gen)

### Overview
The new lineup of media streaming devices continues to impress every year. With more features like 4K, voice control, and HDR added into physically smaller devices, I feel like I can constantly upgrade my old TV at a cheap price. Indeed, my 2015 Vizio TV is more useful with a Roku Streaming Stick+ so I no longer have to browse through a slow, ancient web interface. 

Sidenote: Though media streaming devices are capable of impressive feats, I’ve found that the best TV watching experience lies with a high-end smart TV like the LG OLED series.  The gyroscopic remote controls make it as easy as possible for anyone to pick up a remote and intuitively browse through the TV’s wide selection of apps. The LG OLED TVs are really impressive, if you can afford it. See my TV Section to learn more.

#### Things to consider before buying a media streaming device

- A media streaming device may not be necessary if your TV or video game console supports the same video apps.
- Companies sell 1080p and 4K versions of their products. I recommend future-proofing by purchasing the 4K version.
- Beware: When you use a media streaming device or service, your TV viewing data is being collected. There’s a reason why these devices are so cheap: the companies are collecting data on the videos you watch, and possibly selling the information to third parties, like advertisers.

#### What you get with a media streaming device

- Upgrade an outdated TV with new features like voice control, and a faster browsing experience.
- Remotely switch HDMI ports using emulated Roku feature on Home Assistant
- Integrated smart home automations, as nearly all devices are supported by Home Assistant
- Move devices to different TVs.

### Roku
![](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1550159628930_roku+logo.png)


I recently switched over to the Roku Streaming Stick+, and agree with the Wirecutter that it is the best media streaming device available today. It supports both Google Assistant and Amazon Alexa, as well as Youtube TV and Amazon Prime Video—all without any workarounds. Normally when you try to be a jack of all trades, you end up being good at nothing. In this case, Roku ends up being good enough for my needs, and I haven’t found anything missing besides deeper integration with voice assistants. I just hope Google and Amazon don’t take away their respective apps from Roku and create more segregated market.

I find the Roku voice search function on the remote is much more useful with the ability to search for a title through multiple apps. I never purchase TV shows or movies, so I like Roku’s search function because it highlights the free or subscription options first. Google Assistant and Alexa are officially supported, though it is limited to opening apps, powering on TV or changing volume. Voice commands aren’t as deeply integrated at the application level, compared to the Fire TV or even the Chromecast.

On the premium Roku products like the Streaming Stick+, the remote includes extra nifty features like TV power and volume control buttons. This also works in tangent with HDMI ARC to control the AV receiver or soundbar volume. With this, I’m able to dump my old TV remote. Though it lacks an Input Change button, I have HDMI-CEC working so rarely do I need it.

#### The Problems
The casting feature on Roku is supported on some apps, but not as many as Chromecast. I did a quick test and found that casting works on Netflix, Youtube, Youtube TV, but not Hulu or Plex. It seems like a weird oversight as Roku can easily cast videos as Chromecast. There are times when I miss the casting to Chromecast. So I decided—why not use both? As both devices support HDMI-CEC, I don’t have to worry about switching TV inputs. Though if I’m paying for two devices, I should consider purchasing an Android TV like the Nvidia Shield TV.

#### Installation and Smart Home Integration
Roku is easily detected and automatically integrated with Home Assistant as a media player and remote. It offers full media controls, shows state information—like the currently playing app—but also has standard remote functions so you can create a Roku remote card like @iantrich. 

The Roku media player integration is sufficient for lighting automations, though I wish it could detect whether a video is playing or paused. Home Assistant can only detect whether you opened an app on the Roku. The media player status takes 2-3 seconds to update in Home Assistant.


![Google Assistant: Official Integration Works, though doesn’t offer a deep integration with apps like Youtube TV.](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1543622841706_google_assistant.jpg)
![Home Assistant: “Official” Integration  Roku devices are automatically detected if the HA discovery component is enabled.](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1550124719134_media_streaming-roku-ha.PNG)

![Roku App Standard remote interface, but als an option to play TV audio through phone’s headphone jack.](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1551461576379_media_streaming-roku-app01.jpg)
![Roku App Roku has a TV and movie content aggregated library for you  to browse, follow and watch on respective apps.](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1551461132223_media_streaming-roku-app.jpg)



### Chromecast
![](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1551462275089_chromecast_logo.png)

![Google Chromecast, 2nd Generation](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1546983628592_media_streaming-chromecast-photo.jpg)


Even though I use Chromecast in my home, I find it difficult to recommend as the sole media device in your home because it lacks a TV user interface and remote. I believe most people want a remote to browse videos, so I recommend trying a Roku, Android TV, or both Roku and Chromecast for these features. My roommates prefer to ignore the Chromecast altogether for the lack of a remote.


![Example of video thumbnails, but only works with Hulu and Youtube.](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1546977358256_tv_stick-chromecast-ha.gif)
![](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1546977277424_google_home_media_integration.png)


I initially liked the Chromecast because it would show video thumbnails on Home Assistant when watching Hulu and Youtube. I thought this feature worked on all apps, but further testing shows the feature doesn’t work on Netflix, Plex, or anything else. Casting from a web browser works, unlike my experiences with Miracast. 

#### Installation and Smart Home Integration
Out of all the devices I tested, Chromecast has the best integration with Home Assistant. Instant status updates, pause/play detection, episode details on Youtube and Hulu. Voice control on Chromecast is only useful for the deeper integration with Youtube TV, Netflix, HBO, Starz, or Viki, but not Hulu, Prime Video, Dramafever, or Vudu.

### Amazon Fire TV

![](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1546983454340_media_streaming-fire_tv-photo02.jpg)


If you’re using Amazon Echo and Alexa, then the Amazon Fire 4K TV sticks are hard to pass up for its low price, but the lack of Youtube support makes this a non-contender. Voice control is impressive, supporting Hulu and some other network TV apps — why can’t Chromecast support Hulu as well?

#### Installation and Smart Home Integration
Fire TVs are moderately difficult to setup in Home Assistant, requiring install of ADB and using command-line interface. Home Assistant integration is sufficient for lighting automations, though I wish it could detect whether a video is playing or paused — it only detects whether an app is opened. Player status takes 5 to 10 seconds to update in Home Assistant. There are also slight delays when sending pause/play commands from Home Assistant. Keep in mind, I tested a first generation Amazon Fire TV stick, which is the slowest Fire TV device.

#### Recommended Reading

- The Wirecutter’s Best Streaming Device Recommendation