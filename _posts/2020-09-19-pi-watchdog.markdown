---
title: "Raspberry Pi as Watchdog :eyes:"
layout: post
date: 2020-09-19 21:30
tag: 'raspberry pi"
image: /assets/images/raspberrypi.png
headerImage: true
projects: true
hidden: true # don't count this post in blog pagination
description: "A Raspberry Pi (Zero) checks whether home network stuff behaves."
category: project
author: axel
externalLink: false
---

At home I have a [Raspberry Pi Zero](https://www.raspberrypi.org/products/raspberry-pi-zero/) that needs entertainment.
It's watching our home network devices (WiFi, VOIP / SIP = FritzBox, [vdr](https://www.vdr-portal.de/), fiber internet connection), and reports anything broken on its [simple LED display](https://shop.pimoroni.com/products/scroll-phat-hd?variant=2380803866634).
It also reports incoming calls visually over that display - great if your phone supports silent night mode: you see if someone is calling, without the kids complaining that they woke up by the phone ringing!

Code is here: [pistatescrollhd](https://github.com/karies/pistatescrollhd)
