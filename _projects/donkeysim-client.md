---
layout: project
title: 'Donkey Sim Client'
caption: Online Racing Telemetry/Control
description: >
  Python client that sends driving inputs from an XBox controller or a 
  self-driving neural network model. Records video and telemetry data 
  for training and posterity.
date: 6 Jan 2022
image: 
  path: /assets/img/projects/donkeysim-client.jpg
  srcset: 
    840w: /assets/img/projects/donkeysim-client.jpg
    420w:  /assets/img/projects/donkeysim-client@0,5x.jpg
    210w:  /assets/img/projects/donkeysim-client@0,25x.jpg
links:
  - title: Github
    url: https://github.com/GrantMoe/donkeysim-client
# accent_color: '#4fb1ba'
# accent_image:
#   background: '#193747'
# theme_color: '#193747'
sitemap: false
---
<!--spacer to prevent body header replacing title-->
## Overview
[DIY Robocars](https://www.meetup.com/DIYRobocars/) hosts remote races using the [Donkey (Car) Simulator ](https://www.donkeycar.com/updates/simulator). I wanted to compete, but I found that my XBox controller wasn't playing well with the default client. Specifically, I was not able to use my analog triggers for throttle and brake.

Thus, I wrote my own client using the available [API](https://docs.donkeycar.com/guide/simulator/#api).

In doing so, I gained the ability to record telemetry data in formats other than the default [Donkey Car Tub](https://docs.donkeycar.com/parts/stores/#tub) format.

### Supported Data Formats
* [Donkey Car Tub](https://docs.donkeycar.com/parts/stores/#tub) - format used by Donkey Car for autonomous driving training. Enables use with neat [Donkey UI](https://docs.donkeycar.com/utility/ui/) tools.
* CSV for my [General Assembly Data Science Immersive capstone project](https://github.com/GrantMoe/DSI-Capstone-Project) - plugs straight into Pandas for easier data processing and modeling.
* ASL format - used in my experiments with the [OpenVSLAM](https://github.com/OpenVSLAM-Community/openvslam) Visual Simultaneous Localization and Mapping framework.

## Status
![Mini-Monaco Demo Lap with Minimap](/assets/img/projects/donkeysim-monaco-lap.gif){:.lead width="840" height"454" loading="lazy"}  
  
Living, breathing, and evolving as needed.