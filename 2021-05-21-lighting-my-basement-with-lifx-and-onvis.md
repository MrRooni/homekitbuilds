---
layout: post
title: "HomeKit Build & Review: Lighting My Basement With LIFX and ONVIS"
excerpt: "With my garage door properly automated my mind turned to other places in my house that could do with a bit of HomeKit love."
---

![LIFX Mini Day & Dusk and ONVIS Contact Sensor CT2](/assets/images/lifx-and-onvis.jpg)

## Light ‘em Up

With our [garage door properly automated](https://homekitbuilds.mrrooni.com/2021/05/14/meross-smart-wi-fi-garage-opener.html) my mind quickly turned to other places in my house that could do with a bit of automation. Lighting is the typical smart home entry point and that’s where I headed next. The previous homeowner had finished the basement of our house and installed ceiling lights operated by pull chain throughout. If you wanted to turn on the lights in the basement you had to walk around to four separate locations to do so.

Those lights last about a year before the pull chains were snapped by overzealous children and I started on a project I would never finish to wire these lights to a proper wall switch. The old bulbs were removed, the chains were never replaced, and we made due with a mostly dark basement whenever we went down there.

With my newfound HomeKit hobby, however, I realized there was a better way than cutting holes in the wallboard and fishing wire. By setting the fixtures to always on, they were perfect candidates for smart bulbs.

## LIFX to the Rescue

I picked up a four pack of [LIFX Mini Day & Dusk bulbs at amazon.com](https://www.amazon.com/gp/product/B072Y6X7QS/) based on a few criteria:

	0.	**The fact that they didn’t need a hub.** While Philips Hue is the most popular smart bulb system, it requires an extra hub to work, and I wasn’t prepared to buy into an entire ecosystem for an endeavor that was still an experiment.
	0.	**Their review rating** — 4.4 stars out of 5 with nearly 7,000 reviews.
	0.	**The price.** $74 over all and $18.50 is a lot of money per bulb, but it was certainly cheaper than my construction project alternatives.

Installation was trivial (I mean, it’s a light bulb…) and adding it to HomeKit was quite easy. Within the package was a card with each of the HomeKit codes on it in numbered order. The order on the cards matched the order of the bulbs in the box, so I wrote the bulb’s number on its stem before screwing it in. One thing that surprised me — and this is totally my fault for not reading carefully — is that these are not RGB bulbs. They are a range of color temperature variations on white.

![LIFX HomeKit code card](/assets/images/lifx-homekit-card.jpg)


After a quick firmware update via the LIFX app I was ready to go. I grouped three of the bulbs into one group called **Ceiling Lights** and named the fourth bulb **Freezer Light** as it resides directly over our chest freezer. Let me tell you, not having to use our phone’s flashlight when getting something out of the freezer is great!

![Home app showing the basement lights](/assets/images/basement-lights.png)

When I first installed these lights I was using Siri on my Apple Watch to control them. Every time I went down the basement stairs: **Hey Siri, turn on the basement lights.** Every time I came up the basement stairs: **Hey Siri, turn off the basement lights.**

This was fun the first couple times, but it turns out I go up and down the basement stairs a lot — especially when I’m in the middle of a home improvement project. (Which I currently am). This also didn’t help my wife or kids who weren’t keen to yell out to the HomePods in the living room each time they went downstairs. For them it was like nothing had changed. I needed something better.

## ONVIS to the Rescue of LIFX

I had an [ONVIS door and window sensor](https://www.amazon.com/gp/product/B08JQ96N8J/) from another project that didn’t work out (more on that in a future article) and decided to put it to use automating my basement lights. I installed it on the hinge side of the basement door, added it to the Basement in the Home app, and hooked up a very simple automation. Whenever the basement door is opened, set the basement lights to 100% and turn them off again five minutes later.

![Basement lights automation in the Home app](/assets/images/basement-light-automation.jpeg)

This automation has been exactly what we needed. The timing on the lights is perfect and it has even received what I consider the highest praise it can: completely unprompted my wife told me, **Those basement lights you installed work perfectly. They’re great.**

![House layout, Basement](/assets/images/home-layout-basement.png)

![House layout, first floor](/assets/images/home-layout-first-floor.png)

## The Good

The LIFX bulbs, which connect directly to HomeKit over Wi-Fi, have worked out really well. They’re plenty bright enough, quite responsive to commands, and I haven’t had any problems to speak of. 

The ONVIS sensor, which also connects directly to HomeKit but over Bluetooth, is a decent sensor. It does require a nearby Bluetooth connection to be responsive, though, which leads me to…

## The Not So Good

This automation works 100% of the time, but it doesn’t always fire immediately. I’d say that about 90% of the time the lights come on as soon as the door opens. The other 10% of the time it’s a mixed bag with the lights coming on as I’m heading down the stairs or am in the basement headed to my destination. One time I actually made it all the way to the freezer (which is just about as far from the door as I can go) before the lights finally kicked on.

The other less-than-great aspect of these accessories are their apps. They are clearly write-once, run-anywhere apps designed to check a box. They aren’t great iOS apps by any means. I don’t really use them beyond periodic checks for firmware updates, so they aren’t a deal breaker. There is one thing that tells me someone at LIFX cares about making a great iOS app, though: the LIFX app exposes [Siri Shortcuts](https://support.apple.com/en-us/HT209055). More on that in the **Automations** section below.

| The LIFX App | The ONVIS App |
| ------ | ------ |
| ![The LIFX app](/assets/images/lifx-app.jpeg) | ![The ONVIS app](/assets/images/onvis-app.jpeg) |

## Automations With This Device

Beyond the door sensor automation, I have these lights participating in a few other automations:

* **10:20 PM, Daily** our **Good night** scene sets, which turns the basement lights off.
* **Midnight, Daily** This catch-all automation turns off all the lights in the house, in case they were turned on after 10:20.

There was another automation I really wanted that took me a few days to figure out. I wanted the color temperature of these bulbs to change based on time of day. Cooler during the day, and warmer in the evenings. I struggled to find a way to do this in the Home app or even the wonderful [Eve app](https://itunes.apple.com/app/elgato-eve/id917695792). Ultimately it was LIFX’s Siri Shortcuts that solved this for me. Using the Shortcuts app I was able to create two different **Personal** automations. One that runs at sunset and one that runs at sunrise:

	•	**At Sunrise, Daily** set the light to white, 3500 K.
	•	**At Sunset, Daily** set the light to white, 2700 K.


|  |  |
| ------ | ------ |
| ![LIFX sunrise automation in the Shortcuts app](/assets/images/lifx-sunrise-automation-1.jpeg) | ![LIFX sunrise automation actions in the Shortcuts app](/assets/images/lifx-sunrise-automation-2.jpeg) |


I’m hoping to see a firmware update from LIFX that enables [HomeKit Adaptive Lighting](https://homekitnews.com/2020/11/02/adaptive-lighting-in-homekit-how-it-really-works/) for these bulbs. With that in place I could get rid of both of these Shortcuts. In the meantime these Shortcuts work great and the bulbs properly reflect the time of day every time I go to the basement.

## Fading to Black

What’s interesting about this setup is that _technically_ it breaks one of my rules: Make sure all smart accessories can still be controlled via physical controls.

I can’t go around to each bulb and physically operate it very easily. I _could_ find the pull chain stub on each one and toggle it off and on to get the bulbs to light up, but I won’t realistically ever do that. Regardless, these bulbs are incredibly practical and definitely make sense.

In general I don’t think that smart bulbs have nearly the amount of value you can get out of a smart switch. But for this particular application with an always-on power supply they were perfect. If you’re looking for some starter bulbs to introduce smart lighting to your home you would do well to consider these bulbs. Couple them with a door sensor and you too can automate one more thing away.

## Further Reading

* [LIFX at HomeKit News](https://homekitnews.com/?s=LIFX)
* [ONVIS CT2 Smart Contact Sensor Review at HomeKit News](https://homekitnews.com/2020/10/15/onvis-ct2-smart-contact-sensor-review/)
* [Best HomeKit Light Bulbs at iMore](https://www.imore.com/best-homekit-light-bulbs)
* [Best HomeKit Door and Window Sensors at iMore](https://www.imore.com/best-homekit-door-window-sensors)
* [Best smart light bulbs for HomeKit at Wirecutter](https://www.nytimes.com/wirecutter/reviews/best-homekit-devices/#best-smart-light-bulbs-for-homekit)
* [lifx.com](https://www.lifx.com)
* [ONVIS at amazon.com](https://www.amazon.com/s?k=ONVIS)
