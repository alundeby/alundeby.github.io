---
permalink: /projects/battery-killer
layout: single
title: "Battery Killer"
---

This project was a test of several things:
* PCB design
* ATTiny in-place programming
* Surface mount soldering skills

I had seen people building joule thief circuits to use up the last remaining power from nearly dead batteries but I wanted to do something more complex as a challenge. I decided to build a custom PCB around a single AA battery holder and use it to power an ATTiny85.

<img src="https://media.darkwire.com/battery-killer/battery_killer.jpg">

I started by selecting a single cell AA holder that would provide the PCB footprint. I wanted something with through-hole pins so that I wouldn't have any wires that could eventually break.

The next step was designing a power supply. I knew that I needed a minimum of 1.8v to run the ATTiny85 controller so I opted for a MCP1640T boost regulator. It's capable of running on well below 1.0v input and has an adjustible output from 2.0 to 5.5v which was perfect for my application.

<img src="https://media.darkwire.com/battery-killer/board_top.png">
<img src="https://media.darkwire.com/battery-killer/board_bottom.png">

The notch in the PCB is actually to allow clearance for an orientation pin on the battery holder.
