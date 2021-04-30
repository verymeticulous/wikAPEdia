I Was Missing a KEY Piece of the Puzzel. This is how HFTs are covering FTDs and Why the TD TOS "Bugs" are NOT What We Think They Are.
=====================================================================================================================================

**Author: [u/jsmar18](https://www.reddit.com/user/jsmar18/)**

**[Source](https://www.reddit.com/r/GME/comments/mf1f6n/i_was_missing_a_key_piece_of_the_puzzel_this_is/)**

[DD](https://www.reddit.com/r/GME/search?q=flair_name%3A%22DD%22&restrict_sr=1)

3/29 Edit: Just want to say, almost everything on this subreddit is speculative. DD researchers do their best to bring new information to light, however the financial market is one of the most complex artificial ecosystems humans have created. You can't resonably expect everything to be right, it's okay to be wrong, as long as we acknowledge it and take it in our stride. We're bayesian thinkers by nature afterall (or at least i like to think so).

We update our beliefs based on new evidence being presented, as such i've had some great conjecture shown to me in particular relating to the ever present TD TOS "glitch". So i'm adjusting my post to reflect this new information.

---------------------------------------------------------------

My previous post's theories were ¼ right~~, but it was missing something extremely important. That being~~ ~~*Add Liquidity Only orders*~~ ~~and Supplemental Liquidity Providers (SLP) which explains:~~

1.  ~~Why we see huge "volume" pop up on TD TOS for GME~~

2.  ~~Why we see huge "volume" pop up on TD TOS for other stocks~~

3.  ~~Why we see it in the "volume" column with no buy/sell orders lodged against it~~

4.  Why this "volume" can't be used to calculate short interest, potential prices or whatever other

~~The middle two being points where people still had questions around and the latter other posters speculating and using them incorrectly (nothing wrong with that, this sub is about improving all our analysis when new information is found!).~~

3/29 Edit: Keep reading on and take in the edits, you'll understand why i've striked this out. I've left 4 unstriked as the TOS TD volume still should not be used in DD posts until it's been 100% concretely clarified what it is.

Now, this will be a long read which is why I'm trying to get it out on a Sunday for people to consume and take it in before the market opens.

Thanks to [u/SmithEchoes](https://www.reddit.com/u/SmithEchoes/) for collaborating with me on this DD.

---------------------------------------------------------------

Acronym Legend:

NYSE = New York Stock Exchange

IOC ISO = Immediate or Cancel Intermarket Sweep Order

ALO = Additional Liquidity Order

SLP = Supplemental Liquidity Provider

TD TOS = TD Ameritrade Think Or Swim

MM = Market Maker

HFT = High Frequency Trading

FTD = Failure to Deliver

MSM = Mainstream Media

---------------------------------------------------------------

Let's get into it!

The same assumption regarding NYSE Chicago being a sandpit for Shitadel and co remains the same from my [previous post](https://www.reddit.com/r/GME/comments/mdnph0/more_proof_the_115_billion_buy_order_was_real_and/).

Let's recap what we saw in terms of order behaviour on this exchange over the past 6 months.

[![r/GME - I Was Missing a KEY Piece of the Puzzel. This is how HFTs are covering FTDs and Why the TD TOS "Bugs" are NOT What We Think They Are.](https://preview.redd.it/y3jcvaeczrp61.png?width=512&format=png&auto=webp&s=2d9eab1540ec5bd37c5f940cc5a4a63e986f9896)](https://preview.redd.it/y3jcvaeczrp61.png?width=512&format=png&auto=webp&s=2d9eab1540ec5bd37c5f940cc5a4a63e986f9896)

We saw volume shift away from *Limit Non-Routable IOC* to:

1.  IOC ISO

2.  Limit Non-displayed

3.  Add Liquidity Only (ALO)

These three order types are the keys to the puzzle we've been needing, to figure out their strategy to manipulate GME prices. So let's start off by getting an understanding of what they are!

Bare with the explanations, pretty graphs, charts and some pretty mind boggling conclusions lay beyond the order type explanations.

IOC ISO (Immediate or Cancel Intermarket Sweep Order)

For those who have not read my previous post find an excerpt below.

[Intermarket sweep order](https://ibkr.info/article/1734)'s are generally a large quantity order that is sent to multiple exchanges.This is how it functions:

-   An order is submitted in the pre market to sell at a price of 40.80 and is sent to exchange A.

-   The best offer price on exchange A is 40.63.

-   Exchange B receives an intermarket sweep order to buy 800 shares of the stock at a limit price of 40.88.

-   The best offer price on exchange B is 40.88

*The trader that enters the intermarket sweep order would be required to fulfill their Regulation NMS requirement by executing the maximum available quantity on exchange A at 40.63 and then may execute the balance of the order on exchange B at 40.88 even though it is at a price that is inferior to the 40.80 order resting in the book on exchange A. The 40.80 price is not the inside quote and is therefore not "protected" in terms of the balance of the sweep order executing at exchange B at a price of 40.88.*

So in monke speak, it fills the lowest alternate exchange price before filling the order at the higher price.

To make it more complicated this is an order with a modifier (ISO is the modifier), so let's understand an IOC.

These are orders which attempt to execute immediately and cancel any unfilled portion. E.g. place a buy for 10 @ $180.01 , it's only able to be filled to a portion of 5 @ $180.01 and then canceled straight away.

A key part to these types of orders is derived from the following.

*"The intermarket sweep exception enables trading centers that receive sweep orders to execute those orders immediately, without waiting for better priced quotations in other markets to be updated."*

This is [derived from a response](https://www.sec.gov/comments/sr-nyse-2014-32/nyse201432-2.pdf) to change how ALOs work by the NYSE, as they've been a thorn in their side since 2014. A prelude to what we'll go into later. Sounds suspicious right?

**nudge nudge* Almost like they'd be handy for HFTs *nudge nudge**

Limit Non-displayed

An order to buy or sell stock at or better than a specified price, these orders are HIDDEN from us apes and others. They also don't care about [lock or cross situation](https://www.investopedia.com/terms/l/lockedmarket.asp) cases. Refer to [previous post](https://www.reddit.com/r/GME/comments/mdnph0/more_proof_the_115_billion_buy_order_was_real_and/) for and understanding on this.

This means the HFT (high frequency traders) can effectively jump the line by posting ["hide not slide"](https://docs.google.com/document/d/1QmoFpdq9HeGJ-cdPP7y808uWxVufJNr2b69J0GY_-SQ/edit?usp=sharing) orders instead of visible orders. This is because a hidden order will not be slidden, resetting the timestamp. So if i placed an order at $120.01 for GME, they then place a hidden order for $120.01 as well, I get my timestamp reset as i've placed a locked/cross order, but the hidden order does not get their timestamp reset therefore essentially skipping the fucking line.

Yet another bread and butter tool when it comes to HFT. The key here though is the fact that it's HIDDEN and how this plays out with ALO order types (IB allows retail to place these orders as well).

Add Liquidity Only (ALO)

First of all, major thanks to [u/SmithEchoes](https://www.reddit.com/u/SmithEchoes/) on this bad boy as it's a complicated beast.

Now this order type is a doozy, and is currently being used for nefarious purposes.

ALO follows a strict "If,then" rule set based on if it locks [(7.31(e)(2)(b)iii-iv)](https://nyseguide.srorules.com/rules/document?treeNodeId=csh-da-filter!WKUS-TAL-DOCS-PHC-%7B4A07B716-0F73-46CC-BAC2-43EB20902159%7D--WKUS_TAL_19401%23teid-37) OR crosses [(7.31(e)(2)(b)ii)](https://nyseguide.srorules.com/rules/document?treeNodeId=csh-da-filter!WKUS-TAL-DOCS-PHC-%7B4A07B716-0F73-46CC-BAC2-43EB20902159%7D--WKUS_TAL_19401%23teid-37). This rule set forces the ALO to perform these trades until it is fully consumed, or the order is canceled. Rule [7.31(e)(2)(C)](https://nyseguide.srorules.com/rules/document?treeNodeId=csh-da-filter!WKUS-TAL-DOCS-PHC-%7B4A07B716-0F73-46CC-BAC2-43EB20902159%7D--WKUS_TAL_19401%23teid-37), once ALO is resting on the exchange AND it was forced to change its price in accordance with [7.31(e)(2)(b)i-iv](https://nyseguide.srorules.com/rules/document?treeNodeId=csh-da-filter!WKUS-TAL-DOCS-PHC-%7B4A07B716-0F73-46CC-BAC2-43EB20902159%7D--WKUS_TAL_19401%23teid-37) THEN it now gets to be priced in accordance with [7.31(e)(1)(A)iii and iv](https://nyseguide.srorules.com/rules/document?treeNodeId=csh-da-filter!WKUS-TAL-DOCS-PHC-%7B4A07B716-0F73-46CC-BAC2-43EB20902159%7D--WKUS_TAL_19401%23teid-37). This is the equivalent of HFT when ALO "activates" BUT it comes with a built in safety feature that IF the price goes UP(Sell ALO) or DOWN (buy ALO) the ALO limit price is no longer locking or crossing at the values it was getting moved to, it REVERTS back to its original limit order price.

Monke speak translator: These orders create sell/buy walls that have a nifty function that essentially "flips the safety switch" back to the original limit order price if too much buy/sell pressure is applied.

Funnily enough, the NYSE has tried to [amend how ALO orders work](https://www.federalregister.gov/documents/2014/10/16/2014-24547/self-regulatory-organizations-new-york-stock-exchange-llc-nyse-mkt-inc-order-approving-proposed-rule), because of how they can be used for nefarious purposes.... **cough* Shitadel *cough** The amendment would force to cancel the ALO once it crosses or locked, and not perform how it currently does in accordance with [7.31(e)(2)(b)i-v](https://nyseguide.srorules.com/rules/document?treeNodeId=csh-da-filter!WKUS-TAL-DOCS-PHC-%7B4A07B716-0F73-46CC-BAC2-43EB20902159%7D--WKUS_TAL_19401%23teid-37). Which means no buy/sell wall capability for them to use and abuse.

The last thing we needa talk about are mother fucking SLPs. This ain't an order type but it'll clear up many questions. We'll then get into analysing price action after this (the fun part).

SLP (Supplemental Liquidity Providers)

3/29 Edit: I'm still retainting this as it's factually true of how SLPs function.

Guess who can be a [SLP](https://www.nyse.com/markets/liquidity-programs)? That's right. Market Makers.

Our friend, Shitadel is a SLP.

SLPs are pretty simple to understand. They are market participants that use HFT to create high volume on exchanges in order to add liquidity to the markets. This is all done to create *tight spreads*.

SLPs such as Shitadel can artificially create liquidity in the market through explosively shitting out volume through the use of HFT methods. This is important.

[![r/GME - I Was Missing a KEY Piece of the Puzzel. This is how HFTs are covering FTDs and Why the TD TOS "Bugs" are NOT What We Think They Are.](https://preview.redd.it/jpucmp5fzrp61.png?width=510&format=png&auto=webp&s=1d95d29d66122b4c7702e4b0e8af26e7513415d0)](https://preview.redd.it/jpucmp5fzrp61.png?width=510&format=png&auto=webp&s=1d95d29d66122b4c7702e4b0e8af26e7513415d0)

Because GME liquidity has been drying up bit by bit since January-2021, Shitadel and co ~~need to use~~ can use their position as an SLP to ~~manipulate~~ add liquidity into GME~~s price as us apes are hodling~~.

The whole premise of market makers is to remain neutral and to make money through scraping cents of cents off the spread, therefore not directionally affecting the price. ~~However, if i'm on my last legs and feel like doing something illegal, I can use a mixture of the order types above in combination with SLP to manipulate GME at my will.~~

3/29 Edit: Removing this reference as i've been unable to dig up any prior evidence that suggests MM who are SLPs have used their position for maket manipulation.

SLP and Our Beloved TD TOS "Errors"

3/29 Edit:

I've only ever seen screenshots of the TD TOS error. SLP and the TD TOS made alot of sense to me given i viewed it as a sort of reserve volume that does not nessecarily need to be used.

I was shown a video of it occuring for the first time and it's changed my opinion on what it is entirely, *IT DOES NOT LOOK LIKE IT'S SLP VOLUME*. I won't speculate in this post about it any further other than saying it should not be used in DD again until it has been 100% concrete clarified what it is. I have therefore adjusted this post to reflect this new beliefs as the order type content and HFT manipulation is still valid given evidence it exists and obviously order types are a thing.

~~Let's clear up this TD TOS situation once and for all as I'm HIGHLY certain this is exactly what we're seeing.~~

~~As we've said above, Shitadel and co can explosively shit volume into the market. This is exactly what we're seeing flow through TOS.~~

~~Myth 1. "BuT iT IsN'T BuY oR sELl"~~

~~It's neither a sell or a buy because it's both~~~~. Which is why we see no buy orders or sell orders in TOS in the example below. It's also why we can't project prices using it, so any post you see trying to do that to justify the value of GME, it's just not true as not all of it needs to be executed. Apologies.~~

[![r/GME - I Was Missing a KEY Piece of the Puzzel. This is how HFTs are covering FTDs and Why the TD TOS "Bugs" are NOT What We Think They Are.](https://preview.redd.it/m3a2sgxgzrp61.png?width=632&format=png&auto=webp&s=6a6b8d5a088a836db8fcb5c5da0008b78e548d05)](https://preview.redd.it/m3a2sgxgzrp61.png?width=632&format=png&auto=webp&s=6a6b8d5a088a836db8fcb5c5da0008b78e548d05)

~~Myth 1. "BuT iT hAppEnS to OtHEr TiCkeRs"~~

~~It's also commonplace within the market, which is why we see it pop up for other stocks. In general, SLP is good because it does create those tighter spreads. But it sure as hell can be used for manipulation if the SLP wants to take illegal risks to shake retail investors from a certain stock~~ ~~**cough* GME *cough**~~~~.~~

[![r/GME - I Was Missing a KEY Piece of the Puzzel. This is how HFTs are covering FTDs and Why the TD TOS "Bugs" are NOT What We Think They Are.](https://preview.redd.it/8t1t4wzhzrp61.png?width=636&format=png&auto=webp&s=d1d1fcf0a6af0a70e82744c2037b0fd6383940cf)](https://preview.redd.it/8t1t4wzhzrp61.png?width=636&format=png&auto=webp&s=d1d1fcf0a6af0a70e82744c2037b0fd6383940cf)

Rewind.

Now we know what we're talking about, let's go back to this table. A very juicy pattern starts to emerge which is the huge increases we see in ALO distribution.

[![r/GME - I Was Missing a KEY Piece of the Puzzel. This is how HFTs are covering FTDs and Why the TD TOS "Bugs" are NOT What We Think They Are.](https://preview.redd.it/fwr7cswjzrp61.png?width=506&format=png&auto=webp&s=fe7d3ba75b4014d179c36c6cf995b145bf47fe34)](https://preview.redd.it/fwr7cswjzrp61.png?width=506&format=png&auto=webp&s=fe7d3ba75b4014d179c36c6cf995b145bf47fe34)

When we look at historical *NYSE Chicago volume*, we see visible step changes in the highs that sussly match up with ALOs monthly increases.

[![r/GME - I Was Missing a KEY Piece of the Puzzel. This is how HFTs are covering FTDs and Why the TD TOS "Bugs" are NOT What We Think They Are.](https://preview.redd.it/n98d42zkzrp61.png?width=622&format=png&auto=webp&s=76d4b13baaf6e2e2bfb57c84518083f3b74fef41)](https://preview.redd.it/n98d42zkzrp61.png?width=622&format=png&auto=webp&s=76d4b13baaf6e2e2bfb57c84518083f3b74fef41)

This leads me to believe they are using ALOs as a buy/sell wall in level 2 data, which helps them to control momentum. However ALOs need to be timed well, as they could be blown away due to pressure from other parties.

So what are the tools that our HFs buddies have to manipulate the price?

1.  IOC ISO orders

    1.  Cross exchange sweep that allows them to get ahead of the order queue to an extent

    2.  Used as buy/sell pressure when needed

2.  Limit non-displayed orders

    1.  A hidden order that does not affect the price

    2.  Used to offset IOC ISO orders so as a market maker they can remain "neutral" without causing buy/sell pressure

3.  ALO orders

    1.  A order placed to create a buy/sell wall

    2.  Used to stop momentum and turn the trend around

Here are the players which they need to factor into their strategy:

1.  Retail investors 📈🐒

    1.  Likely displaying a predictable buying pattern by now

2.  Long Whales 📈🐳

    1.  Shitadel and Co likely know the strategy they are trying to employ (outside of sporadic buy pressure from the equitie side of things

3.  Other parties such as day traders 📉👿

    1.  *Don't day trade GME for the love of everything good in this world*

Let's put it all together!!!!!

3/29 EDIT: Based on my TD TOS Update above, disregard the TOS Volume i've highlighted in the picture below. The strategy breakdowns logic following the picture however can still be applied to the movements highlighted in the pink rectangles.

[![r/GME - I Was Missing a KEY Piece of the Puzzel. This is how HFTs are covering FTDs and Why the TD TOS "Bugs" are NOT What We Think They Are.](https://preview.redd.it/lmyg2mqmzrp61.png?width=634&format=png&auto=webp&s=f6704aefbe17b150cd44df6dc631e3bb4985ca84)](https://preview.redd.it/lmyg2mqmzrp61.png?width=634&format=png&auto=webp&s=f6704aefbe17b150cd44df6dc631e3bb4985ca84)

~~I'm taking the three most recent observations of SLP volume from TOS and have marked them on a GME 1 hour candle chart.~~ It's pretty telling looking at this straight away what's going on~~. At each of the specific candles i've highlighted, we see a~~~~*wall*~~ ~~being hit and a reversal in price.~~

3/29 Edit: Let's check out the on the graph above where we see major swings in prices. These are highlighted in the pink rectangles.

Strategy Breakdown

~630M @~$181

1.  Place ALO sell order to create a wall in preparation for earnings in after market

2.  Use HFT IOC ISO sell order to create downward pressure during earnings call and after

3.  Use HFT Limit Non-Display buy order to remain "neutral" without creating any upward pressure

~113M @~$120

1.  Place IOC ISO buy order to buy up shares on the way up

2.  Place Limit buy order to buy up shares on the way up

~290M @~$183

1.  Place ALO sell order to create a wall to reduce upward pressure

2.  Use HFT IOC ISO sell order to create downward pressure

3.  Use HFT Limit Non-Display buy order to remain "neutral" without creating any upward pressure

The question is WHY are they doing this?

FTDs.

The shorts know they have to cover a certain amount of FTDs out of pocket each [cycle](https://iamnotafinancialadvisor.com/Current-DD/), they naturally want the price as low as possible in order to do this. Cover implies whatever they could not borrow to use towards covering their FTDs.

Yep, you read that right ape.

Those screenshots you see from iborrow with borrowed shares disappearing ain't being used to short the stock, they are being used to cover their FTDs.

On that bombshell, back to HFT. As mentioned above, they'd want to manage buy pressure and keep the price as low as possible so they sweep up some shares at the lowest price they can.

~~This is what's happening from the first SLP Volume coming through in the picture above~~. Drop the price, then at the point they can't drop it much further they start sweeping up shares with IOC ISOs and regular limit orders to cover the rest of their FTDs they could not through borrowing. Lastly, they needa put a cap on this so it does not get out of control, so they create a sell wall and start to work the price back down again.

They knew Earnings Release was a good bet to tank the price, they had it all planned out, from the PR campaign MSM was running to even profiting off the spread from the decline to the bounce. ~~due to them adding liquidity into the market as a~~ ~~SL-fucking-P~~.

3/29 Edit: They can still manipulate the price regardless of whether [they are a SLP or not](https://www.sec.gov/news/press-release/2014-229). My theory is that they're using their positions as SLPs for further nefarious purposes - but there is no proof, so i'm stripping it until any evidence comes to light.

Theory time (this whole post is, but humour me as I have the PERSONAL belief the above is fairly on point, do your own DD to confirm 😉 ).

Theory 1 | We Will See It Again

As FTDs are cyclical we will see this behaviour moving forward until the bubble bursts as the FTD cycle slowly grows out of their control. HODL.

~~I base this on the fact that I believe if we had noticed the SLP volume sooner we would be able to match this whole post to exactly what happened in late February below (with a few variations in strategy dependent on their options spread).~~

3/29 Edit: I still believe this to be true, the run up in the chart below and the "flash crash" we saw is far too obvious in terms of what they were trying to accomplish. I believe they were apply buy pressure to drive the price up, likely grabbing what shares they can in the process to cover their FTDs, before dropping the price drastically within minutes (of which there are sevrel possible methods of doing based on what i understand, however i will not speculate until i've looked into the details of it).

[![r/GME - I Was Missing a KEY Piece of the Puzzel. This is how HFTs are covering FTDs and Why the TD TOS "Bugs" are NOT What We Think They Are.](https://preview.redd.it/6fltgujozrp61.png?width=634&format=png&auto=webp&s=c5b38abb929ece9d9c8533e8b79aab0ef0498396)](https://preview.redd.it/6fltgujozrp61.png?width=634&format=png&auto=webp&s=c5b38abb929ece9d9c8533e8b79aab0ef0498396)

Theory 2 | Options and Long Whales

Shorts are trying to balance two plates.

1.  Covering FTDs

2.  Making money to cover those FTDs through options

They are carefully managing how they can use their HFT strategy using their status as a SLP and to make money on options as well to fund covering FTDs among other things like paying employees etc..

This is where the long whales come in, historically in MY EYES, whales are responsible for the spike in price on the 24th February to just under the $200 mark. Since then and much before, they contributed little volume. It's entirely made up of HFT and retail investors buying.

Where they do play into this and i think is a valid theory is using their weight when it matters to inflict [max pain](https://www.reddit.com/r/GME/comments/mejp0k/the_concept_of_max_pain_and_why_this_is_probably/) (post suggest whales pushed up price, that's not true based on everything in this post, but it's entirely valid that they slowed it down so the price upon market close on friday would inflict max pain).

Conclusion

Wow, that was a lot. As such, take time to take it in and properly understand it. As always, PM or comment and I'll clear things up as best I can.

This has been going on since as early as October when we first witnessed a huge shift in order strategy. SLPs are meant to be a "good" thing for the market, ~~but as always, there is room to misuse their positions as market makers to yet again fuck over retail investors.~~

3/29 Edit: The last sentence in this post is unsubstantiated, upon digging i've been unable to find evidence that would suggest this. However saying this HFT manipulation [is very much a real thing](https://www.sec.gov/news/press-release/2014-229) (Lots more evidence out there), which is why alot of the concepts in this post are still valid.

~~Best part about this is, when we see SLPs volume come through in TD TOS, we can likely with a~~ ~~reasonable degree of accuracy predict price movements.~~

3/29 Edit: This was stupid and dangerous of me to write (especially the prediction component). I believe my feelings got caught up in the process of writing this DD given it took a long time to research and write.

And last last note i promise, this is why using TA analysis ON ITS OWN is dangerous as it doesn't know what's actually going on.

3/29 Edit: I was chatting with a researcher from the GME discord server who it extremely knowledgeable and insightful. TLDR of the conversation is that i had a bad gut feeling about SLP and it aligned with her gut feeling. Therefore without evidence of SLP being used for nefarious purposes, i've adjusted my post to reflect this.

TLDR;

3/29 Edit: The following points are theories, theories are okay. It helps spur healthy conversation and allows others to raise conjecture which is what we need in this sub.

The shorts are in a death spiral of borrowing to cover FTDs and using HFT trading tactics to cover the remaining FTDs that the borrowed shares could not.

Whales are on our side, but are putting their effort into controlling buy/sell pressure on certain days to inflict max pain on the shorts options spread.

The price action we are seeing is largely made up of HFTs, Retail, the odd day trader or two (don't fucking do it).

This ain't financial advice yo, just an ape analysing data and reading boring as fuck SEC filings.

Edit: Readability changes

Edit: Thanks the the suport everyone. I've just woken up - so i'll go through your comments today and respond. Keep in mind there are nearly a thousand, if you have a valid point or really want to ask, PM me!

Edit: Checkout my [collaborators comment](https://www.reddit.com/r/GME/comments/mf1f6n/i_was_missing_a_key_piece_of_the_puzzel_this_is/gsl7jsq?utm_source=share&utm_medium=web2x&context=3) in regards to ALO in particular, thanks [u/SmithEchoes](https://www.reddit.com/u/SmithEchoes/)

Edit: Added acronym legend, sorry for those newer apes for using a bunch of them without saying what they were.
