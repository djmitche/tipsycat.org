---
layout: post
title:  "Temperature Control"
date:   2014-06-01
categories: [brewery]
---

I've been brewing on the brewstand for a while now.
I've worked out a system for getting mash temperatures right -- even with a HERMS system, it's not as easy as it might seem!

To review, a HERMS (heat exchanger recirculating mash system) maintains mash temperature by pumping the wort through a heat exchanger (a copper coil in my case) in the hot liquor tank.
The hot liquor tank is temperature controlled.
Other options are RIMS (recirculating infusion mash system), which circulates wort through a tube with a heating element; and directly heating the mash tun.
Both of these options have the disadvantage of directly heating the wort, which may send it over 170&deg;F (the temperature range where the diastatic enzymes denature) a little bit at a time.

Mashing In
==========

The obvious choice for mashing in with a HERMS is to heat the hot liquor tank to the desired mash temp (say, 152&deg;F), draw off the strike water into the mash tun, and dough in.
There are two problems with this.
First, those 15lbs or so of grain and the heat mass of the mash tun will pull the overall mash temperature down 10-20&deg;F.
Second, there is a temperature differential of about 4&deg;F between the hot liquor tank and the mash tun.
So, for that 152&deg;F mash, the HLT should be at 156&deg;F, but once the water hits the mash tun, it's at something closer to 135&deg;F -- way too low.
With a 1500W element, it takes almost an hour to get that mass back up to 152&deg;F, meaning a slow ramp through the &beta;-Amylase range ultimately a very thin-bodied beer.

The solution to this quandry is to strike at an appropriate temperature for the mash, just like an infusion mash, then start the recirculation once hte HLT is near the target temperature.
To accelerate the brewday, I heat all of the brewing liquor in the boil kettle, where the 5500W element can get it to temperature in under a half-hour.
I then transfer the strike water directly to the mash tun, then pump the rest into the hot liquor tank.

There's one more temperature differential to think about in this case: for reasons I can't identify, the system loses about 25&deg;F between the boil kettle and the mash tun.
I suspect that this is due to loss heating the tubing, fittings, and pump bodies, but at any rate it's consistent.

So the process is this: 
First, I calculate the strike temperature given the desired mash temperature, grain weight, and mash-tun mass (BeerSmith does this for me, but online calculators do too), and add 25&deg;F.
I heat the total water volume, plus enough to cover the HERMS coil, to this temperature.
The strike volume goes into the mash tun, with the remainder going into the hot liquor tank, and the grain goes into hte mash tun.

I set the hot liquor tank for 4&deg;F over the mash temperature, but don't start recirculating until the water cools to about that temperature, or until the mash temperature falls a few degrees below the mash temp.

Mashing Out
===========

The mash out is, fortunately, a little simpler: I change the HLT temperature controller to 168&deg;F and wait.
The system can heat that at about 0.3&deg;F/min, so about a half-hour later, the mash is at 168&deg;F.
At that point, the hot liquor tank is full of 168&deg;F water ready to sparge.

Only as Good as Your Tools
==========================

A few weeks ago, I co-brewed a with Rian Colbert, following the plan above.
I measured the temperature in the boil kettle with my "traceable" Fisher thermometer, and bragged about how fast it came up to temperature (190&deg;F).
I measured the water in the mash tun at about 165&deg;F, as expected.
We doughed in, and then Rian measured the mash temperature - 132&deg;F!
The dial on the mash tun, and the probe from the HLT temperature controller agreed - way too low.

After some testing, I discovered that the thermometer will sometimes read about 25&deg;F hot.
It does so consistently, but will "reset" to the correct temperature after a power cycle.

We managed to get the mash to temperature eventually, by re-heating some of the wort in the boil kettle -- but in the process de-natured the enzymes in that wort.
The beer is still in the fermenter, so no word yet on how it turned out, but surely less well than it could have!

I've purchased a pair of digital probe thermometers now - a [ThermoWorks RT600C](http://www.thermoworks.com/products/low_cost/rt600c.html) and a [CDN DTQ450X](http://www.amazon.com/gp/product/B0021AEAG2/ref=oh_details_o02_s00_i00?ie=UTF8&psc=1) - and will be using both and comparing the results.
In today's brewday, both new thermometers agreed with one another and with the temperature controller, so I have high confidence in the mash temps for this brew.
