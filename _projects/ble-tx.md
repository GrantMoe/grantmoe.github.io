---
layout: project
title: 'Robocar TX'
caption: Custom Arduino-Powered BLE Transmitter
description: >
  DIY modification of a stock 2.4 GHZ radio to function instead with 
  Bluetooth Low Energy. Removes the need for a separate receiver module, 
  interacting directly with Linux through the Human Interface Device (HID) 
  protocol. 
date: 4 Jan 2022
image: 
  path: /assets/img/projects/ble-tx/ble-tx.jpg
  srcset: 
    3264w: /assets/img/projects/ble-tx.jpg
    1632w:  /assets/img/projects/ble-tx/ble-tx@0,5x.jpg
    816w:  /assets/img/projects/ble-tx/ble-tx@0,25x.jpg
links:
  - title: Github
    url: https://github.com/GrantMoe/robocar-tx
# accent_color: '#4fb1ba'
# accent_image:
#   background: '#193747'
# theme_color: '#193747'
sitemap: false
---
<!--spacer to prevent body header replacing title-->
## Overview

I decided to gut the stock RC transmitter that came with my [crawler bot's](/projects/crawler-bot) [chassis kit](https://www.nitrorcx.com/03c09-madtorque-orange.html) 
replace its 2.4GHz radio module with a [Nordic nRF5832](https://www.nordicsemi.com/products/nrf52832).

Previously, I interfaced the RC radio with my robocar by first reading
the output of the stock RC receiver with a Teensy microcontroller, then 
passing it via serial to my Jetson Nano. With the custom BLE method, I 
could skip the receiver and microcontroller by connecting directly to the
Jetson and using Linux's [Human Interface Device](https://en.wikipedia.org/wiki/Human_interface_device) protocol.

HID allows me to interface with the device any way I want, whether with Python
or C++ or whatever, and the kernel handles all of the pairing/trusting/connecting
required by Bluetooth for me.

## Components
- Transmitter Module / PCB: [51C00-9082 2.4G Transmitter](https://www.nitrorcx.com/51c00-90820.html)
- BLE Transmitter: [Adafruit Feather nRF52 Bluefruit LE - nRF52832](https://www.adafruit.com/product/3406)
- Transmitter Display/Input: [Adafruit Mini Color TFT with Joystick FeatherWing](https://www.adafruit.com/product/3321)
- Power Converter: [MPM3610 5V Buck Converter Breakout - 21V In 5V Out at 1.2A](https://www.adafruit.com/product/4739)
- Data Connector: [USB DIY Connector Shell - Type Micro-B Plug](https://www.adafruit.com/product/1390)
- Added switches/hardware: Stuff I found lying around [CRASH Space](https://blog.crashspace.org/)

## Status
Very much in progress. Currently stymied by a hardware issue: the ground wire for the throttle input potentiometer has somehow failed and needs to be re-soldered.

Software-wise, I am now working on a TFT Menu display and hammering out the details of what info needs to be sent to the robocar for full functionality.

## Images
![stock TX testing](/assets/img/projects/ble-tx/ble-tx-testing.jpg){:.lead width="2448" height"2448" loading="lazy"}

Establishing the output of the stock transmitter based on the signals sent to the stock receiver.
{:.figcaption}

![stock TX wiring](/assets/img/projects/ble-tx/ble-tx-before.jpg){:.lead width="3264" height"2448" loading="lazy"}

Stock controller PCB before modification.
{:.figcaption}

![new wiring version 1](/assets/img/projects/ble-tx/ble-tx.jpg){:.lead width="3264" height"2448" loading="lazy"}

The first attempt at new wiring. Kind of a mess. Pardon the blurry image; this was taken with an ancient phone.
{:.figcaption}