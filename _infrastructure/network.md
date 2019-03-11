---
layout: article
title: Network / Internet
category: infrastructure
mode: immersive
header:
  theme: dark
article_header:
  type: cover
  image:
    src: /docs/assets/images/banners/network.jpg
---

## Internet, Network, Wireless Infrastructure

**Published xx/xx/2019**
**Competitors in this space:** Google, Eero, Ubiquiti, Netgear, Linksys, Asus, Plume, TP-Link

I’ve personally tested the following:

- Google Wifi (one Google Wifi point and TP-Link Onhub AC1900 as Wi-Fi mesh)
- Amplifi HD AFI-R (two linked as WiFi mesh and wired backhaul)
- T-Mobile/ASUS TM-AC1900 router

### Overview
When I added a few cameras, tablets, smart speakers, and media streaming devices to the house, my network router nearly died from the overload. Websites took longer to load, devices stopped responding, and eventually the wireless network went offline. I knew I would have more issues down the line until I changed the router, so I started looking into the latest tech—Wi-Fi mesh systems. 

Sidenote: For advanced networking users who want features like VPN and VLAN, I would suggest Ubiquiti’s lineup of routers, wireless APs and switches. Before purchasing, you need to decide whether you need managed network switches for VLANs and Power-over-Ethernet (PoE) to connect wired cameras and access points (AP) all around the house. If you want both, then it will cost you — an 8-port managed network switch with PoE sells for $200. 

Tom’s Guide offers a good primer on Wi-Fi mesh technology, but essentially Wi-Fi mesh offers improved wireless range and speed, easy network management, streamlined connections, and tighter security. Having unsuccessfully tried alternatives like wireless repeaters, powerline and MoCA adapters, I highly recommend Wi-Fi mesh systems to anyone who wants to spend less time rebooting and troubleshooting routers. The high cost was initially an issue, but Google Wifi and other mid-range mesh systems can be purchased for $200 or so, making it an easier to recommend.

No matter what product you choose, be sure to thoroughly test the system for issues. That means connect as many devices as you can and start watching videos on multiple devices. Turn on every feature you plan to use—like static IP addresses, VPN and guest network. Every system has problems and the same goes for my recommendation—there isn’t a router that meets everyone’s needs.  

Also make sure to buy the right product, as companies are releasing a confusing amount of SKUs to take advantage of brand recognition and consumer confusion. Not all Netgear Orbis are created equal—without proper research, you could be paying a high price for a low-end product. The Wirecutter’s Wi-Fi mesh system recommendations are listed by model number and also suggests avoiding certain SKUs that are underpowered. 

To get a sense of the SKU confusion, here is a list of products currently available from each major company. I won't bother explaining the differences—it's better to do your own research. 

Google Wifi: Google Wifi point
Netgear Orbi: RBK53, RBK50, RBK44, RBK40, RBK33, RBK30, RBK23W, RBK22, RBK20W
Linksys Velop: AC6600, AC4800, AC4400, AC3900, AC3600, AC2600, AC2200, AC1300
Ubiquiti Amplifi: Amplifi HD routers, Amplifi mesh points, Amplifi Instant

#### Considerations before buying a Wi-Fi mesh system

- Know the model # that fits your needs—don’t just buy based on brand alone.
- What is more important—speed or reliability? Household that watch multiple 4K video streams and have gigabit internet should consider faster but less reliable systems  like Netgear Orbi.
- Test the router thoroughly as it’s impossible to guarantee everything will work with your mix of devices.

#### What You Get With a Wi-Fi mesh system

- An easy to use interface to manage the network. Usually through a phone app, that can remotely access the network.
- Increased wireless coverage and speed through Wi-Fi mesh, hard-wired APs, or faster routers.
- Support a greater number of wired and wireless devices on the network.

### Google Wifi
![](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1551230652581_google_wifi_logo.png)
![Image: Google](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1545414049139_google_wifi.jpeg)


**If you want a hassle-free WiFi mesh system with decent set of features, go with Google Wifi. ** It is not the fastest Wi-Fi mesh system, but the reliability of Google Wifi convinced me to buy one. It is incredibly easy to setup and manage the network using the Google Wifi app, as you would expect from Google. No more clunky web interfaces here—routers finally feel like the modern connected devices they should be.  Security updates are frequent, though new features are rare or nonexistent for a two year-old product. That’s fine with me—I’ll trade reliability for features, since features are meaningless if it doesn’t work properly. 

Another unique feature of Google Wifi is that each wifi point acts as a standalone router, meaning you can buy a multi-pack and split it among friends. In my case, I only needed two points, so I bought a 4-pack from Costco and sold two to my friends. I paid only $150 for a basic Wi-Fi mesh system that I could easily expand buy purchasing another point. Hooray for scalability!


