---
layout: project
title: 'Robocar - TB05'
caption: 1/10 Scale Autonomous Racer
description: >
  Bigger, faster, and meaner than a Donkey Car, running on fully custom
  software. Built on a Tamiya TB-05 Pro chassis kit.
date: 1 Jun 2021
image: 
  path: /assets/img/projects/robocar-tb05.jpg
  srcset: 
    4032w: /assets/img/projects/robocar-tb05.jpg
    2016w:  /assets/img/projects/robocar-tb05@0,5x.jpg
    1008w:  /assets/img/projects/robocar-tb05@0,25x.jpg
links:
  - title: Github
    url: https://github.com/GrantMoe/robocar-py
# accent_color: '#4fb1ba'
# accent_image:
#   background: '#193747'
# theme_color: '#193747'
sitemap: false
---
<!--spacer to prevent body header replacing title-->
## Overview
After building my 1/16 Donkey Car I became aware of the fact that the fastest racers all used 1/10th scale touring cars. Even though I had not yet mastered autonomous driving, I jumped up a scale or two to join them.

Currently the car uses a Jetson Nano for high-level (navigation, vision, autonomy) control and a Teensy 4.0 development board for low level control (sensor interface, steering servo and ESC control signals).

Manual driving is handled by my custom Bluetooth Low Energy transmitter.

## Components
- Chassis: [Tamiya TB-05 Pro](https://www.tamiyausa.com/shop/110-4wd-shaft-drive-road-tb/rc-tb-05-pro-chassis-kit/tb-05/)
- Brains: [Jetson Nano (4GB)](https://developer.nvidia.com/embedded/jetson-nano-developer-kit)
- Steering/Throttle: [Teensy 4.0](https://www.pjrc.com/store/teensy40.html)
- Vision: [IMX219-200 camera](https://www.amazon.com/gp/product/B07T73PQQW)
- Steering Servo: [PohwerHD B7 Revolution PRO](http://www.chd.hk/Product_Detail.aspx?id=189)
- Electronic Speed Control: [Hobbywing XR10 JUSTOCK ESC (G2)](https://www.hobbywing.com/goods.php?id=336)
- Motor: [Hobbwing XERUN V10 G3R Motor - SPEC Class (13.5T)](https://www.hobbywingdirect.com/products/xerun-v10-g3r-motor-spec-class)
- Voltage Regulator: [Polulu 5V, 9A Step-Down Voltage Regulator](https://www.pololu.com/product/2866)
- Battery: [Gens Ace 6500mAh 7.4V 50C 2S1P Hardcase Lipo Battery Pack](https://www.genstattu.com/gens-ace-6500mah-7-4v-50c-2s1p-hardcase-lipo-battery-pack-10-with-4-0mm-banana-to-deans-plug.html)

## Status
Under active development.