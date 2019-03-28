---
layout: article
title: Streaming Media Services
short_title: Streaming Media Services
excerpt: Music, video, blah blah blah.
category: [media, home automation]
permalink: /media/streaming-media-services
key: media-streaming_media_services
aside:
  toc: true
banner: assets/images/overlay/music.jpg
mode: immersive
header:
  theme: dark
article_header:
  type: overlay
  theme: dark
  background_color: '#203028'
  background_image:
    gradient: 'linear-gradient(135deg, rgba(34, 139, 87 , .4), rgba(139, 34, 139, .4))'
    src: /assets/images/overlay/music.jpg

---

<!--more-->
<figcaption><b>Image:</b><a href="https://www.freestocks.org"> freestocks.org</a></figcaption>


**Quick Links:**
<div class="grid-container">
  <div class="grid grid--p-2">
    <div class="cell cell--3"><a href="/media/streaming-media-services#music"><div><div class="card">
      <div class="card__image">
        <img class="image" src="/assets/images/grid/music.jpg"  />
      </div>
    </div></div></a></div>
    <div class="cell cell--3"><a href="/media/streaming-media-services#live-tv-providers"><div><div class="card">
      <div class="card__image">
        <img class="image" src="/assets/images/grid/live-tv-provider.jpg"/>
      </div>
    </div></div></a></div>
  </div>
</div>

# Music

**Competitors in this space:** Spotify, Plex, Pandora, Youtube Music, Tidal, Apple Music/iTunes, Google Play Music, Amazon Music, Volumio

I’ve personally tested the following:

|---
| ![](\assets\images\logo\spotify.png){:.image--md} |  ![](\assets\images\logo\plex.png){:.image--md} | ![](\assets\images\logo\google-play-music.png){:.image--md} | ![](\assets\images\logo\volumio.png){:.image--md} | ![](\assets\images\logo\mopidy.png){:.image--md}
|:-:|:-:|:-:|:-:|:-:
| | | | |

![](\assets\images\logo\spotify.png){:.image--md}   ![](\assets\images\logo\plex.png){:.image--md}  ![](\assets\images\logo\google-play-music.png){:.image--md}  ![](\assets\images\logo\volumio.png){:.image--md}  ![](\assets\images\logo\mopidy.png){:.image--md}

### What you need to know

Music is a big part of my life, and so I wanted it to be a major feature of my home. I love rummaging through my music collection, checking out the album covers and reading the liner notes. It spurs fond memories of how I discovered the artist, or how I felt when I listened to the album for the first time. With the help of a smart home, I wanted to recreate that nostalgic feeling in a digital form somehow, and have music playback be an integrated and seamless experience. It should be easy to find a song on any platform (phone, laptop, voice) and play on the speakers in the house. 

I love the current state of streaming music services—I can access music discographies from thousands of artists, and get music recommendations tailored to my listening habits. Although I no longer have any interesting recent memories of discovering music, I’ve been able to find so many new artists that I never would have found if I continued manually searching for music the old way. 

I do want to acknowledge my music listening past (including the good and bad artists) by having my CD and MP3 collection available to play on the speakers, so it was important to find a solution that can play both streaming and local music on my Chromecast built-in speakers. Luckily, those solutions exist now and are fantastic to use.

### Considerations before purchasing a music subscription

> - Most subscriptions offer a family plan that you can split among your household members. 

### What you get with a music subscription

> - A huge collection of music accessible through mobile app, web browser, and voice control.

### Recommended Reading

