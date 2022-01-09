---
layout: project
title: 'Crawler Bot'
caption: 1/8th Scale Autonomous Rock Crawler
description: >
  1/8 scale RC Rock Crawler controlled by an ODROID C2 and Parallax Propeller
date: 2 Jan 2022
image: 
  path: /assets/img/projects/crawler-bot.jpg
  srcset: 
    1500w: /assets/img/projects/crawler-bot.jpg
    750ww:  /assets/img/projects/crawler-bot@0,5x.jpg
    375w:  /assets/img/projects/crawler-bot@0,25x.jpg
links:
  - title: Propeller C Repo
    url: https://github.com/GrantMoe/robogarnt-cpp
  - title: BLE Radio Repo
    url: https://github.com/GrantMoe/robo-radio
# accent_color: '#4fb1ba'
# accent_image:
#   background: '#193747'
# theme_color: '#193747'
sitemap: false
---
<!--spacer to prevent body header replacing title-->


## Overview
This was conceived as a robot that could drive around on unprepared surfaces, specifically Aldrich Park at UC Irvine.

I decided I absolutely needed HARD REALTIME performance for a robot that maxes out at a brisk walking pace, so I adopted a [Parallax Propeller](https://www.parallax.com/propeller-1/) running C.

The [RoboPi](https://www.mikronauts.com/raspberry-pi/robopi/) robot controller provides an easy Raspberry Pi-compatible interface, servo-style connectors, power handling, voltage level shifting, and analog input. 

I learned how to do some neat low-level stuff like bit banging SPI communication with an analog-digital converter chip, but I got distracted by other projects before I got everything working together.

## Components
- Chassis: [Exceed RC 1/8Th Mad Torque Rock Crawler](https://www.nitrorcx.com/03c09-madtorque-orange.html)
- Brains: [ODRIOD-C2](https://wiki.odroid.com/odroid-c2/odroid-c2)
- Sensors/Control: [RoboPi](https://www.mikronauts.com/raspberry-pi/robopi/)
- ESC: [QUICRUN 1060 ESC - BRUSHED](https://www.hobbywingdirect.com/products/quicrun-10-esc-2-3s-brushed) x2 
- Steering Servo: [Solar D772 High Voltage Servo](https://www.hobbypartz.com/33p-solarservo-d772.html) x2
- Radio: [custom BLE radio project](https://github.com/GrantMoe/robo-radio)

## Status

<iframe width="560" height="315" src="https://www.youtube.com/embed/cdBuQvcAnks" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>  
<br>
Partially complete. Drivable in manual mode.

On hold while I develop self-driving software on smaller platforms.