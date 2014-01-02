---
layout: post
title:  "Liquid Sunshine Starter Arithmetic"
date:   2014-01-01 21:30:03
categories: [yeast,  technique]
---

I've got a dubbel planned, full of lots of dark, fruity flavors.
The recipe comes in at 1.067, and I'm planning to pitch [WLP500](http://www.whitelabs.com/yeast/wlp500-trappist-ale-yeast-0) into 5.25g of wort.
Pitching-rate calculators suggest about 250 billion cells for a wort of this gravity and volume -- far over the 53 billion cells in my 2-month-old vial.

Based on the calculator built into BeerSmith, I determined that I needed a 2L starter.
I followed my usual process: combine 2L of water and 200g of DME in the easy-to-remember ratio for creating a 1.030 wort.
I boiled this in an Erlenmeyer flask for about 15 minutes, cooled it in an ice bath, and pitched the yeast.
About 18 hours later, with no visible action from the starter, I reached out to my fellow brewers for help.
Ryan Hope suggested that I had underpitched the starter, and should have made a 1L starter as the first step.
He also suggested, and loaned me, a stir plate.

While the starter was bubbling away, I set about educating myself, so that I could better understand what the tools in BeerSmith and mrmalty.com were telling me.
I began with [Yeast](http://www.amazon.com/Yeast-Practical-Fermentation-Brewing-Elements/dp/0937381969) by by Jamil Zainasheff and Chris White.
Figure 5.5 gives propagation rates as a function of the innoculation rate.
The data is based on pitches of 100 billion cells into different volumes of wort, with no agitation or aeration.
Here's an abridged version:

<table>
 <tr><th>Starter Volume<br/>(liters)</th><th>Innoculation Rate<br/>(millions/mL)</th><th>Total Cells at Finish<br/>(billions)</th></tr>
 <tr><td>0.5</td><td>200</td><td>112</td></tr>
 <tr><td>1</td><td>100</td><td>152</td></tr>
 <tr><td>2</td><td>50</td><td>205</td></tr>
 <tr><td>4</td><td>25</td><td>276</td></tr>
</table>

My starter was 53 billion cells pitched into 2L of wort, or about 25 million/mL, so based on this data I should expect 2.76&times;53=146 billion cells -- still a short pitch.

But I'm using a stir plate.
How does that affect the calculation?
All Zainasheff and White have to say is "the yield will be higher."
Thanks guys!

Anecdotal information around the internet ranges from a factor of 1.53 more growth (in [Mr. Malty's Pitching Rate Calculator](http://www.mrmalty.com/calc/calc.html)) through 10 times more growth ([MB Raines' "Yeast Propagation and Maintenance: Principles and Practices"](http://www.maltosefalcons.com/tech/yeast-propagation-and-maintenance-principles-and-practices)).
That's still a pretty wide range!

I [posted](http://www.albanybrewcrafters.com/forum/index.php?topic=843.0) to the Albany Brew Crafters forums and Ryan again helped me out, pointing me to [K. Troester's "Estimating Yeast Growth"](http://braukaiser.com/blog/blog/2012/11/03/estimating-yeast-growth/) and [yeastcalc.com](http://yeastcalc.com) which implements it.

Troester's post is in terms of bilions per gram of extract, but the conversion is simple enough, assuming the standard 10ml/g ratio for building starter worts.
An innoculation rate of 50 million cells per mL, for example, is 500 million cells for 10ml or 1g of extract, or 0.5 B/g.

Similarly, Troester gives growth rates in B/g.
Converting this to a raw cell count is also straightforward, given the starter volume.
For example, a starter volume of 2L contains 200g of extract, so a growth rate of 1.4 B/g will result in 280 billion cells.

Combining Troester's formula with the table from Yeast, still for a pitch of 100 billion cells each:

<table>
 <tr>
   <th>Starter Volume<br/>(liters)</th>
   <th>Innoculation Rate</th>
   <th>Total Cells at Finish<br/>No Stir<br/>(billions)</th>
   <th>Total Cells at Finish<br/>Stirred<br/>(billions)</th>
 </tr>
 <tr><td>0.5</td><td>200 m/mL, 2 B/g</td><td>112</td><td>150</td></tr>
 <tr><td>1</td><td>100 m/mL, 1 B/g</td><td>152</td><td>240</td></tr>
 <tr><td>2</td><td>50 m/mL, 0.5 B/g</td><td>205</td><td>380</td></tr>
 <tr><td>4</td><td>25 m/mL, 0.25 B/g</td><td>276</td><td>660</td></tr>
</table>

My starter had a growth rate of 1.4 B/g in 2L of wort, so I should see 280 billion new cells beyond the 53 billion from the pitch, for a total of 333 billion cells.
At an OG of 1.067, in 5.25g of wort, that will be about 0.98 million cells / mL / &deg;P - close enough for me!
