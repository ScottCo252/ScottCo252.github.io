---
layout: post
title: GPS Telemetry
tag: RC
---

After the let down of trying to plot GPS telemetry data from a Futaba brand telemetry sensor, I decided to build my own solution as a learning experience. I was disappointed in the off the shelf solution's 1hz data logging rate. This rate was far too slow to make a 3d plot of my EF1*** race flight path.

![Mk1 Sensor]({{ site.baseurl }}/images/mk1_sensor.JPG "Mk1 Sensor") 

This is my first attempt at making a GPS telemetry sensor. It's a Raspberry Pi Zero W running Raspbian Jesse Lite. Attached is a Adafruit GPS Breakout board***. The adafruit board is capable of outputting a 10hz data rate over serial, which is sent to PI, which logs it as a text file and saves to the sd card. This sensor is powered by a 500mah battery*** attached to a Raspberry PI lipo Shim***. Data was retrived via SCP and cygwin on my desktop.
![Mk2 Sensor]({{ site.baseurl }}/images/sensor_top_mount.JPG "Mk2 Sensor") 

After the Mk1 sensor was damaged in a crash, I built the Mk2. In this version I replaced the Adafruit breakout board with something better, the Ublox NEO-M8N GPS Module.
![Comparison]({{ site.baseurl }}/images/sensor_comparison.JPG "Mk1 vs Mk2 Comparison") 
![Battery and Switch]({{ site.baseurl }}/images/battery_switch.JPG "Battery and Switch on bench")
![Switch]({{ site.baseurl }}/images/switch.JPG "Switch and Battery") 
![Pi Battery Mount]({{ site.baseurl }}/images/pi_battery_mount.JPG "Raspberry Pi Zero W and Battery Mounted") 
