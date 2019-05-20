---
permalink: /projects/garage-mesh
layout: single
title: "Garage Door Sensor"
---

Devices:
Particle Argon and Xenon
Magnetic garage door sensor

My garage is situated underneath the main floor of my home and faces the alley so it's easy to overlook when the garage door has been left open. I wanted an easy way to verify that it was shut without having to walk down three flights of stairs so I decided to build a remote indicator setup. I could have done this over wifi but Particle was in the process of releasing their new mesh devices and I thought this would be the perfect project to try them out on.


<img src="https://media.darkwire.com/garage-mesh/track_sensor.jpg">
At first I was planning to mount everything near the bottom of the door as that is the way I had always seen it done. After thinking about it I realized that the height didn't matter, I just needed it to be on a flat section of track. The top of the door ended up being closer to my power supply as well as keeping the sensor up and out of the way.

<img src="https://media.darkwire.com/garage-mesh/track_sensor2.jpg">
The sensor comes on a mounting bracket designed to clip to the outside of the track away from the wheels.

<img src="https://media.darkwire.com/garage-mesh/door_magnet.jpg">
The magnetic portion is attached to the door. I selected a location where I could screw into a steel mounting plate rather than the flimsy aluminum skin of the garage door panel.

<img src="https://media.darkwire.com/garage-mesh/sensor_installed.jpg">
Sensor assembly installed. 

<img src="https://media.darkwire.com/garage-mesh/wemos_open.jpg">
My first version used a Wemos module as the controller and sent broadcast UDP packets over wifi to the receivers. When the door is open the blue LED is lit.

<img src="https://media.darkwire.com/garage-mesh/wemos_closed.jpg">
When the door is closed, the blue LED turns off.
