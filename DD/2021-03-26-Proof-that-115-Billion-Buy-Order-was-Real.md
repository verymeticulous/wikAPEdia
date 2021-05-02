More Proof the $115 Billion Buy Order WAS REAL and how HFs use HFT to Manipulate GME through One Specific Order Type.
=====================================================================================================================

| Author       | Source       | 
| :-------------: |:-------------:|
| [u/jsmar18](https://www.reddit.com/user/jsmar18/)| [Reddit](https://www.reddit.com/r/GME/comments/mdnph0/more_proof_the_115_billion_buy_order_was_real_and/) | 

---

[DD](https://www.reddit.com/r/GME/search?q=flair_name%3A%22DD%22&restrict_sr=1)

Putting this at the top because it's important.

Edit: I love us. [u/TendieTard](https://www.reddit.com/u/TendieTard/) commented an awesome [youtube video](https://www.youtube.com/watch?v=kFQJNeQDDHA). Skip to minute 29 and watch for the next 15-20 minutes. It explains how order types basically skew the system towards those making the trades. This is real. This perpetuates inequality within the market by disenfranchising retail investors.

THIS NEEDS TO CHANGE. We talk about equality so much in this big wide world and it should apply to every single corner of this world. Including our financial markets. We CANNOT allow exchanges to exploit inequality to make money off of us.

Edit: To reiterate this, and boy am i half asleep. They are covering their positions with naked shares right? What does that mean.... FTDs.... What do FTDs mean...? ETFs.... eventually there will be an end. There is a legit physical limit because none of these are a "full loop", nothing actually covers the real problem which is their initial fucking short position. So I see it going FTDs implode -> naked shares implode -> GME explodes in the best way possible. HODL.

Not financial advice. Ofc.

---------------------------------------------------------------------------------------------------------------------

Here I lay out an in-depth analysis of order types, order types are an important part of a HFs strategy. Exchanges actually market different order types as a means for attracting business, but alas - they are suseptible to being misused.

I actually went down this analysis path in an attempt to prove the TD TOS volume from [why the $115 Billion buy order was not a bug](https://www.reddit.com/r/GME/comments/mcu6et/why_the_115_billion_buy_order_was_not_a_bug_do/), but also happened to find another extremely interesting tidbit

Let's get started.

First, we need to understand a few things which will give some context to this. As we all know GME is listed on the [NYSE exchange](https://www.nyse.com/index). What you might not know is that the NYSE exchange is comprised of different exchanges:

-   NYSE

-   NYSE Arca

-   NYSE National

-   NYSE American

-   NYSE Chicago

The best part about this is NYSE started to release reporting on order types early last year, which allows us to analyse the % of different types of orders being placed. You can probably see where this is going...

NYSE Chicago is the most interesting because:

1.  It has the lowest volume of equities being traded ~5-20m per day (compared to NYSE 1b+)

2.  Due to this it's easier to see how trading strategies emerge based on the order types used

3.  Our beloved friend Shitadel is based in Chicago

The following analysis is formed on the basis that Shitadel, being a market maker based in Chicago, likely deals with the majority of the NYSE Chicago's exchange volume. Therefore assuming any patterns we identify is actually them.

Delving into NYSE Chicago Order Types

The table below shows us the % distribution of these high-level order types for the past 6 months. We can observe that between Sep-20 and Oct-20 there was a monumental shift in order behaviour that's remained the same to our current date ASWELL as the slow increase in % of Non-Displayed Limit orders each month.

What happened between Sep-20 and Oct-20? GME started lighting the boosters for take-off.

[![r/GME - More Proof the $115 Billion Buy Order WAS REAL and how HFs use HFT to Manipulate GME through One Specific Order Type.](https://preview.redd.it/ay2md51n6dp61.png?width=799&format=png&auto=webp&s=7bbfb6ddc4b9621b54f4630bc5c05ba08218c516)](https://preview.redd.it/ay2md51n6dp61.png?width=799&format=png&auto=webp&s=7bbfb6ddc4b9621b54f4630bc5c05ba08218c516)

This is also when [u/DeepFuckingValue](https://www.reddit.com/u/DeepFuckingValue/) started to see traction majorly gain in his posts jumping from around 3k upvotes per post up to 16.1k upvotes on Oct 8th 2020.

[![r/GME - More Proof the $115 Billion Buy Order WAS REAL and how HFs use HFT to Manipulate GME through One Specific Order Type.](https://preview.redd.it/nmxhmhqo6dp61.png?width=789&format=png&auto=webp&s=c14550788477463e0e1e7c1a03c51e732511b77f)](https://preview.redd.it/nmxhmhqo6dp61.png?width=789&format=png&auto=webp&s=c14550788477463e0e1e7c1a03c51e732511b77f)

Understanding Order Types

Sorry apes, we're gonna have to get a bit technical here. Let's understand this fancy order type terminology before going any further.

Immediate or Cancel (IOC) = An order to buy or sell stock that MUST be executed immediately. Any portion of an IOC order that cannot be filled immediately will be cancelled.

Displayed Limit = An order to buy or sell stock at or better than a specified price, these orders are visible to the public.

Non-Displayed Limit = An order to buy or sell stock at or better than a specified price, these orders are HIDDEN.

So what does this tell us based on the change in order behaviour of the NYSE Chicago? Suddenly there's a shift away from IOC orders to Limit orders AND we're seeing a huge increase in the number of HIDDEN LIMIT ORDERS.

Big whoop? What does this prove?

Let's go one step deeper

We have more order types than just the three above, they are just overarching groups.

[![r/GME - More Proof the $115 Billion Buy Order WAS REAL and how HFs use HFT to Manipulate GME through One Specific Order Type.](https://preview.redd.it/517tllfq6dp61.png?width=791&format=png&auto=webp&s=90edcf8f903def9f7c48e803bf098ad3a8c49cf2)](https://preview.redd.it/517tllfq6dp61.png?width=791&format=png&auto=webp&s=90edcf8f903def9f7c48e803bf098ad3a8c49cf2)

Above we have even more data to play with. I've highlighted in yellow where we see the major shifts in % distribution.

In Immediate or cancel we see distribution shift to IOC ISO in October [20.21% -> 40.95%], within displayed limit orders we see a huge increase in Limit [8.92% -> 19.73%] and Non-routable limit [6.32% -> 11.68%] orders (all of these taking % share away from Limit non-routable IOC, which means the majority of orders pre Sep-20 were trading purely within NYSE Chicago). Lastly we have the steady increase in Non-displayed limit orders.

THIS IS WHERE IT GETS INTERESTING.

IOC ISO Orders

[Intermarket sweep order](https://ibkr.info/article/1734)'s are generally a large quantity order that is sent to multiple exchanges.This is how it functions:

-   An order is submitted in the pre market to sell at a price of 40.80 and is sent to exchange A.

-   The best offer price on exchange A is 40.63.

-   Exchange B receives an intermarket sweep order to buy 800 shares of the stock at a limit price of 40.88.

-   The best offer price on exchange B is 40.88

*The trader that enters the intermarket sweep order would be required to fulfill their Regulation NMS requirement by executing the maximum available quantity on exchange A at 40.63 and then may execute the balance of the order on exchange B at 40.88 even though it is at a price that is inferior to the 40.80 order resting in the book on exchange A. The 40.80 price is not the inside quote and is therefore not "protected" in terms of the balance of the sweep order executing at exchange B at a price of 40.88.*

So in monke speak, it fills the lowest alternate exchange price before filling the order at the higher price. Now, this is getting scarily close to what [u/I-had-a-Thought19](https://www.reddit.com/u/I-had-a-Thought19/) was theorizing about the HUGE TD TOS volumes of 634M @$182 in the following post. <https://www.reddit.com/r/GME/comments/mcu6et/why_the_115_billion_buy_order_was_not_a_bug_do/>.

The missing piece of the puzzle is how they control the price which leads us to our next two order types.

Displayed Limit Orders and Non-Routable Limit Orders.

These are straight forward, they are visible orders which are placed to buy/sell stock at a particular price. Non-routable again meaning not changing exchange out of NYSE Chicago in this case.

These two saw a huge move in distribution come Oct-20 as well, previously sitting at <15% of volume, now representing 30%+ worth of volume.

I believe they are using a combination of IOC ISO orders with displayed limit orders to create the perceived effect of covering. Here's the logic using the 634M @$182 as an example:

1.  Set-up a string of Non-routable sell limit orders on NYSE Chicago

2.  Set-up a string of limit sell limit orders on NYSE Chicago

3.  Make sure what's being sold are naked shares

4.  Place a huge fucking IOC ISO buy order @$182

5.  Hope that the IOC ISO buy order gobbles up all the naked sell orders, therefore making it look like they've covered. It might even gobble up some real shares as a bonus for them

There's probably some intricacies at play there in terms of how they set-up the non-routable vs routable sell limit orders to get maximum bang for buck.

THIS IS THEORY 1.

They place such large IOC ISO orders in hope they somehow trigger a chain reaction and try to cover as much of their short position as possible relative to the amount of limit sell orders they have placed to control it.

It all makes sense why we magically see such huge orders pop up, because they are shoving through ISOs which get shot out to every exchange that has GME listed and it has been likely happening SINCE OCTOBER.

This is also backed up through this quote from [IB](https://ibkr.info/article/1734).

*"Traders may see, on occasion, execution prices reported to time and sales that are at price levels through an order that they may have had working at the time."*

They then keep using them as their regular order tool as it's beneficial to try and sweep up as many shares as possible - only using it for the huge orders when they've got a good set-up in place. Kinda like how TA traders look for entry points, there are certain times when it's better to go all in.

[u/stormshawty](https://www.reddit.com/u/stormshawty/) - fuck me up fam, I hope I've done you proud.

Do you think I'm mother fucking done though?

Hell no. Let's move onto our last victim. Motherfucking Limit Non Displayed Orders.

Motherfucking Non Displayed Limit Orders

Let's start off with the chart below. These mofos haven't just been increasing on the NYSE Chicago but on every single other NYSE exchange since October-20. This shit is definitive proof that Shitadel and friends have been using HFT to manipulate the price of GME and I'll explain why.

[![r/GME - More Proof the $115 Billion Buy Order WAS REAL and how HFs use HFT to Manipulate GME through One Specific Order Type.](https://preview.redd.it/qa3vcasw6dp61.png?width=778&format=png&auto=webp&s=3aba013bc3407e898f16221d9f089ceff2c1ab42)](https://preview.redd.it/qa3vcasw6dp61.png?width=778&format=png&auto=webp&s=3aba013bc3407e898f16221d9f089ceff2c1ab42)

A regular displayed limit order or IOC is visible to all us apes. They are also prohibited from locking or crossing the market?

WTF is locking or crossing the market?

If an offer for GME at $x is already on another exchange (NYSE Chicago), another exchange (NYSE National) cannot post a bid for $x or higher as it creates a locked or crossed market respectively. Another way to say this is, shit becomes out of sync, which ain't good.

If someone tried to place such an order that I explained above, that order will be "slidden" until it no longer causes a [lock or cross situation](https://www.investopedia.com/terms/l/lockedmarket.asp). Slides are considered cancellations because of this and will reset the timestamp associated with it.

These regulations ensure that there is a bid/ask spread, guaranteeing the traders the cost of that spread in a size at least the minimum tick.

BUT WHAT ABOUT NON DISPLAYED ORDERS???

Calm down.

Hidden (Non-display) orders don't have any of these regulations... This means the HFT (high frequency traders) can effectively jump the line by posting ["hide not slide"](https://docs.google.com/document/d/1QmoFpdq9HeGJ-cdPP7y808uWxVufJNr2b69J0GY_-SQ/edit?usp=sharing) orders instead of visible orders. This is because a hidden order will not be slidden, resetting the timestamp. So if i placed an order in the scenario above at $120.01 for GME, they then place a hidden order for $120.01 as well, I get my timestamp reset as i've placed a locked/cross order, but the hidden order does not get their timestamp reset therefore essentially skipping the fucking line.

THIS IS THEORY 2.

Monke speak: They get in front of the order book to benefit their HFT strategy of driving GME down in price so efficiently.

I've calculated the order volume from the Limit Non Display Orders - subtracting the "pre GME spike" %s (September as that's all i have) so that it's essentially assuming anything on top of the Septembers' base % (the MoM increases in the chart above) are assumed to basically be GME related.

[![r/GME - More Proof the $115 Billion Buy Order WAS REAL and how HFs use HFT to Manipulate GME through One Specific Order Type.](https://preview.redd.it/qwr05psy6dp61.png?width=788&format=png&auto=webp&s=94046d001fef927805d79348204db395d7139594)](https://preview.redd.it/qwr05psy6dp61.png?width=788&format=png&auto=webp&s=94046d001fef927805d79348204db395d7139594)

Let's also checkout GME trading volume....

[![r/GME - More Proof the $115 Billion Buy Order WAS REAL and how HFs use HFT to Manipulate GME through One Specific Order Type.](https://preview.redd.it/0x9g79d07dp61.png?width=442&format=png&auto=webp&s=ed73d6565d8fa9d49d0eae8aaccdbf4518bda75f)](https://preview.redd.it/0x9g79d07dp61.png?width=442&format=png&auto=webp&s=ed73d6565d8fa9d49d0eae8aaccdbf4518bda75f)

Well, wouldn't you look at that, it's actually reasonable that that monthly volume could have all been used in GME alone to manipulate its price for the past three months.

That's it.

Takeaways:

1.  More evidence to support [u/I-had-a-Thought19](https://www.reddit.com/u/I-had-a-Thought19/) theory, in that they are using IOC ISO orders which cause the huge volumes we see come through in TD TOS feeds

2.  In my eyes, definitive proof that HFs are using HIDDEN ORDERS in their HFT strategy to manipulate GMEs price.

Hopefully, I've added more fuel to your confirmation bias, because I sure as fucking have dumped a truckload on myself.

Poke holes into this analysis, question it. More than happy to have a discussion to see how this can further evolve. [u/rensole](https://www.reddit.com/u/rensole/), this be the DD i was referring to.

Edit: a word.

Edit: For people worried about hidden orders, and them just covering without us knowing. This is wrong. It's actually the best fucking point. They can't do this as WE BE A HODL'ING.

Edit: To clarify "covering their position" They're walking a fine fucking line. They need to create the perceived effect of covering shorts but they're covering with naked shares (not real shares), so whenever they do this (theory 1 in my post) - they walk an extremely fine line between us walking away with the momentum and the price exploding and them being safe for another week. All we need to do is HODL to win once, but they need to win every single time they do this.

Edit: I'll be asleep during the AMA could people ask old mate on his thoughts about HFs using hidden order types to manipulate GME and how exchanges offering order types retail investors can't access perpetuates inequality within the stock market. Please and thankyou!!!

Edit: I love us. [u/TendieTard](https://www.reddit.com/u/TendieTard/) commented an awesome [youtube video](https://www.youtube.com/watch?v=kFQJNeQDDHA). Skip to minute 29 and watch for the next 15-20 minutes. It explains how order types basically skew the system towards those making the trades. This is real. This perpetuates inequality within the market by essentially, disenfranchising us retail investors.

THIS NEEDS TO CHANGE. We talk about equality so much in this big wide world and it should apply to every single corner of this world. Including our financial markets. We CANNOT allow exchanges to exploit inequality to make money off of us.

Edit: To reiterate this, and boy am i half asleep. They are covering their positions with naked shares right? What does that mean.... FTDs.... What do FTDs mean...? ETFs.... eventually there will be an end. There is a legit physical limit because none of these are a "full loop", nothing actually covers the real problem which is their initial fucking short position. So I see it going FTDs implode -> naked shares implode -> GME explodes in the best way possible. HODL.

Not financial advice. Ofc.
