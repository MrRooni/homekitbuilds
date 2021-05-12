---
layout: post
title: "Automation Update: ecobee SmartThermostat + Shortcuts"
excerpt: "A shortcut to turn off my ecobee thermostat kicked into gear this morning."
---

![ecobee loves Shortcuts](/assets/images/ecobee-loves-shortcuts.png)

## Smart Meets Smarter

When I wrote my post last week about the [ecobee4 SmartThermostat](/2021/05/08/ecobee4-smartthermostat-with-voice-control.html) there was an automation I didn't talk about because up until today it didn't work. What I wrote was:

> For the most part my interaction with the thermostat is completely hands off. It does what I need it to do when I need it to do it. Occasionally, especially around the change in seasons, I find myself turning the heat on and off based on the high and low temperatures for the day and sometimes I even do that by saying, **Hey Siri, turn off the thermostat.**

Turning off the thermostat based on the weather conditions of the day was something I had tried to automate using the Shortcuts app, and it worked fine when running within Shortcuts, but it never seemed to trigger automatically. And then this morning, this happened:

![ecobee auto shutoff notification](/assets/images/ecobee-auto-shutoff-shortcut-notification.jpeg)

🎉 

I'm not 100% sure what changed, but my shortcut for automatically turning off the thermostat finally kicked into gear. It could be the recent iOS update to iOS 14.5.1, or something else. It's also possible that it was a fluke and it won't work again. Regardless, I wanted to share it with you now.

The psuedocode version is this:

1. If the thermostat is off, do nothing.
2. Get the forecast for the day at my location.
3. For each hourly temperature over the next 8 hours, check these things:
4. If the house is being cooled, and the temperature will drop below 78º, turn off the thermostat and post a notification.
4. If the house is being heated, and the temperature will rise above 65º, turn off the thermostat and post a notification.

I run this at 8:30 every morning. This time was set by my daughter because she enjoys the heat coming out of the vents when she first wakes up in the morning. 🙂

![Daily ecobee shortcut automation](/assets/images/daily-ecobee-automation.png)

![ecobee auto shutoff automation](/assets/images/ecobee-auto-shutoff-shortcut-notification.png)
