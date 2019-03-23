---
layout: post
title: GPS Telemetry
tag: RC
---

After the let down of trying to plot GPS telemetry data from a Futaba brand telemetry sensor, I decided to build my own solution as a learning experience. I was disappointed in the off the shelf solution's 1hz data logging rate. This rate was far too slow to make a 3d plot of my [EF-1](http://www.nmpra.net/rules.htm "NMPRA Rules") race flight path.

![Mk1 Sensor]({{ site.baseurl }}/images/mk1_sensor.JPG "Mk1 Sensor") 

This is my first attempt at making a GPS telemetry sensor. It's a Raspberry Pi Zero W running Raspbian Jesse Lite. Attached is a [Adafruit GPS Breakout board](https://www.adafruit.com/product/746 "GPS Breakout Module"). The adafruit board is capable of outputting a 10hz data rate over serial, which is sent to PI, which logs it as a text file and saves to the sd card. This sensor is powered by a [500mah battery](https://www.adafruit.com/product/1578 "Adafruit Battery") attached to a [Pimoroni LiPo Shim](https://www.adafruit.com/product/3196). Data was retrived via SCP and cygwin on my desktop.

![Mk2 Sensor]({{ site.baseurl }}/images/sensor_top_mount.JPG "Mk2 Sensor") 

After the first sensor was damaged in a crash, I built the next version. In this version I replaced the Adafruit breakout board with something better, the [Ublox NEO-M8N GPS Module](https://store.drotek.com/DP0107 "Drotek GPS Module"). This module is capable of using Beidou, GPS, Glonass and Galileo signals. It will also output a 14hz signal, the Adafruit board was only outputting 10hz.

![Comparison]({{ site.baseurl }}/images/sensor_comparison.JPG "Mk1 vs Mk2 Comparison") 
Size Comparison between the two sensors. The Mk1 was attached to the PI. 
In the second version I broke apart the HW and moved the PI inside the fuselage.

![Battery and Switch]({{ site.baseurl }}/images/battery_switch.JPG "Battery and Switch on bench")

Since I no longer had easy access to the battery connector, I installed a switch with a seperate charge cable.

![Switch]({{ site.baseurl }}/images/switch.JPG "Switch and Battery") 

I installed the switch up top near the GPS sensor.

![Pi Battery Mount]({{ site.baseurl }}/images/pi_battery_mount.JPG "Raspberry Pi Zero W and Battery Mounted") 

The Raspberry Pi and 500 mAh battery as seen inside the fuselage with the wing removed.