> - Home Assistant Spotify component
> - Spotify not supporting multroom audio with Echo.
> - Plex Media Server can be installed on a Windows, Mac or Linux device
> - Plex Media Server hass.io addon if you want to run the server on a Raspberry Pi with Home Assistant. There are storage limitations as you cannot connect external devices to Hass.io.
> - Phlex Hass.io addon adds Google Assistant capabilities to Plex. Requires the Cast.bundle Plex addon to be installed.
> - Python script to generate a permanent token from Plex. Was originally posted on the Plex forum.
- [How to generate a temporary token for Plex.](https://forums.plex.tv/t/how-to-request-a-x-plex-token-token-for-your-app/84551)


## Spotify
![](\assets\images\logo\spotify.png){:.image--xl.align-left}

**For streaming music, Spotify is, without a doubt, the best offering not only for its catalog of music, but because it is the most openly supported music platform out there.** Spotify works with voice assistants, web browsers, Android, iOS, and Amazon platforms—not many music services can make that claim.  Even open-source platforms like Home Assistant and Volumio can access the Spotify API to control playback like the official app.  For the music lover, the playlist curation and personalized music recommendations are so precise that Spotify can find a song I love from an artist or album I don’t like. 

<figure style="width: 100%;" >
 <img src="\assets\images\other\spotify-desktop.jpg" alt="" />
 <figcaption>
A view of the Spotify desktop app for Windows.
 </figcaption>
</figure>

Spotify supports all major multi-room audio formats: Chromecast Built-in, Amazon Echo, Sonos and Apple Airplay 2. Audio quality is respectable, using 320kbps Ogg Vorbis format (as long as the High Quality Streaming setting is enabled). That is the best quality you can get before going for lossless audio like FLAC, or Tidal’s lossless music service. 

### The Problems

There are a few areas that Spotify falters: one is the lack of unofficial remixes and live sets that are somehow allowed on Youtube. The Spotify Windows app and Home Assistant cannot cast music to Chromecast speakers directly. You will need to use the mobile app, a voice assistant or web browser to do that. Amazon Echo and other speakers supporting Spotify Connect work, so this is likely an inherent limitation of Chromecast.

### Installation and Smart Home Integration

Spotify is fully controllable in Home Assistant, though selecting a speaker source doesn’t work. I haven’t found a way to play Spotify to a Chromecast speaker using Home Assistant.

Voice control works really well. I can ask to play a particular song, artist or one of my custom playlists.


<figure class="figure figure--50">
 <img src="/assets/images/integrations/spotify-ha.png" alt="Small picture of a kitten" />
 <figcaption>
  <b>Home Assistant: Good</b><br>Several steps requiring developer account, edit config file, browser authorization.
 </figcaption>
</figure>
<figure class="figure figure--50">
 <img src="/assets/images/integrations/google-home.png" alt="Small picture of a kitten" style="width: 100%" />
 <figcaption>
 <b>Voice: Great</b><br>Spotify works perfectly with Google Assistant.
 </figcaption>
</figure>
<figure class="figure figure--50">
 <img src="/assets/images/integrations/na.png" alt="Small picture of a kitten" style="width: 100%" />
 <figcaption>
 <b>SmartThings: None</b><br> Integration does not exist.
 </figcaption>
</figure>
<figure class="figure figure--50">
 <img src="/assets/images/integrations/spotify-app.png" alt="Small picture of a kitten" style="width: 100%" />
 <figcaption>
 <b>Native App: Great</b><br>Amazing!
 </figcaption>
</figure>

## Plex
![](\assets\images\logo\plex.png){:.image--xl.align-left}

**For local music, Plex is the best (and free!) app that can organize your music collection and offers the same functionality as popular music apps like Spotify.**  Plex is accessible on web browsers, Xbox One, Playstation 4, Android, iOS, and Amazon platforms, and even remote access to your music isn’t too hard to set up. Chromecast multi-room audio is supported with Plex, but unfortunately Amazon, Sonos  and Apple’s multi-room audio solutions do not work yet. It sounds like I’m describing Spotify as Plex comes close to providing the same user-friendly experience, which is important to making music playback as easy as possible.

<figure style="width: 100%;" >
 <img src="\assets\images\other\plex-app.jpg" alt="" />
 <figcaption>
A view of the Plex app through any web browser.
 </figcaption>
</figure>

You will be surprised how hard it is to get a Spotify-like music experience for your local music. I tried open-source music players like Volumio, Mopidy, and PiMusicbox, but those tend to miss critical features—like a good search function or artist biographies—that keep it as a bare-bones app. It is amazing how the underlying parts (media scrapers, search, file support) of Plex work together to make a cohesive experience.

<figure style="width: 100%;" >
 <img src="\assets\images\other\plex-app02.jpg" alt="" />
 <figcaption>
Artist biographies in Plex. It’s fun to read about your favorite artists. Plex also shows similar artists, popular tracks—just like Spotify.
 </figcaption>
</figure>

{:.info}
**Here’s a tip on bypassing Plex Pass restriction when watching videos and music on the phone:** normally, the Plex iOS and Android apps are time-restricted one minute without Plex Pass, but if you play the video or song to a Chromecast, the time limit is ignored.

### The Problems

You will need a server or device running 24/7 to run the Plex Media Server. An Nvidia Shield TV or a spare laptop running Windows, Mac, or Linux make for excellent Plex servers. It’s possible to run Plex Media Server on a Raspberry Pi as a Hass.io add-on, but due to the restrictions of Hass.io and Docker, you can only store music on the SD card where Home Assistant is stored. I’m sure there is a way to connect a USB drive, but I’m not familiar with Docker to do so.

### Installation and Smart Home Integration

Music players don’t integrate with SmartThings—that’s expected by now. Home Assistant integrates with Plex but requires an authentication token to connect. I recommend using the temporary token outlined [here](https://forums.plex.tv/t/how-to-request-a-x-plex-token-token-for-your-app/84551) and see if that works well enough. After getting the token, any device running the Plex app is treated as a media player in Home Assistant.

Voice control is more difficult on Google Assistant, though I think Amazon Alexa has an official integration with Plex. Getting Assistant to work requires installing a plug-in called Phlex and Cast.bundle. I would take some time to install it, so I couldn't do it at the time of this writing.

<figure style="width: 100%;" >
 <img src="\assets\images\other\jriver-app.jpg" alt="" />
 <figcaption>
Jriver Media Center has an extensible set of tools to clean up metadata and cover art.
 </figcaption>
</figure>

Before using Plex, I recommend cleaning up your music collection first. That means converting CDs to the FLAC lossless format, fixing any low-resolution cover art, standardizing artist and album names, fixing track numbers, and renaming files and folders. It’s a one-time effort to do over the weekend, but worth it to see the result—an immaculate, organized collection that is fun to browse through. I used Jriver Media Center to handle the CD ripping, metadata scraping, and file/folder renaming. A free 30-day trial is available, which should be enough time to perform the cleanup.


<figure class="figure figure--50">
 <img src="/assets/images/integrations/plex-ha.png" alt="Small picture of a kitten" />
 <figcaption>
 <b>Home Assistant: Difficult</b><br>Requires obtaining a temp token. Cover art doesn’t load.
 </figcaption>
</figure>

<figure class="figure figure--50">
 <img src="/assets/images/integrations/google-home.png" alt="Small picture of a kitten" style="width: 100%" />
 <figcaption>
 <b>Voice: Difficult</b><br>Requires Phlex and Cast.bundle add-ons to work with Google Assistant. Must expose HA to the internet.
 </figcaption>
</figure>

<figure class="figure figure--50">
 <img src="/assets/images/integrations/na.png" alt="Small picture of a kitten" style="width: 100%; height: 100%" />
 <figcaption>
 <b>SmartThings: None</b><br> Integration does not exist.
 </figcaption>
</figure>

<figure class="figure figure--50">
 <img src="/assets/images/integrations/plex-app.png" alt="Small picture of a kitten" style="width: 100%" />
 <figcaption>
 <b>Native App: Great</b><br> Simple, and easy-to-use.
 </figcaption>
</figure>


## The Competition
![Google Play Music logo](\assets\images\logo\google-play-music.png){:.image--xl.align-left}

Google Play Music was my alternate method to paying my local music collection. It's not technically playing music locally, as I first needed to upload my 80 gigabyte music collection to Google's servers and sync it thereafter. An Google Play agent application exists to monitor folders and upload new tracks. 

Play Music mobile app works, though  navigation is annoying as the app is constantly pointing you towards streaming radio and eventually some form of paid music subscription. 

There are limitations on the number of times you can download your entire collection. And the number of devices you can stream your music from. We also don't know if Google will shut down the service at some point. Google is well known for this. Youtube paid content is going away. It's very much possible since Google doesn't get any money from this service and it's ~a liability to host all this music, obtained through legal and unlegal ways.. Amazon Music also canceld their local music service.


![Volumio logo](\assets\images\logo\volumio.png){:.image--xl.align-left}

Volumio is very well polished open-source product out of the box. Easy to flash an image and install on SD card. really nice default skin. Spotify plugin availabale to access Spotify music and local music in one interface. But Volumio focuses on being a hi-fi music player/amp for a single pair of speakers, not versastile.. You connect an inexpensive DAC to the Pi. Doesn't offer Chromecast (though it's open-source, so anything is possible in the future). 

The menu stuff is pretty basic. No artist biographies, related music and artists. Not that fun to browse through, no learning. Mobile app exists and the skin looks professional. Home Assistant integration exists and works well. Not sure if cover art shows.

Volumio didn't fit my needs, but I still think it's a solid application that might be useful for others who want a high fidelity music solution in their smart home.

![Mopidy logo](\assets\images\logo\mopidy.png){:.image--xl.align-left}

I used Mopidy for some time before realizing Plex does everything I needed, but better. 

It's open-source. Quite barebones but several plugins and themes make it look really presentable. 

There is a way to stream to Chromecast speakers. But there is about a 5-second delay, and there's issues skipping songs, choosing new songs, and the sound quality is worse. Basicallt Mopidy is streaming output to an Ogg Vorbis file, and you send the URL of the file to the Chromecast to play.

There is a mobile app but it's very basic and no skins.

For some reason, I never got the music to play through my web browser. Annoyed the heck out of me

# Live TV Providers

**Competitors in this space:** Youtube TV, Playstation Vue, Hulu Live, Sling TV, Philo, OTA local channels

I’ve personally  tested the following:

![](\assets\images\logo\youtubetv.png){:.image--md}  ![](\assets\images\logo\slingtv.png){:.image--md}  ![](\assets\images\logo\hdhomerun.png){:.image--md}

### What you need to know

If you came here hoping for a way to integrate your Xfinity, Verizon, or Dish Network TV receivers with Home Assistant or Amazon Alexa, then you’re out of luck! Those are closed ecosystems and you’re stuck with whatever features they offer. To be fair, the Xfinity app has improved and the Xfinity remote’s voice feature worked well during the times I tried it. If you absolutely refuse to cut the cord with cable TV, then the Logitech Harmony remote can add some voice control and Home Assistant integration, but requires a lot of testing to get it right. To be honest, I haven’t found a reason to use my voice to watch live TV and prefer using a remote to browse through the TV guide or recordings. So you’re not missing much by not integrating.


There are a growing number of video streaming services that offer live local TV and select premium channels for a lower price and no contracts. These integrate services better with voice assistants and Home Assistant by association of the Rokus, Chromecasts and Fire TVs it supports. So lets review one of these services!

### Considerations Before Purchasing an Internet TV Subscription

> - **Do you really need another subscription that you may not use?** Consider subscribing and canceling when your TV show’s season is over.
> - **Check your internet provider’s internet speed and bandwidth caps.** Your TV watching habits may disrupt another’s video gaming session or exceed bandwidth caps.

### What You Get With an Internet TV Subscription

> - **With Youtube TV, share the subscription with five others in your Google Family.** You can only change families once a year, and can’t be in more than one family. Geographic restrictions also apply, though in my testing, Bay Area region is fine.
> - **Watch TV on the go with your phone, even when traveling across states.** Eventually these apps block local TV access if it detects you’ve been living in a different area for months.

### Recommended Reading

> - Youtube TV official site
> - Using Google Assistant on Youtube TV with Chromecast [article](https://support.google.com/youtubetv/answer/7529864?hl=en)


## Youtube TV
![](\assets\images\logo\youtubetv.png){:.image--xl.align-left} 

**I tested Youtube TV earlier, and it provides a solid TV viewing experience as well as some useful smart home features, like advanced voice control with Google Assistant.**  Like any good streaming service, Youtube TV supports playback on web browsers, Chromecast, Roku, Apple TV, and most new TVs (2016 models or later). Streaming starts within seconds without any noticeable lag or dropouts, even when watching live sports. The experience convinced me that streaming live TV doesn’t have to suck, unlike my experience with Sling TV.

Voice commands with Google Assistant work really well on Youtube TV (naturally), but only when using Chromecast. Saying “play the latest episode of Conan” works as expected on my Chromecast Ultra, but not on Roku. The most I can do with my voice is say “open Youtube TV on Roku,” which is not all that useful.

{:.info}
**Did you know...**
Youtube TV also has a generous family sharing option, allowing up to five additional members to have their own Youtube TV account, with three simultaneous streams each. There are certain limitations, like members can switch families only once a year, you can’t join more than one family. and members should be within a geographic range (unconfirmed as to the range). 

<figure style="width: 100%;" >
 <img src="\assets\images\other\tv_sub-youtube_tv-app.jpg" alt="" />
 <figcaption>
 The Youtube TV app on Android.
 </figcaption>
</figure>

### The Problems
There are some annoyances worth noting before signing up for Youtube TV. Sadly, due to feud between Google and Amazon, Youtube TV does not work with Amazon Fire TV or tablets. Unofficial installation methods exist, but are likely to stop working in a few months whenever an app update is required. 

Secondly, finding and favoriting TV shows should be easy, but the app separates on-demand and broadcast shows, meaning you can’t browse through all of FX’s catalog in one spot. In some cases, I had to search for specific TV shows, like TBS’ Miracle Workers, in order to record them. I’m not able to bookmark Mr. Robot either, at least not until after the season premiere occurs. I also noticed the selection of episodes available on demand fluctuates, much to my annoyance. The shows Angie Tribeca and Final Space on TBS  tends to flip between the first and second half of the latest season every few weeks.

### Installation and Smart Home Integration

<figure class="figure figure--50">
 <img src="/assets/images/integrations/youtubetv-ha.png" alt="Small picture of a kitten" />
 <figcaption>
 <b>Home Assistant: None</b><br>Works as long as the media player works with HA.
 </figcaption>
</figure>

<figure class="figure figure--50">
 <img src="/assets/images/integrations/google-home.png" alt="Small picture of a kitten" style="width: 100%" />
 <figcaption>
 <b>Voice: Good</b><br>Supports deep integration if using a Chromecast and Google Assistant. Not so good with Roku and Google Assistant.
 </figcaption>
</figure>

<figure class="figure figure--50">
 <img src="/assets/images/integrations/na.png" alt="Small picture of a kitten" style="width: 100%; height: 100%" />
 <figcaption>
 <b>SmartThings: None</b><br> Integration does not exist.
 </figcaption>
</figure>

<figure class="figure figure--50">
 <img src="/assets/images/integrations/youtubetv-app.png" alt="Small picture of a kitten" style="width: 100%" />
 <figcaption>
 <b>Native App: Great</b><br> Simple, and easy-to-use.
 </figcaption>
</figure>