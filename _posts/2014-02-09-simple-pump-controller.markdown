---
layout: post
title:  "Simple Pump Controller"
date:   2014-02-09 10:15:00
categories: [brewery]
---

The parts for the new brewery are arriving, and a few days ago I assembled a simple pump controller.
The pumps will eventually be automatically controlled, so this is a temporary solution while I get used to the system.

This is a simple 2-gang outlet box with two switch/outlet combo devices - one to control each of two pumps.

Materials
=========

* 2-gang &frac12;" FSE PVC box - Lowes = $5
* 2-gang PVC faceplate - Lowes = $3
* 2x 15A switch/outlet combination - Lowes = $9 x 2 = $18
* Short length &frac12;" conduit - Lowes = $1
* &frac12;" to &frac12;" female threaded adapter - Lowes = $1
* &frac12;" thread cable gland - Lowes = $1
* 8' 12-3 (H/N/G) SJOOW - Lowes = $10
* 8' &frac12;" TechFlex expandable sleeving - Amazon = $4 (partial from 50' lot)
* 2x &frac34;" x 4" heat-shrink - Amazon = $1 (partial from 10' lot)
* 5-20P straight blade plug - Amazon = $8

Build
=====

Cord
----

The cord design is based on the build at [The Electric Brewery](http://www.theelectricbrewery.com/): round cable covered with nylon mesh sleeving, with the ends secured with shrink-wrap.
The underlying cable is waterproof, and the sleeving gives it some abrasion resistance and generally looks good.
The shrink-wrap keeps the ends of the sleeving from fraying and adds a little stiffness.
The stuff frays quickly:

![TechFlex on Cable](/img/techflex.jpg)

The smart way to do this would have been to shrink the heat-shrink before adding the devices to the cable.
I don't have a heat gun, so I was left applying heat with a gas stove to a cable already wired into the plug and box.

Box
---

The FSE box that I chose for this project is intended to be glued to PVC conduit running to another box.
The whole system is intended to enclose wires, so Lowes doesn't stock appropriate cable glands.
On the advice of an employee, I attached a &frac12;" female threaded coupling using a very short piece of conduit and fit a cable gland (intended for steel conduit) to the end.
The best view of this assembly is in the finished controller, below.

Wiring
------

The plug was simple to wire -- it's even color-coded!
The 5-20P has one of its blades turned 90&deg; so that it won't fit in a 15A receptacle.
More on that later.

The box, too, should have been simple, just like wiring a residential receptacle.

![Controller Components](/img/pump-controller-pieces.jpg)

I used some extra solid-core wire from other wiring projects to branch the hot, neutral, and ground to both receptacles.
My mistake, shown in this diagram, was assuming that I knew what the terminals meant based on color alone.
This particular arrangement has the receptacles permanently hot, with the switches doing nothing.
Following the wiring diagram that came with the receptacles cleared this right up.

![Miswired Controller](/img/pump-controller-miswired.jpg)

Results
=======

The finished controller looks like this:

![Finished Controller](/imag/pump-controller-finished.jpg)

The switches are mounted at the top with the intention that the box would be mounted with the cable entering from below, adding a little drip resistance.
This isn't a NEMA-4 installation, but every little bit helps.

Safety
======

There are three major problems with this build.
Perhaps you've already spotted them!

First, you can see from the lack of a T-shaped slot that the receptacles in the controller are only rated for 15A, while the controller requires a supply rated at 20A.
The guiding principle for fire safety in electrical systems is that any current-carrying components must be able to sustain at least the rated current of the upstream breaker or fuse.
The idea is that if the load draws, say, 18A, then a 20A breaker will not trip, so everything between the load and the breaker must carry that full current without igniting.
That's not the case with this controller: a pump drawing 18A would not trip the breaker, but could cause the 15A-rated receptacles to burn out.

This wasn't an accident: I couldn't find a 20A version of these devices, I know that the pumps draw only 1.5A each, and anyway this is a temporary build.
I will re-use the 5-20P later, in a 20A build.

Second, the steel cable gland is a safety hazard.
Any externally exposed metal in a project like this should be grounded.
Then, if by some accident it comes into contact with a live conductor, the current will short to ground and trip the breaker.
If this gland managed to cut through the insulation on the cable, the gland would be at line voltage, but nothing would fail.
Not, at least, until someone touched the gland and provided a path to ground.
The GFCI protection might save a life in that situation, but it might not.

![Oversized Cable Gland](/img/pump-controller-oversized-gland.jpg)

Third, the cable gland is too large for the cable.
This means that the weight of the cable is supported by the conductors and the wire nuts inside.
A good tug could probably pull the cable out of the enclosure entirely, exposing live wires.

I've temporarily remedied the latter problem by wrapping the shrink-wrap with enough electrical tape that the gland grips it.
I'll fix both problems with a new, non-metallic cable gland better sized to the cable.
