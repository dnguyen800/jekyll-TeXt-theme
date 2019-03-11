---
layout: article
title: Music
category: media

---
## Music

**Published xx/xx/2019**

![](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1551248677440_music2.jpg)


**Competitors in this space:** Spotify, Plex, Pandora, Youtube Music, Tidal, Apple Music/iTunes, Google Play Music, Amazon Music, Volumio

I’ve personally tested the following:

- Spotify
- Plex
- Google Play Music

### Overview
Music is a big part of my life, and so I wanted it to be a major feature of my home. I love rummaging through my music collection, checking out the album covers and reading the liner notes. It spurs fond memories of how I discovered the artist, or how I felt when I listened to the album for the first time. With the help of a smart home, I wanted to recreate that nostalgic feeling in a digital form somehow, and have music playback be an integrated and seamless experience. It should be easy to find a song on any platform (phone, laptop, voice) and play on the speakers in the house. 

I love the current state of streaming music services—I can access music discographies from thousands of artists, and get music recommendations tailored to my listening habits. Although I no longer have any interesting recent memories of discovering music, I’ve been able to find so many new artists that I never would have found if I continued manually searching for music the old way. 

I do want to acknowledge my music listening past (including the good and bad artists) by having my CD and MP3 collection available to play on the speakers, so it was important to find a solution that can play both streaming and local music on my Chromecast built-in speakers. Luckily, those solutions exist now and are fantastic to use.

#### Considerations before purchasing a music subscription

- Most subscriptions offer a family plan that you can split among your household members. 

#### What you get with a music subscription

- A huge collection of music accessible through mobile app, web browser, and voice.

### Spotify
![](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1546739743915_music-spotify_logo.png)


For streaming music, Spotify is, without a doubt, the best offering not only for its catalog of music, but because it is the most openly supported music platform out there. Spotify works with voice assistants, web browsers, Android, iOS, and Amazon platforms—not many music services can make that claim.  Even open-source platforms like Home Assistant and Volumio can access the Spotify API to control playback like the official app.  For the music lover, the playlist curation and personalized music recommendations are so precise that Spotify can find a song I love from an artist or album I don’t like. 


![](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1546740051349_music-spotify-desktop_app.jpg)


Spotify supports all major multi-room audio formats: Chromecast Built-in, Amazon Echo, Sonos and Apple Airplay 2. Audio quality is respectable, using 320kbps Ogg Vorbis format (as long as the High Quality Streaming setting is enabled). That is the best quality you can get before going for lossless audio like FLAC, or Tidal’s lossless music service. 

#### The Problems
There are a few areas that Spotify falters: one is the lack of unofficial remixes and live sets that are somehow allowed on Youtube. The Spotify Windows app and Home Assistant doesn’t cast music to Chromecast speakers unfortunately. You will need to use the mobile app, a voice assistant or web browser to do that. Amazon Echo and other speakers supporting Spotify Connect work though, so it feels like this is an inherent limitation of Chromecast.

#### Installation and Smart Home Integration
Spotify is fully controllable in Home Assistant, but selecting a source doesn’t work. I haven’t found a way to play Spotify to a Chromecast speaker using Home Assistant.

Voice control works really well. I can ask to play a particular song, artist or one of my custom playlists.


![Voice Spotify works great with Google Assistant.](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1543622841706_google_assistant.jpg)
![Home Assistant: Unofficial Integration Integration is moderate difficulty. Requires a Spotify developer account and account authorization.](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1546746002013_music-spotify-ha.jpg)

![SmartThings:  SmartTings doesn’t have any media integrations](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1546628372929_not_available.png)
![Spotify App Works great](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1546762697472_music-spotify-app.png)


#### Recommended Reading

- Home Assistant Spotify component
- Spotify not supporting multroom audio with Echo.


### Plex
![](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1543699688630_plex-logo.png)


For local music, Plex is the best (and free!) app that can organize your music collection and offers the same functionality as popular music apps like Spotify.  Plex is accessible on web browsers, Xbox One, Playstation 4, Android, iOS, and Amazon platforms, and even remote access to your music isn’t too hard to set up. Chromecast multi-room audio is supported with Plex, but unfortunately Amazon, Sonos  and Apple’s multi-room audio solutions do not work yet. It sounds like I’m describing Spotify as Plex comes close to providing the same user-friendly experience, which is important to making music playback as easy as possible.


![Browsing by album feels just like any other music app.](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1543699822348_plex.jpg)


You will be surprised how hard it is to get a Spotify-like music experience for your local music. I tried open-source music players like Volumio, Mopidy, and PiMusicbox, but those tend to miss critical features—like a good search function or artist biographies—that keep it as a bare-bones app. It is amazing how the underlying parts (media scrapers, search, file support) of Plex work together to make a cohesive experience.


![Artist biographies in Plex. It’s fun to read about your favorite artists. Plex also shows similar artists, popular tracks—just like Spotify](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1546797253444_music-plex-app03.jpg)


Here’s a tip on bypassing Plex Pass restriction when watching videos and music on the phone. Normally, the Plex iOS and Android apps are time-restricted without Plex Pass, but if you cast the video or song to a Chromecast, the time limit is ignored.

#### The Problems
You will need a server or device running 24/7 to run the Plex Media Server. An Nvidia Shield TV or a spare laptop running Windows, Mac, or Linux make for excellent Plex servers. It’s possible to run Plex Media Server as a Hass.io add-on, but due to the restrictions of Hass.io and Docker, you can only store music on the SD card where Home Assistant is stored. I’m sure there is a way to connect a USB drive, but I’m not familiar with Docker to do so.

#### Installation and Smart Home Integration
Music players don’t integrate with SmartThings—that’s expected by now. Home Assistant integrates with Plex, though generate a permanent token requires running a Powershell script or Python script. I recommend using the temporary token outlined here and see if that works well enough. After getting the token, any device running the Plex app is treated as a media player in Home Assistant.

Voice control is more difficult on Google Assistant, though I think Amazon Alexa has an official integration with Plex. Getting Assistant to work requires installing a plug-in called Phlex and Cast.bundle.

Before using Plex, I recommend cleaning up your music collection first. That means converting CDs to the FLAC lossless format, fixing low-resolution cover art, standardizing artist and album names, fixing track numbers, and renaming files and folders. It’s a one-time effort to do over the weekend, but worth it to see the result—an immaculate, organized collection that is fun to browse through. I used Jriver Media Center to handle the CD ripping, metadata scraping, and file/folder renaming. A free 30-day trial is available, which should be enough time to perform the cleanup.


![Voice: Unofficial integration Very difficult. Requires an add-on called Phlex and Cast.bundle to get it working with Google Assistant. Requires exposing HA to the internet. Best to wait for an official integration.](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1543622841706_google_assistant.jpg)
![Home Assistant: Unofficial Integration Moderately difficult—HA autodetects server but requires getting a temp token. Cover art doesn’t load. Getting a permanent token is more difficult.](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1546627737256_music-plex-ha.PNG)

![SmartThings:  SmartTings doesn’t have any media integrations](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1546628372929_not_available.png)
![Plex App Simple, and easy-to-use.](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1546446928750_music-plex_app.png)


#### Recommended Reading

- Plex Media Server can be installed on a Windows, Mac or Linux device
- Plex Media Server hass.io addon if you want to run the server on a Raspberry Pi with Home Assistant. There are storage limitations as you cannot connect external devices to Hass.io.
- Phlex Hass.io addon adds Google Assistant capabilities to Plex. Requires the Cast.bundle Plex addon to be installed.
- Python script to generate a permanent token from Plex. Was originally posted on the Plex forum.