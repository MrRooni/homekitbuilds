---
layout: post
title: "HomeKit Build & Review: ecobee4 SmartThermostat with Voice Control"
excerpt: "Welcome to the first post of substance! In today’s post we’ll cover my initial piece of HomeKit tech: The ecobee smart thermostat."
---

![ecobee SmartThermostat with remote sensor](/assets/images/ecobee-hero-image.png)

## A Warmup

Welcome to the first post of substance! In today’s post we’ll cover my initial piece of HomeKit tech: The ecobee smart thermostat.

Even though the ecobee predates the HomeKit rules I’ve set for our house, it follows them nonetheless:

1.  Make sure all smart accessories can still be controlled via physical controls.
2.  Keep it practical; stick to enhancements that actually make sense.

## Stay Smart, Stay Economical

It was Nest that originally popularized the concept of a learning thermostat, and Nest was actually the first smart ecosystem I bought into. I loved the idea of a thermostat that could automatically update my home’s heating and cooling settings based on my habits and routines. It seemed like a great solution to a problem I really wanted to solve: heat and cool my home as efficiently, economically, and with as little waste as possible.

The Nest solved this problem for me for a few years until an electrical short in its backing plate left me with a decision: Buy a replacement Nest or buy an accessory that supported Apple’s new home automation standard.

## Enter The Bee

￼![ecobee lifestyle image](/assets/images/ecobee-lifestyle-shot.png)

I ended up purchasing the **ecobee4 SmartThermostat with voice control** in 2017. The reviews were solid, the company presented a consumer friendly face, and of course it supported HomeKit.

Swapping it in for the Nest was really straightforward. All the power and control wires I needed were already run for both heating and cooling. I then placed the included remote sensor in the upstairs hallway to help even out the temperature readings in the warmer summer months.

![House layout, first floor](/assets/images/home-layout-first-floor.png)

## The Good

Over the last few years the ecobee has been a really nice thermostat for our forced air heating and cooling system. Even though it’s a learning thermostat, we ended up just setting a set schedule for the week with a slightly modified one for the weekends. One aspect that has worked incredibly well, though, is the ability to have the thermostat reduce our energy usage when we’re out of the house and then resume our schedule when we return. This was the problem I really wanted to solve with a smart thermostat and the ecobee does it perfectly.

Another aspect that I appreciate are the service and filter reminders. Once per year I will get a notification that it’s time to have my HVAC (heating, ventilation, and cooling) equipment serviced. More frequently I receive notifications to replace my furnace’s air filter. Knowing that the filter reminders happen based on usage and not just a set schedule means that I’m not always replacing filters that haven’t seen much use.

ecobee (the company) has been pushing out consistent updates to both its app and the thermostat itself which have delivered some new features like eco+ which is actually five features in one:

* **Feels like**, where your indoor humidity is factored into the temperature you’ve set to help keep you comfortable while reducing energy usage.
* **Schedule Assistant** monitors your routine against your set schedule and will suggest new schedules to better match your day-to-day.
* **Smart Home & Away**, which I mentioned above, ensures that energy usage is reduced when the house is empty.
* **Time of Use** & **Community Energy Savings** connect to your local energy supplier to try and call for energy at off-peak times. These features both save you money on your energy bills, and help reduce load on the energy grid.

## Room For Improvement

Overall I’m really happy with our ecobee. There are some things that could be better, though. For one, the mobile app is a bit hard to navigate. I routinely have to tap around quite a bit to get to the settings I’m looking for. It also doesn’t look or feel like an iOS app, but rather one that was the result of one of those development tools that spits out an iOS and Android app from the same code base. The iPad app, while it suffers from the same lack of a native interface, is much nicer.

![ecobee iPad app](/assets/images/ecobee-ipad-app.png)

The other aspect that’s a bit off putting is the cost if you want to add extra sensors to your home. A two pack of sensors is $79 USD on Amazon, and rarely moves from that price point. That’s far too expensive for me to consider putting more of them around my house.

The last thing that’s a bit strange is the way it integrates with HomeKit. For example, my **I’m leaving** scene in the Home app says it will adjust the thermostat to 65º. That’s not quite what I want, though; I want the thermostat to enter its "away" state where it cools or heats the house less while I’m gone. To get that behavior I need to open the ecobee app, tap on the **Account** tab, scroll down to **Integrations**, and tap on **HomeKit**. From there I have to scroll down to the **Scenes** bubble, find the **I’m leaving** scene, and make sure it uses my _Away Comfort Setting_. This will ensure that the thermostat does the right thing in both heating and cooling mode. It’s a pretty involved and inscrutable process that I truly wish was clearer and felt less fragile.


![Home iPad app showing Front Hallway with ecobee thermostat](/assets/images/home-app-front-hallway-ecobee.jpeg)


## Automations With This Device

Being my first ever HomeKit accessory, I didn’t quite grasp how to set it up within the Home app. For the longest time I had a single accessory named **ecobee** in a room in my Home that was named **House**. Today, though, I have a **Thermostat** in my **Front Hallway**. I have the remote sensor in my Upstairs Hallway where it shows up as two named sensors: **Temperature** and **Motion**.

All told the ecobee thermostat adds three different sensors in the Home app:

1. Motion
2. Occupancy 
3. Temperature

And two more for the remote sensor:

1. Motion
2. Temperature 

| Front Hallway | Upstairs Hallway |
| ------ | ------ |
| ![Home app showing my front hallway room](/assets/images/home-app-ecobee-front-hallway.jpeg) | ![Home app showing my upstairs hallway room](/assets/images/home-app-ecobee-upstairs-hallway.jpeg) |


The automations I’ve set up for this thermostat are fairly simple:

* At 10:20 PM every night, my **Goodnight** scene sets, which sets the thermostat to the overnight temperature.
* When the first person arrives home, the **I’m home** scene sets, which tells the thermostat to resume its schedule. This works particularly well in case we come home late at night. The ecobee doesn’t start heating or cooling, it just resumes its schedule – even if that’s the overnight one.
* When the last person leaves, the **I’m leaving** scene sets, which sets the ecobee to its Away Comfort Setting.
* And lastly the internal schedule I’ve set on the ecobee itself, which starts heating or cooling the house at 6:30 in the morning.

For the most part my interaction with the thermostat is completely hands off. It does what I need it to do when I need it to do it. Occasionally, especially around the change in seasons, I find myself turning the heat on and off based on the high and low temperatures for the day and sometimes I even do that by saying, **Hey Siri, turn off the thermostat.**

## Wrapping It Up

I would definitely buy another ecobee thermostat if I needed to, and I would recommend it to others too. It’s a solid thermostat that does its job well. Beyond that it has some really sensible and economical features like eco+ and smart home & away that help the environment and save me money. Lastly, ecobee (the company) is always looking for ways to improve its products and regularly pushes out updates that make this smart thermostat even smarter.

## Further Reading

* [ecobee.com](https://www.ecobee.com)
* [Ecobee SmartSensor 2 Pack on Amazon.com](https://smile.amazon.com/ecobee-SmartSensor-2-Pack-White/dp/B07NQVWRR3)
* [The Best Smart Thermostat at Wirecutter](https://www.nytimes.com/wirecutter/reviews/the-best-thermostat/#other-smart-thermostats-we-like)
* [Best ecobee Thermostats at iMore](https://www.imore.com/best-ecobee-thermostats)