![](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1546274366130_google_wifi_app.png)


#### The Problems
That said, I’m disappointed that I’ve run into some issues with Google Wifi. I had to reboot and reconnect the wifi points to the network once a month. I believe the cause is the refurb Onhub Google router I’m using, which has been exhibiting other problems with it, like a dead ethernet port.

To Google’s credit, every issue was easily resolved through the app—I even fixed the issue while I was away from the house. Still, I wish this system was a set-and-forget-it type solution, but I haven’t found the answer, yet.

Not everyone prefers Google Wifi as its simplicity means less control in some cases. I’ve run into issues that could have been resolved if Google Wifi had the following features: 


- Wifi speeds are not sufficient to utilize gigabit internet. Best to go with Netgear Orbi or wired access points if the fastest speeds are important.
- Wifi band steering cannot be disabled, meaning the router determines which Wi-Fi band (2.4  5ghz) is best, when sometimes it isn’t. 
- VLAN is not supported, but most consumer routers don’t have this feature unfortunately.
- Cannot disable internet connectivity on a per device basis.  Family Wifi Pause feature exists, but blocks local and internet access.

#### Recommended Reading

- Search Slickdeals to find the router on sale
- Google Wifi subreddit


### Amplifi HD
![](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1551235939534_amplifi_logo.png)
![Image: Amplifi](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1551235949962_amplifi.png)


**If you want faster wifi speed and reliability, consider purchasing two Amplifi HD routers to form a WiFi mesh system. **It is more expensive than Google Wifi and sales are infrequent, but I have personally used it for the past year and found it to be solid. Setup and maintenance is almost as easy as Google Wifi, though tasks like assigning static IP addresses will reset the router on each assignment.  When you’re assigning addresses to over twenty devices, the waiting can be tedious. Using as a single router, the Amplifi HD’s Wi-Fi performance is worse than my Netgear R7000, but as a WiFi mesh system with wired backhaul, all my devices connect without a problem.

Amplifi routers are made by Ubiquiti, a trusted company that has provided quality professional-level network gear under the Unifi name for several years now. Security updates and useful features like wired backhaul have been rolling out for the past two years, so the support is still active. I haven’t seen any major complaints or issues on the r/Amplifi subreddit either.

At this price range ($250-350), you are encroaching on Netgear Orbi’s territory, which the RBK50 is the top performer to beat. I hesitate recommending Netgear because of my past bad experiences with their firmware and their confusing product line (9 different Orbis? Why?), despite Wirecutter’s recommendation. I can only point to the Netgear Orbi forums to show the little faith that consumers have in Netgear’s firmware.

#### Recommended Reading

- Search Slickdeals to find the router on sale
- Amplifi subreddit for detailed discussions


### Asus TM-AC1900
![](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1551236456687_asus_logo.png)
![Image: Asus](https://d2mxuefqeaa7sj.cloudfront.net/s_6F2D06D13ED5B646A7B3ABF92554F4B018DC3C58310A9D7A5EC1772E423FF837_1545418132251_tmobile_router2.jpg)


**For the budget-conscious who doesn’t mind taking a gamble, the T-Mobile TM-AC1900 router can provide great value, if only the features worked reliably.** The router is a rebranded ASUS RT-AC68U router that normally sells for $100-160, so you can see why this is a steal when it is on sale for $40. 
 
Though I had major problems using this router, my friend’s router, with stock firmware, hasn’t run into the same problems. I would normally stick with stock firmware, but the router is no longer supported by T-Mobile or ASUS since early 2018, and patches for security issues like the KRACK vulnerability are going to be few and far between.

#### The Problems 
I bought a TM-AC1900, thinking that it would be powerful enough for my 25+ devices, but it failed quite hard under normal internet usage. Between the Wi-Fi disconnect issues, broken guest network, difficulty in flashing the router and updating the firmware, lack of security updates, and the time wasted dealing with these issues, I just cannot recommend this router for beginners. A few things to consider before purchasing this router:


- The steps to flash from T-Mobile to ASUS firmware can be difficult for beginners.
- Features like AiMesh aren’t as fast or reliable as true WiFi mesh systems, according to Smallnetbuilder.
- Features like wireless bridge stopped working after running for one day .
- ASUS is taking drastic measures to revert the router back to T-Mobile firmware without user permission. This was as recent as June 2018.
- Custom firmware like Asuswrt-Merlin do not support the TM-AC1900. The creator specifically said so here, here, and here.

#### Recommended Reading

- Search Slickdeals to find the router on sale
- Instructions to flash the router to ASUS RT-AC68U firmware