---
layout: post
title: "HomeKit Build & Review: Meross Smart Wi-Fi Garage Door Opener"
excerpt: "The accessory that kicked off my HomeKit hobby in earnest, the Meross garage door opener was truly the Home addition I’d been waiting for."
---

![Meross Smart Wi-Fi Garage Door Opener](/assets/images/meross-opener.png)

## Looking for an Opening

Ever since the introduction of HomeKit there’s been one accessory that I’ve been pining after over all others: a garage door opener. In the early days of Apple's foray into home automation, garage door options were both incredibly limited and extremely pricey. At one point back in 2016 I even started researching [DIY solutions](https://www.youtube.com/watch?v=03J497Pmve4).  Ultimately I decided to table my search and try again in the future.

And then something happened earlier this year that restarted my search: our garage door remotes started dying. Our garage door is the primary ingress and egress for our home, and the possibility of getting locked out of the house sent me looking for a HomeKit-powered backup. First I replaced the batteries in our clickers, and then I opened a new browser tab to dive into some research.

## “Did you shut the door before we left?”

While the dying batteries in our remotes were the impetus for my renewed interest in a HomeKit garage door opener, it wasn’t the main problem I wanted to solve. The real problem occurred on a semi-regular basis when my family and I would head out on some excursion. We’d be anywhere from the end of the block to a mile away when my wife or I would say to the other, “did we close the garage door?” Almost without fail we’d pull a U-turn and go check. There are lots of ways to fix this problem, including being more mindful about our actions, but I was looking for a safety net that would give us peace of mind even when we weren’t being mindful.

## What I Didn’t Buy

![Chamberlain MyQ System](/assets/images/chamberlain-myq-system.png)

