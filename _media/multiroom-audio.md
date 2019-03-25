---
layout: article
title: Multi-room Audio
short_title: Multi-room Audio
excerpt: Previously limited as a wired solution, multi-room audio is now achievable using wireless speakers.
category: [media, home automation]
permalink: /media/multiroom-audio
key: media-multiroom_audio
aside:
  toc: true
banner: assets/images/overlay/multiroom-audio.jpg
mode: immersive
header:
  theme: dark
article_header:
  type: overlay
  theme: dark
  background_color: '#203028'
  background_image:
    gradient: 'linear-gradient(135deg, rgba(34, 139, 87 , .4), rgba(139, 34, 139, .4))'
    src: /assets/images/overlay/multiroom-audio.jpg

---

**Competitors in this space:** Google Home/Chromecast, Amazon Echo, Sonos One, Apple Homepod, Denon Heos, and wired solutions


I’ve personally tested the following:

| Chromecast Built-in Speakers (Google, Polk, Insignia, Lenovo) | Amazon Echo (1st gen), Echo Dot |
|:-------:|:--------:|:---------:|
| ![Google Home](\assets\images\product-photo\google-home.jpg){:.image--sm} ![Insignia Speaker](\assets\images\product-photo\insignia-speaker.jpg){:.image--sm} ![Polk Magnifi Mini](\assets\images\product-photo\polk-magnifi-mini.jpg){:.image--md} | ![Amazon Echo photo](\assets\images\product-photo\amazon-echo-1st.jpg){:.image--md}![Amazon Echo Dot](\assets\images\product-photo\amazon-echo-dot-2nd.jpg){:.image--md} |

## What you need to know
Multi-room audio is the ability to play music synchronized with speakers placed around the house to achieve the effect of music following you around the house. It works really well and is one of my favorite uses in a smart home.  What is great about the solution is that the speakers are wireless, so it’s possible to have a clean audio setup in a rented apartment or house. 



### Considerations before choosing multi-room audio speakers

> - **Research app compatibility with multi-room audio before buying.** Chromecast supports the most services. Amazon Echo and Sonos doesn’t support Plex for local music.



### What you get with a multi-room audio speakers

> - Synchronized music in every room.
> - Continue the music playing from your car to the house.
> - Start playing multi-room music using your voice or music app.
> - Depending on your choice, works with most major music apps.

### Recommended Reading

