Math Black Magic Vol 2: The Limit Does not Exist!
=================================================

| Author       | Source       | 
| :-------------: |:-------------:|
|  [u/nydus_erdos](https://www.reddit.com/user/nydus_erdos/) | [Reddit](https://www.reddit.com/r/Superstonk/comments/nwy0oz/math_black_magic_vol_2_the_limit_does_not_exist/) | 

---

[DD 👨‍🔬](https://www.reddit.com/r/Superstonk/search?q=flair_name%3A%22DD%20%F0%9F%91%A8%E2%80%8D%F0%9F%94%AC%22&restrict_sr=1)

DISCLAIMER: Second part of my first DD. Not financial advice. All credit to the authors of cited works. I am not trying to karma farm or be dramatic by breaking this up into parts. I tried to post it all at once, but the picture limit had other plans.

-----------------------------------------------------------------------------------------------------------------------------------------------------

ACKNOWLEDGEMENTS:

Shout out to [u/sososhibby](https://www.reddit.com/u/sososhibby/). One of their [comment](https://www.reddit.com/r/Superstonk/comments/nm3mtr/relevant_af/) got me started down this rabbit hole and they were nice enough to give my work a quick check before I posted. They've also posted about this topic as well: [Part 1](https://www.reddit.com/r/Superstonk/comments/nmaaaa/john_d_finnerty_excerpt_from_hoc_3_explained_pt1/), [Part 2](https://www.reddit.com/r/Superstonk/comments/nmdbzz/excerpt_from_hoc3_relevant_af_20_finnerty_fer/)

[u/JNWolman](https://www.reddit.com/u/JNWolman/) was all over this topic months ago. IMO, the post didn't get the exposure it was due. Give it a [read](https://www.reddit.com/r/GME/comments/mgmbkf/would_the_real_exit_strategy_please_stand_up/).

I'll also be using [charts](https://www.reddit.com/r/Superstonk/comments/nwwy5x/0610_update_broke_the_logfloor_by_1_5_in_linear/) from [u/JTH1](https://www.reddit.com/u/JTH1/), aka "exponential floor guy".

-----------------------------------------------------------------------------------------------------------------------------------------------------

A. Topics Explored

In [Vol. 1](https://www.reddit.com/r/Superstonk/comments/nw8281/math_black_magic_vol_1_why_it_is_mathematically/), I laid out [Finnerty's paper](https://www.sec.gov/comments/s7-08-08/s70808-318.pdf) which mathematically proves that to drive a firms price very close to zero, a manipulator MUST naked short AT LEAST the same number of shares as there are shares outstanding, effectively doubling the float.

This write up is more of my examination of the implications of Finnerty's paper and how it applies to GME. This is not meant to be proof, more of this smooth brain's musings. Feedback and constructive criticism are welcome. In this volume I'll examine:

-   What I think the hedgies' algorithm and how apes fucked up said algo.

    -   I should note, that I believe the algos covered here have been modified since, but the damage has been done.

-   Why short attacks are getting weaker.

-   The negative volume that pops up every so often.

-   Why it is Impossible to Short Ape Curve Close to Zero.

PROTIP: This volume is a bit more math heavy than the last, but don't let that intimidate you!

Don't focus too much on the letters, as long as you know who is doing what at each time and what greater than (>) , less than (<) and equal (=) means you'll be good. I'll try to clarify anything that gets too intense.

-----------------------------------------------------------------------------------------------------------------------------------------------------

B. Naked Short Selling: Separating Equilibrium

In separating equilibrium, the manipulator scares away the other participants with unconcealed, aggressive naked shorting. This maximizes profits by eliminating competition. Since the manipulator has price control it doesn't matter whether the time 3 price should be *H* or *L*.

The lack of competition also makes this strategy a bit more formulaic than the previous examples. The manipulator maximizes his short sale proceeds by naked shorting at time 1 (Pg. 48 par. 1, Pg. 54-55, par. 1):

[![r/Superstonk - Math Black Magic Vol 2: The Limit Does not Exist!](https://preview.redd.it/n42c0ax4ag471.png?width=1058&format=png&auto=webp&s=042be52553c72a8b726c3cfe08aa169145c5b35e)](https://preview.redd.it/n42c0ax4ag471.png?width=1058&format=png&auto=webp&s=042be52553c72a8b726c3cfe08aa169145c5b35e)

Price at Time 1

[![r/Superstonk - Math Black Magic Vol 2: The Limit Does not Exist!](https://preview.redd.it/53iy2wm8ag471.png?width=1074&format=png&auto=webp&s=0c529a4731e2fe5e73009d21f13f45017923a87d)](https://preview.redd.it/53iy2wm8ag471.png?width=1074&format=png&auto=webp&s=0c529a4731e2fe5e73009d21f13f45017923a87d)

Price at Time 2

[![r/Superstonk - Math Black Magic Vol 2: The Limit Does not Exist!](https://preview.redd.it/hku7v10hag471.png?width=1116&format=png&auto=webp&s=cb29b1b65823c35eebd53733bdc417e1d330930c)](https://preview.redd.it/hku7v10hag471.png?width=1116&format=png&auto=webp&s=cb29b1b65823c35eebd53733bdc417e1d330930c)

Price at Time 3

Note the rate of change:

> This has occurred with a huge volume of naked shorting and a precipitous decrease in share price that first cut the price in half and then reduced it close to zero. (Pg. 46, par. 2)

I found that statement slightly unclear as the price is reduced by a third then halved. At most it could be an editing mistake, but more than likely it is my smooth brain. Wrinkle brain help is appreciated.

-----------------------------------------------------------------------------------------------------------------------------------------------------

C. Inverted Demand Curve

First, lets put the original general demand curve into slope intercept (i.e. make it easier to graph as a line):

[![r/Superstonk - Math Black Magic Vol 2: The Limit Does not Exist!](https://preview.redd.it/99u0fkwpbg471.png?width=1079&format=png&auto=webp&s=16e5c56e020759b1add8ca735ed16bf23d230d1b)](https://preview.redd.it/99u0fkwpbg471.png?width=1079&format=png&auto=webp&s=16e5c56e020759b1add8ca735ed16bf23d230d1b)

Slope Intercept Demand Function

This is a line with a downwards slope of *-B*. Recall that in Finnerty's model, *B* is the price that retail buys, which is always lower than the prevailing price. That means that as retail acquires more and more shares, the price/demand will decrease.

[![r/Superstonk - Math Black Magic Vol 2: The Limit Does not Exist!](https://preview.redd.it/26cayz89cg471.png?width=1052&format=png&auto=webp&s=070d5441380426260557d52bcd1db5fcdd3479e6)](https://preview.redd.it/26cayz89cg471.png?width=1052&format=png&auto=webp&s=070d5441380426260557d52bcd1db5fcdd3479e6)

Demand Curve Comparison

With apes, however, it works the opposite way. Yes, apes buy at any prices, but what I think fucked up the algorithm is apes buy at higher and higher prices because ape and FOMO. In this case, demand and price increase as supply increases. Meaning that if apes got all the shares, the price would rise to *H* This changes the slope of the demand curve positive:

[![r/Superstonk - Math Black Magic Vol 2: The Limit Does not Exist!](https://preview.redd.it/mefhrczrcg471.png?width=1280&format=png&auto=webp&s=7ba9489b6191491937bd9e755e43b562fc731947)](https://preview.redd.it/mefhrczrcg471.png?width=1280&format=png&auto=webp&s=7ba9489b6191491937bd9e755e43b562fc731947)

Ape Demand Function

What I gathered from this is most of the hedgies' problem results from a simple change in sign. I take this a bit further and apply it to the exponential and log curves later on. I figure that the inverse of these functions is what fucked up what the algorithm originally intended.

*Exponential & Logarithmic Graphs*

The following list has the floors calculated by [u/JTH1](https://redditpreview.com/u/JTH1) (aka "exponential floor guy") and the inverted version of the curve I hypothesize the hedgies originally had planned:

[![r/Superstonk - Math Black Magic Vol 2: The Limit Does not Exist!](https://preview.redd.it/a86fowc6eg471.png?width=1291&format=png&auto=webp&s=ddee910bdcee8a375241290b7608a740ad57736d)](https://preview.redd.it/a86fowc6eg471.png?width=1291&format=png&auto=webp&s=ddee910bdcee8a375241290b7608a740ad57736d)

Ape & Hedgie Curves

Based on this inverse hypothesis, I think this is the ideal curve hedgies wanted:

[![r/Superstonk - Math Black Magic Vol 2: The Limit Does not Exist!](https://preview.redd.it/ys4mcl3mgh471.png?width=983&format=png&auto=webp&s=95a47f214cc84052888c2cf2182d910e3df536ed)](https://preview.redd.it/ys4mcl3mgh471.png?width=983&format=png&auto=webp&s=95a47f214cc84052888c2cf2182d910e3df536ed)

Hedgie Curves

If you want to see the current curve, check out exponential floor guy's posts (the most recent at the time of this writing is linked at the very top of the post).

D. Pareto Principle & Rate of Change

(This section is based heavily on a comment by sososhibby. This section makes a lot more sense if you read it. Its linked at the top.)

*Hedgie Case*

I thought it was interesting that the author stressed throughout the paper, that price is reduced CLOSE to zero and not zero.

Remember, in separated equilibrium naked shorting drops the price by a third, then halves it before it quickly drops close to zero.

That sounded like asymptotic behavior (asymptote = the thing the curve has to approach for the limit to exist, remember *Mean Girls?*), so I was curious to see the progression to zero so I kept it going and halved *P(2)* again and repeated the process with my result. I assume this is happening quickly between time 2 and time 3:

[![r/Superstonk - Math Black Magic Vol 2: The Limit Does not Exist!](https://preview.redd.it/2o17ngi8lh471.png?width=973&format=png&auto=webp&s=1f44aafd13eb3f81ccb7f1f4db0214a41d84edd0)](https://preview.redd.it/2o17ngi8lh471.png?width=973&format=png&auto=webp&s=1f44aafd13eb3f81ccb7f1f4db0214a41d84edd0)

[![r/Superstonk - Math Black Magic Vol 2: The Limit Does not Exist!](https://preview.redd.it/ero04mjalh471.png?width=910&format=png&auto=webp&s=9aa8b4836a4a7b880224998176146a060b2a65e3)](https://preview.redd.it/ero04mjalh471.png?width=910&format=png&auto=webp&s=9aa8b4836a4a7b880224998176146a060b2a65e3)

Price Progression to Close to Zero

I'd take it further but you get the picture. So I took the points made a scatter plot. Didn't look like much. I got curious and wanted to see if I could fit the negative exponential curve. I had to use some scaling factors, but always try to base them as a proportion of 1.

[![r/Superstonk - Math Black Magic Vol 2: The Limit Does not Exist!](https://preview.redd.it/ekvd81pmlh471.png?width=876&format=png&auto=webp&s=8c1448d0d623d47ca188bbf95a5e38596b682d2a)](https://preview.redd.it/ekvd81pmlh471.png?width=876&format=png&auto=webp&s=8c1448d0d623d47ca188bbf95a5e38596b682d2a)

[![r/Superstonk - Math Black Magic Vol 2: The Limit Does not Exist!](https://preview.redd.it/4ell2arrlh471.png?width=834&format=png&auto=webp&s=7e10e0d89e6c936605b574fe7bfe56cc738fbbd7)](https://preview.redd.it/4ell2arrlh471.png?width=834&format=png&auto=webp&s=7e10e0d89e6c936605b574fe7bfe56cc738fbbd7)

Hedgie Curve

Didn't look like much either, but the fact that it had asymptotic behavior at 0.2 or 20 percent. I figured it might be worth mentioning. Maybe somebody else can take it further.

*Ape Case*

Remember, in the normal case of naked shorting in separating equilibrium the price is dropped by a third, then halved, then taken close to zero.

In the ape case, the price increases. This is where the exponential/power function may come into play. I tried to find the rate of change by re-computing values using equations from earlier:

[![r/Superstonk - Math Black Magic Vol 2: The Limit Does not Exist!](https://preview.redd.it/wpa0e8femh471.png?width=1056&format=png&auto=webp&s=ffb70662e8d057f9ecefcdca7b73ba7c913a845c)](https://preview.redd.it/wpa0e8femh471.png?width=1056&format=png&auto=webp&s=ffb70662e8d057f9ecefcdca7b73ba7c913a845c)

[![r/Superstonk - Math Black Magic Vol 2: The Limit Does not Exist!](https://preview.redd.it/c7cnltihmh471.png?width=975&format=png&auto=webp&s=fcfce22cebd58f6b95457afe6dafca3b775a1a38)](https://preview.redd.it/c7cnltihmh471.png?width=975&format=png&auto=webp&s=fcfce22cebd58f6b95457afe6dafca3b775a1a38)

Ape Case

As with the last set of values, I wanted to examine the behavior of the ape curve to find a rate of change. It looks like the price increases by a third, then by 1.25 or 25 percent.

[![r/Superstonk - Math Black Magic Vol 2: The Limit Does not Exist!](https://preview.redd.it/pekkb7kvmh471.png?width=910&format=png&auto=webp&s=679c9df194127816f03002feb58a8159c88a012a)](https://preview.redd.it/pekkb7kvmh471.png?width=910&format=png&auto=webp&s=679c9df194127816f03002feb58a8159c88a012a)

To the Moon!

I did the same process of scatter and fitting curve this time with the exponential:

[![r/Superstonk - Math Black Magic Vol 2: The Limit Does not Exist!](https://preview.redd.it/m9sioly1nh471.png?width=903&format=png&auto=webp&s=18f5889fcf4610d3c84b4de88f05dc9d1cc370de)](https://preview.redd.it/m9sioly1nh471.png?width=903&format=png&auto=webp&s=18f5889fcf4610d3c84b4de88f05dc9d1cc370de)

Ape Curve

Also, not sure if there's anything here, but the number 0.8 or 80 percent stood out to me. Need more wrinkled feedback.

-----------------------------------------------------------------------------------------------------------------------------------------------------

E. Impossible to Short to Zero

I can use the same process as earlier to find the amount of shares needed to short the ape curve close to zero:

[![r/Superstonk - Math Black Magic Vol 2: The Limit Does not Exist!](https://preview.redd.it/58fozggdnh471.png?width=989&format=png&auto=webp&s=69af8afc934a8c1bd51b42578ddf226dbc6acf52)](https://preview.redd.it/58fozggdnh471.png?width=989&format=png&auto=webp&s=69af8afc934a8c1bd51b42578ddf226dbc6acf52)

Shares Needed to Zero

These expressions violate our curve rules from earlier. All elements cannot be negative.

[![r/Superstonk - Math Black Magic Vol 2: The Limit Does not Exist!](https://preview.redd.it/1ctkekv0oh471.png?width=938&format=png&auto=webp&s=9c66d9b4480d5a16c79b715e709d08516d654862)](https://preview.redd.it/1ctkekv0oh471.png?width=938&format=png&auto=webp&s=9c66d9b4480d5a16c79b715e709d08516d654862)

Da Rules

This seems to imply that if apes continue to BUY & HODL the price cannot go to zero. It is mathematically impossible.

*Negative Volume*

This is a connection I just made today, so I'll have to shoehorn it in here.

For the last several months, negative volume will show up in the data feeds for various apes. [This](https://www.reddit.com/r/Superstonk/comments/nwta9j/what_is_this_fuckery_can_anyone_explain_a/) is the most recent incident.

Now Dave Lauer did say that those were most likely end of the day rebalancing and whatnot, so I'm not suggesting anything tin foil-y.

My hypothesis is simply that the negative candle is the manifestation of the algo doing something based on these curves. I don't know the algo is doing and I don't know if it is nefarious or not. I def need wrinkle brain feedback here.

-----------------------------------------------------------------------------------------------------------------------------------------------------

F. The Final Volume

The final volume will be the shortest, but the juiciest. Based on what we've discussed, there may be a way to calculate how many shorted shares there are and find out the true short interest.

-----------------------------------------------------------------------------------------------------------------------------------------------------

TL:DR -> At this point, the number of shares needed to short $GME to zero does not mathematically exist.

TA:DR -> $GME only go up! Math say so!

--------------------------------------------------------------------------------------------------------------------------------------------------------

This post brought to you on behalf of Margery Nesbitt. Help her find Kenny, he isn't taking her calls for some reason...
