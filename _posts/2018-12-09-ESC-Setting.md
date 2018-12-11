---
layout: post
title: ESC Setting Data
tag: RC
---


I "discovered" a better setting for my RC race plane's ESC. I'll be going over the data that was pulled off the ESC and comparing it to
data from a race plane in 2017.

A litte background, I've raced [EF-1](http://www.nmpra.net/rules/EF1NewRules4_15_2014.pdf) class RC airplanes for the past 4 years. This past week, while building my fifth Proud Bird race plane, I noticed a
castle ESC motor timing option labeled 'Custom'. When selecting it, it allowed input of a number from 1-20. This was much higher than
the default 'High' Setting of 10 that I typically use on my planes. I do not know what each unit signifies, but the description of the setting explains that it controls the
power of the motor and will result in higher operating temperatures at higher settings. So I set it to 20 and took the new plane out to the field yesterday.

Four test flights in and I can say it definitley felt faster. On the fourth flight, where I was really pushing it, I hit a low voltage alarm. This is abnormal for my typical practice and race flights, so I had to pull the data and see what happened. I'll be comparing the data from yesterday's fourth flight with race data I pulled off a proud bird in 2017. It will be using the exact same configuration,
a Castle lite 75 speed controller, Great Planes Rimfire EF-1 motor and a Nanotech battery(2.7 A, 4 cell). The only difference will be in the ESC motor timing setting and time of the year (December vs. March).

## Voltage

![Voltage 2018]({{ site.baseurl }}/images/first_flights_dec_2018_voltage.bmp "Voltage 2018") 

The solid red bar signifies the low voltage threshold, you can see I hit the low votlage threshold after 4 minutes into the log.

![Voltage 2017]({{ site.baseurl }}/images/yellow_racer_3_12_17_race_voltage.bmp "Voltage 2017") 

I don't even get close the alarm during that race in march. It looks like the voltage stays above 14 the entire flight in March too. I'll have to research if this is wearing the batteries harder because it seems like it's pulling more out of them with the higher setting.

## RPM

I added a line on the RPM axis at 15K on both graphs. The castle data viewing tool adjusts the scale automatically, so I couldn't set
them the be identical (the higher setting session had a larger scale btw). It looks like the higher setting session has more data points logged above 15K from this crude observation.

![RPM 2018]({{ site.baseurl }}/images/first_flights_dec_2018_rpm_w_line.bmp " RPM 2018") 
![RPM 2017]({{ site.baseurl }}/images/yellow_racer_3_12_17_race_rpm_w_line.bmp " RPM 2017") 

## Current

The session with the higher setting had a larger scale once again and is observed with a much larger peak current, ~74 vs ~62. My dad pointed out that I may be stressing my motor with this level of current. A quick check of the spec shows the rimfire EF-1 is only rated for a 67A surge. I may have to tune the setting lower.

![Current 2018]({{ site.baseurl }}/images/first_flights_dec_2018_current.bmp " Current 2018") 
![Current 2017]({{ site.baseurl }}/images/yellow_racer_3_12_17_race_current.bmp " Current 2017") 

## Temperature

Hard to tell, starting conditions look similar enough.

I have to believe this is running hotter now, especially with all the larger peak values in the data.

![Temp 2018]({{ site.baseurl }}/images/first_flights_dec_2018_temp.bmp " Temp 2018") 
![Temp 2017]({{ site.baseurl }}/images/yellow_racer_3_12_17_race_temp.bmp " Temp 2017") 

## Power

Peak power over 1100 with the higher session, march log has it's peak at 1050. Other older logs varied between 950 and 1050 when I looked through them tonight.

![Watts 2018]({{ site.baseurl }}/images/first_flights_dec_2018_watts.bmp " Watts 2018") 
![Watts 2017]({{ site.baseurl }}/images/yellow_racer_3_12_17_race_watts.bmp " Watts 2017") 