> - [Insignia Large speaker with Google Assistant](https://www.bestbuy.com/site/insignia-voice-smart-portable-bluetooth-speaker-and-alarm-clock-with-google-assistant-gray-black/5865906.p?skuId=5865906)
> - [Slickdeals.net sales of Insignia speakers](https://slickdeals.net/newsearch.php?searchin=first&forumchoice%5B%5D=9&forumchoice%5B%5D=44&forumchoice%5B%5D=25&forumchoice%5B%5D=30&q=insignia+speaker+google+assistant&r=1)
> - [Wirecutter review](https://thewirecutter.com/reviews/best-soundbar/#budget-pick-vizio-sb3651-e6) of the Vizio Smartcast Soundbar


## Chromecast Built-in Speakers

![Chromecast Built-in](\assets\images\logo\chromecast-builtin.png){:.image--xl}

**With a wide selection of reasonably priced compatible AV receivers, speakers and soundbars to choose from, I recommend using any highly rated Chromecast built-in speaker in your home.** If you already have a good pair of speakers, then connect a Chromecast Audio (discontinued as of Jan 2019) to it. There are so many combinations of Chromecasts you can use—even the Chromecast TV dongles work with multi-room audio now, allowing you to leverage your existing TV, receiver and soundbars.  Any speaker that supports Chromecast Built-in will have the same easy setup experience and compatibility with apps that support Chromecast. 


The main selling point of Chromecast is the number of apps that support it. Where else can you find Chromecast multi-room audio support from a nearly dead service like SoundCloud? Chromecast is the only solution I’ve found that can stream multi-room audio from Plex for local music. Last I checked, Amazon Echo and Sonos support Plex but for individual speakers only.


### The Problems

I’ve found Chromecast to be a more frustrating user experience than Amazon Echo—music playback can take a few seconds to start, or not start at all until I force close and re-open the Spotify app. This happens on both iOS and Android apps quite often. Luckily, I haven't had any troubles getting music to play using voice control.

Is that the price to pay for compatibility? Unfortunately, yes. I’m able to live with that trade-off for more supported music apps, but it is one of the biggest annoyances with this setup.  


### Installation and Smart Home Integration

After setting up  the speakers in the Google Home app, create a speaker group in the Google Home app and that’s it--you can access your speaker group in Spotify, Plex, or anything else that supports Chromecast speakers.

![Chromecast Setup](\assets\images\other\chromecast-setup.png)

Home Assistant detects individual Chromecast speakers and speaker groups if the ``Discovery`` component is enabled. I use the ``Universal Media Player component`` to combine all speakers and groups into one Home Assistant entity and show the music currently playing. 

One small quirk I found is that if you want send a broadcast message to all speakers using Home Assistant, you must use a Home Assistant group (not Google). As long as you are not constantly renaming your speakers in Google Home, this shouldn't be a problem. 

Voice control with Google Assistant works great with Spotify. Mention the name of the speaker group and Google will play music there.

#### Integrations 

<figure style="float: left; width: 25%; text-align: center; font-size: smaller; text-indent: 0; padding: 0.5em; border: thin silver solid;" >
 <img src="/assets/images/integrations/chromecast-ha.png" alt="Small picture of a kitten" />
 <figcaption>
 <b>Home Assistant: Great</b><br>  Autodetects speakers and displays media info like so.
 </figcaption>
</figure>

<figure style="float: left; width: 25%; text-align: center; font-size: smaller; text-indent: 0;  padding: 0.5em; border: thin silver solid; " >
 <img src="/assets/images/integrations/google-home.png" alt="Small picture of a kitten" style="width: 100%" />
 <figcaption>
 <b>Voice: Great</b><br> Say "Hey Google, play Spotify on "speaker group" and it works.
 </figcaption>
</figure>

<figure style="float: left; width: 25%; text-align: center; font-size: smaller; text-indent: 0;  padding: 0.5em; border: thin silver solid;" >
 <img src="/assets/images/integrations/chromecast-spotify.png" alt="Small picture of a kitten" style="width: 100%; height: 100%" />
 <figcaption>
 <b>Spotify: Okay</b><br> Sometimes need to force close the app to work.
 </figcaption>
</figure>

<figure style="float: left; width: 25%; text-align: center; font-size: smaller; text-indent: 0; padding: 0.5em; border: thin silver solid;" >
 <img src="/assets/images/integrations/chromecast-app.png" alt="Small picture of a kitten" style="width: 100%" />
 <figcaption>
 <b>Native App: Good</b><br> Control settings, volume and media playback from the app.
 </figcaption>
</figure>


## Insignia Large Speaker with Google Assistant

 ![Insignia Speaker](\assets\images\product-photo\insignia-speaker.jpg){:.image--md.align-left}

**For those who want multi-room audio without breaking the bank, the Insignia Large Speaker with Google Assistant from Best Buy is a good value when it goes on sale for $35.**  It sounds better than the Google Home speakers, and has a few nifty features like 3-hour battery, and a LED display to show the time and temperature. I was able to outfit my home with these speakers for under $200! This is more of a brag than recommendation since the sale is over, but do check Slickdeals periodically if it appears again. There is one big problem with these speakers, which I will go into detail below.



### The Problems

I’ve tested these speakers thoroughly for months now, and they’re great, except for one significant issue. The sound cuts off when playing low-sounding music — it’s especially noticeable on classical, piano, or acoustic songs. The problem fades away by increasing the volume, but listening to classical volume at high volume is a bit of an oxymoron. Firmware updates haven’t resolved the issue, so it’s likely to be a hardware issue that may never be resolved.



## Vizio Smartcast Sound Bar
![Vizio Sound Bar photo](\assets\images\product-photo\vizio-soundbar.jpg){:.image--md.align-left}

**For Chromecast Built-in sound bars, the** [**Vizio Smartcast sound bars**](https://www.target.com/p/vizio-36-5-1-sound-bar-system-black-sb3651-e6/-/A-17303189?clkid=1804d4c5Nd57efb2578d34dbc8b903993&lnm=81938&afid=Skimbit%20Ltd.&ref=tgt_adv_xasd0002) **are considered the best value**. [The Wirecutter](https://thewirecutter.com/reviews/best-soundbar/#budget-pick-vizio-sb3651-e6) recommends them for the best mix of performance, connectivity, features, and price in the budget category. I tested another soundbar, the [Polk Magnifi Mini](https://www.amazon.com/Polk-Audio-MagniFi-Theater-System/dp/B01LW76AKC/ref=sr_1_3?ie=UTF8&qid=1546626122&sr=8-3&keywords=polk+magnifi+mini), and found the Chromecast integration working as expected, but the trade-off of sound quality for the smaller size was not worth it. 






## The Competition
### Sonos
![Sonos photo](\assets\images\product-photo\sonos-one.jpg){:.image--md.align-left}

I don’t own any Sonos products because I’m happy (for now) with my cheap Chromecast Built-in speakers, but if I were willing to spend over $1,000 then I would look into getting Sonos One speakers and a sound bar for my setup. The sound quality is likely better than Chromecast speakers and Amazon Echo, though the voice assistant function is either bad or non-existent. Check out Amazon reviews to get an idea of the complaints. I'm going to assume that Sonos makes a good speaker but a terrible voice assistant, which that may be acceptable to those who don’t want a speaker listening in at all times.

### Amazon Echo
![Amazon Echo photo](\assets\images\product-photo\amazon-echo-1st.jpg){:.image--md.align-left}

I think Amazon Echo's multi-room music feature works much better than Chromecast, but it only works with Spotify, Amazon Music Unlimited, TuneIn, iHeartRadio and Pandora. It doesn't support Plex for local music, so I couldn't use it with my solution. 

.

.

.