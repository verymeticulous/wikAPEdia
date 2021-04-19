WTF Does the most recent NYSE SEC filing mean? | NYSE is giving the HFTs a swift kick in the ass
================================================================================================

**Author: [u/jsmar18](https://www.reddit.com/user/jsmar18/)**

**Source: [Federal Regsiter Proposed Rule Change to Amend Rule 7.37](https://www.federalregister.gov/documents/2021/04/14/2021-07592/self-regulatory-organizations-nyse-chicago-inc-notice-of-filing-and-immediate-effectiveness-of)**

[DD 👨‍🔬](https://www.reddit.com/r/Superstonk/search?q=flair_name%3A%22DD%20%F0%9F%91%A8%E2%80%8D%F0%9F%94%AC%22&restrict_sr=1)

Well, won't we looky here. Looks like the NYSE may be trying to capitalise on the recent market scrutiny to take another potshot at every market manipulator's fav friend.

ALOs (Add Liquidity Orders) and ISOs (Intermarket Sweep Orders)!!!!

So if you don't know by now, I tend to write about order types and HFT. Of particular focus to me is the NYSE Chicago due to:

1.  Particularly low volume, which makes it easy to pick up changes in order type behaviour

2.  A probable stomping ground for our friends Shitadel

3.  NYSE trying to amend ALO and ISO orders, multiple times

For reference, the NYSE is made up of multiple exchanges, such as Arca, National, American and my personal fav Chicago.

Anywho, so what is up with the most recent [news](https://www.reddit.com/r/Superstonk/comments/mqisex/well_look_what_gets_published_tomorrow_this/?utm_medium=android_app&utm_source=share) posted by [u/Phonemonkey2500](https://www.reddit.com/u/Phonemonkey2500/)?

This [bad boy](https://www.federalregister.gov/documents/2021/04/14/2021-07592/self-regulatory-organizations-nyse-chicago-inc-notice-of-filing-and-immediate-effectiveness-of). A filing from the NYSE Chicago with the SEC proposing to amend some rules. It's a pretty fucking dry read. As such, I am at your service to translate it into monke speak, but first off, let's get some background from my [previous post](https://www.reddit.com/r/GME/comments/mf1f6n/i_was_missing_a_key_piece_of_the_puzzel_this_is/) that explains the two orders of interest.

🐍 IOC ISO (Immediate or Cancel Intermarket Sweep Order)

For those who have not read my previous post find an excerpt below.

[Intermarket sweep order](https://ibkr.info/article/1734)'s are generally a large quantity order that is sent to multiple exchanges.This is how it functions:

-   An order is submitted in the pre market to sell at a price of 40.80 and is sent to exchange A.

-   The best offer price on exchange A is 40.63.

-   Exchange B receives an intermarket sweep order to buy 800 shares of the stock at a limit price of 40.88.

-   The best offer price on exchange B is 40.88

The trader that enters the intermarket sweep order would be required to fulfill their Regulation NMS requirement by executing the maximum available quantity on exchange A at 40.63 and then may execute the balance of the order on exchange B at 40.88 even though it is at a price that is inferior to the 40.80 order resting in the book on exchange A. The 40.80 price is not the inside quote and is therefore not "protected" in terms of the balance of the sweep order executing at exchange B at a price of 40.88.

So in monke speak, it fills the lowest alternate exchange price before filling the order at the higher price.

To make it more complicated this is an order with a modifier (ISO is the modifier), so let's understand an IOC.

These are orders which attempt to execute immediately and cancel any unfilled portion. E.g. place a buy for 10 @ $180.01 , it's only able to be filled to a portion of 5 @ $180.01 and then canceled straight away.

A key part to these types of orders is derived from the following.

> *"The intermarket sweep exception enables trading centers that receive sweep orders to execute those orders immediately, without waiting for better priced quotations in other markets to be updated."*

This is [derived from a response](https://www.sec.gov/comments/sr-nyse-2014-32/nyse201432-2.pdf) to change how ALOs work by the NYSE, as they've been a thorn in their side since 2014. A prelude to what we'll go into later in the more recent attempt to fix shady shit that HFTs love abusing.

🐍 Add Liquidity Only (ALO)

First of all, major thanks to [u/SmithEchoes](https://www.reddit.com/u/SmithEchoes/) on this bad boy as it's a complicated beast.

Now this order type is a doozy, and is currently being used for nefarious purposes.

ALO follows a strict "If,then" rule set based on if it locks [(7.31(e)(2)(b)iii-iv)](https://nyseguide.srorules.com/rules/document?treeNodeId=csh-da-filter!WKUS-TAL-DOCS-PHC-%7B4A07B716-0F73-46CC-BAC2-43EB20902159%7D--WKUS_TAL_19401%23teid-37) OR crosses [(7.31(e)(2)(b)ii)](https://nyseguide.srorules.com/rules/document?treeNodeId=csh-da-filter!WKUS-TAL-DOCS-PHC-%7B4A07B716-0F73-46CC-BAC2-43EB20902159%7D--WKUS_TAL_19401%23teid-37). This rule set forces the ALO to perform these trades until it is fully consumed, or the order is canceled. Rule [7.31(e)(2)(C)](https://nyseguide.srorules.com/rules/document?treeNodeId=csh-da-filter!WKUS-TAL-DOCS-PHC-%7B4A07B716-0F73-46CC-BAC2-43EB20902159%7D--WKUS_TAL_19401%23teid-37), once ALO is resting on the exchange AND it was forced to change its price in accordance with [7.31(e)(2)(b)i-iv](https://nyseguide.srorules.com/rules/document?treeNodeId=csh-da-filter!WKUS-TAL-DOCS-PHC-%7B4A07B716-0F73-46CC-BAC2-43EB20902159%7D--WKUS_TAL_19401%23teid-37) THEN it now gets to be priced in accordance with [7.31(e)(1)(A)iii and iv](https://nyseguide.srorules.com/rules/document?treeNodeId=csh-da-filter!WKUS-TAL-DOCS-PHC-%7B4A07B716-0F73-46CC-BAC2-43EB20902159%7D--WKUS_TAL_19401%23teid-37). This is the equivalent of HFT when ALO "activates" BUT it comes with a built in safety feature that IF the price goes UP(Sell ALO) or DOWN (buy ALO) the ALO limit price is no longer locking or crossing at the values it was getting moved to, it REVERTS back to its original limit order price.

Monke speak translator: These orders create sell/buy walls that have a nifty function that essentially "flips the safety switch" back to the original limit order price if too much buy/sell pressure is applied.

🐒 Back to the SEC Filing

Rewind to 2014

Funnily enough, the NYSE has tried to [amend how ALO orders work](https://www.federalregister.gov/documents/2014/10/16/2014-24547/self-regulatory-organizations-new-york-stock-exchange-llc-nyse-mkt-inc-order-approving-proposed-rule), because of how they can be used for nefarious purposes.... *cough* Shitadel *cough* The amendment would force to cancel the ALO once it crosses or locked, and not perform how it currently does in accordance with [7.31(e)(2)(b)i-v](https://nyseguide.srorules.com/rules/document?treeNodeId=csh-da-filter!WKUS-TAL-DOCS-PHC-%7B4A07B716-0F73-46CC-BAC2-43EB20902159%7D--WKUS_TAL_19401%23teid-37). Which means no buy/sell wall capability for them to use and abuse.

Fast Forward to Today

Smart fucks at the NYSE have done them HFs a dirty.

There is no fundamental change to how specific order types work, but a rather elegant smack to the HFTs asses through changing how the PBBO is calculated (read this for wtf a [PBBO](https://www.investopedia.com/terms/o/order-protection-rule.asp) is *"Best Protected Bid and the Best Protected Offer"*).

Going back to our ISO order we discussed (and how it can be used in conjunction with an ALO) is where this starts to come together. I was going to force you to read a paragraph, but i decided to be nice and just translate it into monke speak.

Change how PBBO is calculated, fuck with how the ALO orders "safety switch" as described above. This makes it less enticing in my eyes at least for HFTs as it increases the risk associated with it (risk being eating away their profits due to no safety switch triggering from buy/sell pressure).

This is overly simplifying the implications, which to be honest are not that large as they are following suit of NASDAQ and some other exchanges here. It just has particular ramifications for HFTs two fav order types that make them "riskier" to use i.e. less appealing.

As for when this is going through? ~~I don't do legal things. From what~~ ~~I~~ ~~interpret it as, it's active when it is filed, which I believe is today. Thanks to how it does not "significantly change shit" (my words, not the NYSE's)~~

Thanks to [u/Suspicious-Oil-7096](https://www.reddit.com/u/Suspicious-Oil-7096/) for linking the below. The amendment is effective as of 26th April.

<https://www.nyse.com/regulation/rule-filings>

~~Wait for~~ [u/leaglese](https://www.reddit.com/u/leaglese/) ~~backup on this one though.~~

As always, feedback, opinions and questions are more than welcome, in fact wanted!

TL;DR

NYSE tried to fix order types abused by HFTs in 2014, failed. Tried again today, and on face value have succeeded in giving them a swift kick up the ass. It's now riskier to use ISO/ALO orders due to a "safety" switch of sorts being removed due to how the amendment proposes to calculate the PBBO of ISOs. This means it's less attractive for HFTs to abuse the order type.

Edit: Bad at words, fixed ape speak.

🚀 Edit: Speculation Room

Thought i'd add in a speculation room to put out my thoughts on how this affects GME price action.

Speculation #1

IF it comes into effect from today (again waiting on confirmation from legal wrinkle brain), it means they'll have a harder time controlling the price. No longer being able to reliably create buy/sell walls, which *could* pose a significant risk to them if they choose to artificially increase buy pressure. On the flip side, it could also hurt any friendly HFT whales who use these order types on the buy-side (think max pain theory). I personally believe most price action is being manipulated by the shorts, so it's more of a detriment to them than anything else.

It'll be interesting to observe price action moving forward, that's for sure.

Speculation #2

IF this does have an effect on how NYSE Chicago uses ALO/IOC ISO orders I'd have the expectation that either the rate of increase decreases dramatically in % share of these order types (shown below) ~~OR they decrease and switch entirely back to another order type due to the risk posed by the new filings changes.~~

[![r/Superstonk - WTF Does the most recent NYSE SEC filing mean? | NYSE is giving the HFTs a swift kick in the ass](https://preview.redd.it/id5d5vosb5t61.png?width=613&format=png&auto=webp&s=ff59bf80e04a38b39c79850fe56aeffab21d965d)](https://preview.redd.it/id5d5vosb5t61.png?width=613&format=png&auto=webp&s=ff59bf80e04a38b39c79850fe56aeffab21d965d)

https://www.nyse.com/markets/nyse/trading-info#equities-order-types

Speculation #3

The amendment becomes effective as of 26th April, expect to see the order types abused until this time. This means speculation #2 will likely see a slow down in the % increase, but it's hard to tell given it has already slowed down in the rate of increase over the past few months. We'll sadly need to wait until midish June-2021 to see the effect of this amendment on order type behaviour for NYSE Chicago.