When we first moved into this house there was an old garage door opener that sounded like a rock tumbler every time you opened or closed the door. To call it loud was an understatement — it shook the house. My primary focus for a new opener was sound, which led me to the [Chamberlain Whisper Drive Garage Door Opener](https://www.lowes.com/pd/Chamberlain-0-75-HP-Whisper-Drive-Belt-Drive-Garage-Door-Opener-with-Battery-Back-Up/3653300). The fact that it was compatible with Chamberlain’s MyQ smart home system wasn’t even a blip on my radar at the time, but it definitely came up with the launch of HomeKit. Chamberlain was actually one of the first manufacturers to jump on the Apple bandwagon and add support for HomeKit to their existing MyQ system. They did this by way of an extra hub that you install near your garage door opener. For our MyQ-ready opener that meant buying the MyQ hub and then an _extra_ hub to enable HomeKit support. The price was for this setup was well over $100 and was far more than I was willing to spend at the time. It felt especially egregious because the MyQ hub itself was around $40, while the HomeKit add-on clocked in at two or three times that.

The situation with Chamberlain hasn’t really changed five years later — their proprietary system for HomeKit is still offensively priced. What _is_ different in 2021 is that now there are other options. 

## When Life Closes a Door, Meross Opens It Again

<img src="/assets/images/garage-door-was-opened-notification.png" align="right" alt="Garage Door Was Opened notification"/> I came across the [Meross MSG100 Smart Wi-Fi Garage Door Opener](https://www.meross.com/Detail/29/Smart%20Wi-Fi%20Garage%20Door%20Opener) early on in my search and it immediately hit the right mix of price and positive reviews. There are a lot of factors when it comes to buying a third party accessory for your garage door, not the least of which is compatibility. The Meross unit actually had an extra complication that almost tripped me up: They sell the same unit in two different varieties, one with HomeKit and one without. If you’re shopping on Amazon, [this is the one you want](https://www.amazon.com/dp/B084Z5QZR2).

Once I had confirmed that Meross supported my particular opener using their [compatibility tool](https://www.meross.com/support/Compatibility_Check) and I made sure I had added the right one to my cart, I hit the buy button.

One thing that was mentioned in the Amazon store listing was that I needed to email them for an additional accessory to work with my opener. Their email support was very responsive and after confirming some details about my unit they sent the accessory in the mail. I assumed I would be receiving some sort of interface box to bridge the two wires coming out of the Meross with the inputs on my opener motor. When I received the package I had to chuckle. What arrived was a brand-less opener remote with two wires coming out of it. I paired it with the Chamberlain, hard-wired it to the Meross, and I was off to the races.

Here's what it looks like in my unfinished garage. Yes, it's probably one of my least attractive HomeKit installations, but it's on-brand for this area of the house.

![Meross Garage Door Opener installation in my garage](/assets/images/meross-opener-installation.jpg)

The sensor is a simple magnetic contact sensor that I mounted alongside the rails of my garage door using a spare piece of trim and some lag bolts from a prior projects. Again, she may not look like much, but she's got it where it counts.

![Meross Garage Door sensor installation in my garage](/assets/images/garage-door-installation.jpg)

## Where It Resides In My Home

The opener sits about 19 feet from my router which gives it a really strong signal. I've had no trouble communicating with the opener nor have I seen it become non-responsive within the Home app.

![House layout, first floor](/assets/images/home-layout-first-floor.png)

## The Good

Let’s cut right to the chase: This garage door opener controller is _great_. Connecting it to HomeKit was flawless and pretty much every interaction with it has been exactly what I’d hope for.

The door sensor works really well and has some speedy response times. That shouldn’t be too much of a surprise, though, as it’s a wired sensor that communicates over Wi-Fi.

Most importantly it solved the problem I was hoping to solve plus a few more:

* No longer are we pulling U-turns to double check on the state of the garage door after we leave the house.
* Automations now close the door automatically in the evening.
* If I feel the need to check the door before bed I don’t need to go any farther than the phone on my nightstand.

Beyond the automations that I’ll get to below, I’ve found myself saying, **Hey Siri, close the garage door** to my Apple Watch while buckling the kids into their seats. It’s a small thing, but it works much better than our often-unreliable clickers.

## The Not So Good

As wonderful as this new accessory is there are a few things that surprised me.

For one, I assumed I would be able to have a fully automated setup with our garage door. I had visions of it closing automatically as we rolled down the street away from the house and magically opening again when we return. This is not the case though, and that’s a HomeKit limitation, not a Meross one. As it turns out, any scene that contains a HomeKit accessory that allows entry into your home must be confirmed before being run.

![Garage door automation when anyone arrives home](/assets/images/garage-door-automation-1.png)￼

The other thing that I’ve come to realize is that our home’s geofence is _large_. It stretches clear to the adjacent neighborhood and I frequently will get pings to run automations while I’m out for walks that take me back within the geofence border. I would love to see Apple give us a way to adjust the size of the geofence in iOS 15.

Lastly, the only thing that would have made me reconsider this purchase was the fact that in the end I added another battery-operated dependency to my garage door system. I could _probably_ retrofit the opener with an AC adapter, but the chances of me ever getting to that are pretty small.

## Automations With This Device

Our garage door is probably one of the most automated devices in my home:

* **When Anyone Arrives Home** they are prompted to open the garage door.
* **When Anyone Leaves Home** they are prompted to close the garage door.
* **At 8:30 PM, Daily** the garage door will close. This time also coincides with "lights out" for our kids, so it’s great audible reminder to tell them to go to sleep.
* **10:20 PM, Daily** our **Good night** scene sets, which includes closing the garage door. If the door was opened some time after 8:30, this automation closes it again.
* **Midnight, Daily** I have a catch-all automation that turns off all the lights in the house and, yet again, closes the garage door. It’s rare that anyone is out and about after midnight so this is a nice final safety net for the day.

What’s cool about the prompts to open and close the garage door are that they punch through **Do Not Disturb While Driving**, so I actually do get prompted on my watch as I pull up to the house.

One explicit choice I made with my automations was that I separated out the arrival and departure automations for the garage door from the rest of my arrival and departure automations. I want the thermostat to set itself to **Away** without me having to confirm it, and if I made it part of the same automation that controls the garage door I would have to manually run it every time.

| When Anyone Leaves | When the Last Person Leaves |
| ------ | ------ |
| ![Garage door automation when anyone leaves home](/assets/images/garage-door-automation-2.png) | ![Automation when the last person leaves home](/assets/images/garage-door-automation-3.png) |


## Closing It Down

As I mentioned in my [introductory post for this series](/2021/05/04/homekit-builds-and-reviews-a-series.html), the Meross garage door opener was the HomeKit accessory that kicked this hobby into gear.

It also follows the rules I’m following while building out my smart home:

1.  Make sure all smart accessories can still be controlled via physical controls.
2.  Keep it practical; stick to enhancements that actually make sense.

If you’re in the market for a HomeKit upgrade for your current garage door opener I highly recommend giving Meross a try.

## Further Reading

* [Garage Door Openers at HomeKit News](https://homekitnews.com/tag/garage-door-opener/)
* [Best HomeKit Garage Door Openers at iMore](https://www.imore.com/best-homekit-garage-door-openers)
* [The Best Smart Garage Door Opener Controller at Wirecutter](https://www.nytimes.com/wirecutter/reviews/best-smart-garage-door-controller/)
* [meross.com](https://www.meross.com/)
* [Meross Smart Garage Door Opener Remote, Compatible with Apple HomeKit at Amazon](https://www.amazon.com/dp/B084Z5QZR2)
* [Meross E-mail Support](mailto:support@meross.com)
