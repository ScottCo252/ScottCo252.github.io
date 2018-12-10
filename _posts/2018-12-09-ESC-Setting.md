---
layout: post
title: ESC Setting Data
tag: RC
---


I "discovered" a better setting for my RC race plane's ESC. I'll be going over the data that was pulled off the ESC and comparing it to
data from a race plane in 2017.

A litte background, I've race EF-1 class RC airplanes for the past 4 years. This past week, while building my fith Proud Bird, I noticed
castle ESC had a motor timing option labeled 'Custom'. When selecting it, it allowed input of a number from 1-20. This was much higher than
the default 'High' Setting of 10 that I typically use on my planes. I do not know what each unit signifies, but the discription of the setting explained that it controls the
power of the motor and will result in higher operating temperatures at higher settings. So I set it to 20 and take the new plane out to the
field yesterday.

Four test flights in and I can say it definitley felt faster. On the fourth flight, where I was really pushing it, I hit a low voltage alarm.This is abnormal for my typical
practice flights, so I had to pull the data and see what happened. I'll be comparing the data from yesterday with data I pulled off a proud bird in 2017. It will be using the exact same configuration,
castle speed controller, Rimfire motor and Nantech battery(2.7 A, 4 cell). The only difference will be in the ESC motor timing setting and time of the year (December vs. March).

![Voltage 2018]({{ site.baseurl }}/images/first_flights_dec_2018_voltage.bmp "Voltage 2018") 

You can see I hit the low votlage threshold 4 minutes and 15 seconds into the log. That explains the alarm on that fourth flight.

![Voltage 2017]({{ site.baseurl }}/images/yellow_racer_3_12_17_race_voltage.bmp "Voltage 2017") 

I don't even get close the alarm during that race in march. It looks like the voltage stays above 14 the entire flight in March too. I'll
have to research if this is wearing the batteries harder because it seems like it's pulling more out of them with the higher setting.

![RPM 2018]({{ site.baseurl }}/images/first_flights_dec_2018_rpm_w_line.bmp " RPM 2018") 
![RPM 2017]({{ site.baseurl }}/images/yellow_racer_3_12_17_race_rpm_w_line.bmp " RPM 2017") 

![Current 2018]({{ site.baseurl }}/images/first_flights_dec_2018_current.bmp " Current 2018") 
![Current 2017]({{ site.baseurl }}/images/yellow_racer_3_12_17_race_current.bmp " Current 2017") 

![Temp 2018]({{ site.baseurl }}/images/first_flights_dec_2018_temp.bmp" Temp 2018") 
![Temp 2017]({{ site.baseurl }}/images/yellow_racer_3_12_17_race_temp.bmp " Temp 2017") 

![Watts 2018]({{ site.baseurl }}/images/first_flights_dec_2018_watts.bmp" Watts 2018") 
![Watts 2017]({{ site.baseurl }}/images/yellow_racer_3_12_17_race_watts.bmp " Watts 2017") 

