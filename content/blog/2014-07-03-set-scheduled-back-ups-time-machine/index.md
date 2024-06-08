+++
title = "How to set up scheduled back-ups with Time Machine"
description = "Time Machine is a handy back-up solution, but it would be a whole lot better if you could set up your own schedule. Well, you can…"
date = 2014-07-03
[taxonomies]
tags = ["apps", "back ups"]
+++

When I was setting up my [new iMac](http://wordius.com/save-nearly-200-apples-quad-core-mac-mini/), and got around to organising my Time Machine back-ups, I realised there was something missing. Three years ago when I last set up a new Mac, I wanted to exercise greater control over my back-up system, so it took place when I wanted it to, not according to Time Machine’s fixed schedule:

* Hourly back-ups for the past 24 hours
* Daily back-ups for the past month
* Weekly back-ups for all previous months.

{{ image(path="time-machine-screenshot-576.jpg", caption="Time Machine has a fixed schedule for back ups") }}

A quick search brought me to [Time Machine Editor](http://timesoftware.free.fr/timemachineeditor/) by Time Software, a simple, free, mini application that allows users to determine their own Time Machine back-up schedule. 

{{ image(path="time-machine-editor-screenshot-576.jpg", caption="Time Machine Editor: calendar intervals") }}

Time Machine Editor has three operation modes: Calendar Intervals (as shown above); When Inactive, wherein Time Machine will back-up when your machine is not in use; and, Interval, a simple time-based back-up mode. If you have ever used Apple Mail’s ‘Rules’, you will be familiar with the way the Calendar Intervals mode works. Set an hourly, daily, weekly or monthly schedule; add another by clicking the plus sign on the right. Click ‘Apply’ when you have finished and quit Time Machine Editor.

Simply select Time Machine in System Preferences, under ‘Options’, choose your back-up drive, then switch Time Machine *off*. Yes, I meant *off*. Time Machine editor will switch it on according to the schedule you apply.

Highly recommended.