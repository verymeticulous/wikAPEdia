Greetings, Apes. Let's clarify some things about average trade sizes, transactions reporting, and the FINRA ADF.
================================================================================================================

| Author       | Source       | 
| :-------------: |:-------------:|
|  [u/MarketMicrostructure](https://www.reddit.com/user/MarketMicrostructure/) | [Reddit](https://www.reddit.com/r/Superstonk/comments/na5drq/greetings_apes_lets_clarify_some_things_about/) | 

---


[Education 👨‍🏫 | Data 🔢](https://www.reddit.com/r/Superstonk/search?q=flair_name%3A%22Education%20%F0%9F%91%A8%E2%80%8D%F0%9F%8F%AB%20%7C%20Data%20%F0%9F%94%A2%22&restrict_sr=1)

Hello Apes,

I'm Zak, a colleague of [/u/dlauer](https://www.reddit.com/u/dlauer/) who I've been working with for the past 5 years on all sorts of projects. He told me how fascinating and engaging of a community you all have built, and after spending a couple of days looking around, I completely agree. It's really great how much the general attitude is concerned with really trying to figure out what's true, and that there's a lot of openness and eagerness to learn (especially when a whole lot of people would probably find most of these topics incredibly boring). While I mostly stay buried in development and analytics tasks, I hope to spend a little more time here following along with what you're all up to.

I appreciate the moderating crew for letting me post some stuff while I work on obtaining that sweet karma.

Problems & Background

Some ongoing themes around here involve questions about if/when/where trades are reported, theories about what small average trade sizes mean, and what dark pools, internalizers, and the FINRA ADF are. These things are all closely intertwined. And since there's a lot of effort going into trying to draw conclusions from the data, I think a lot of those efforts would be improved with a few contexts and ideas.

Before any of that, I have to admit that I share Dave's skepticism of the usefulness of the modern US market structure. While some vested interests point to certain price-improvement metrics regarding PFOF and internalization as 'proof' that it is beneficial to market welfare, I'm not sure this tells the whole story. Just because the second-order effects on market stability and quality are hard to measure doesn't mean they don't matter. It's possible a narrow class of people benefits at the expense of many more. I'm not ready to draw a conclusion one way or the other, but I am more than a bit annoyed at how easily this gets brushed aside.

Last disclaimer: everything here is to the best of my knowledge from a few years spent developing analytics for institutional clients to measure their execution quality and assess trading performance resulting from routing orders to different brokers who would then execute the orders in a mix of on- and off-exchange transactions. Before that, most of my career was spent in futures, which tend to be much nicer for simple people like myself.

Are all trades reported to the tape?

Generally, yes (unless someone is breaking the rules). By any reasonable interpretation of the rules, all FINRA members have an obligation to report transactions. Depending on the parties involved in the transaction and where it's taking place, there are also rules outlining who has the responsibility.

For a very thorough treatment of how different types of transactions generate reporting requirements see [FINRA 6308B](https://www.finra.org/rules-guidance/rulebooks/finra-rules/6380b). There's a lot of concrete examples.

There were some questions about whether Citadel could have a brokerage account at Robinhood and then trade with Robinhood customers without generating a report. I discuss the different scenarios that this could fall into and show that they all generate reporting obligations in this post: <https://www.reddit.com/r/Superstonk/comments/n9331h/dave_lauer_clears_things_up_about_the_dark_pool/gxp36ur/?utm_source=share&utm_medium=web2x&context=3>

At the end of the post above, I qualified it with:

> None of this is to say that rule violations can't happen or don't happen. They do happen. Bank of America was caught [falsifying its trade reports](https://www.reuters.com/article/us-bankofamerica-new-york-settlement/bank-of-america-pays-42-million-fine-in-new-york-masking-probe-idUSKBN1GZ27H) by altering who it said the customers were executing against. Last month, it was reported that Robinhood was [failing to report](https://www.reuters.com/article/us-robinhood-regulation-tradereporting-e/exclusive-robinhood-failed-to-disclose-certain-trade-executions-to-public-feed-idUSKBN2BV0FZ) transactions for its fractional shares.

Unfortunately, sometimes when we choose our words carefully or point out past abuses in specific cases, people's imaginations can run away with it and start seeing abuse everywhere.

I think we clearly need much stronger oversight systems to catch abuses much sooner. But it's important to know that when most of these abuses have been caught, it wasn't from analyzing public data. It's incredibly hard to draw any reasonable conclusions from public data. (However, Dave and I have been working on some projects to do this effectively. Hopefully, we'll be able to share soon.)

The FINRA ADF is not the boogeyman

Some people this morning were concerned about the GME volume labeled as FINRA ADF. But this is actually a "catch-all" designation for off-exchange transactions:

> FINRA ADF is not a dark pool. In fact, no trading occurs on it at all. The volume you're seeing is mostly retail volume from traders like yourselves.
>
> In general, when any FINRA member conducts a transaction, either for themselves or on behalf of a customer, they are required to report the transaction to the tape. Transactions that don't occur on any of the lit exchanges still need a way to enter into the SIP feed so that all market participants can be aware that a transaction has taken place. The FINRA ADF is the exchange code for those transactions.
>
> When a discount broker like Robinhood routes an order to Citadel and Citadel fills the order, that is considered an OTC transaction and is reportable. Citadel reports this transaction to a Trade Reporting Facility and it becomes a part of the time and sales record for that day.

During the trading day, all non-exchange transactions for reg nms stocks are reported in this way. This includes dark pools and internalizers of retail order flow.

Below is a sample of some GME trades from NYSE TAQ data, which is historical data from the SIP feeds. From [the spec,](https://www.nyse.com/publicdocs/nyse/data/Daily_TAQ_Client_Spec_v3.0a.pdf) you can see Exchange Code "D" corresponds to the FINRA ADF. When the Exchange Code is "D" the TRF column is populated with one of the three specific [TRF facilities](https://www.finra.org/filing-reporting/trade-reporting-facility-trf).

[![r/Superstonk - Greetings, Apes. Let's clarify some things about average trade sizes, transactions reporting, and the FINRA ADF.](https://preview.redd.it/s5o4zdhdbjy61.png?width=799&format=png&auto=webp&s=138cca33b04e50133c239f9ba6634a2a7a627bc2)](https://preview.redd.it/s5o4zdhdbjy61.png?width=799&format=png&auto=webp&s=138cca33b04e50133c239f9ba6634a2a7a627bc2)

Snapshot of SIP data with FINRA ADF exchange and a TRF code

In general, the workflow goes like this: one or more FINRA members conduct a transaction; based on the details of the transaction, the member responsible for reporting sends it to the TRF facility with whom they have a relationship; the TRF facility reports it to the SIPs.

A month later you are able to see more specific venue breakdowns for where the volume actually occurred. The [FINRA OTC Transparency](https://otctransparency.finra.org/otctransparency) website lets you get all that data by week. "ATS Issue Data" is for registered dark pools; "OTC (Non-ATS) Issue Data" is for internalizers.

Small average trade sizes don't necessarily imply manipulative behavior

One of the recurring themes I come across in my work with these sorts of complex systems with a lot of feedback and adaptation is how a tremendous amount of entirely different scenarios can generate the same macro-observable outcomes. This is persistently true with market data. When coming up with an explanation for observed data, it's first important to be aware of many possible ways that data could have been generated. Having good background information will help you estimate what explanations are likely. But to be truly rigorous to where you can be confident with a conclusion, you need to know how to rule out alternative explanations.

From the previous two sections, we've already seen that retail order flow that is routed to an internalizer will show up as FINRA ADF. Since retail order flow tends to have very small sizes, it is no surprise that the average trade size for FINRA ADF will be small.

But I've seen some other threads that also try to dig into the dark pool-specific, "ATS Issue Data", from the OTC Transparency website. These threads also reveal the average dark pool trade size can often be 100-200 shares, and many people seem very angry about this.

Having had the opportunity to analyze the way that the trade desks of large $10B+ funds execute their orders, I will propose a pretty simple explanation for why this happens:

-   It's common to hear institutional trade desks talk about how large their position is in terms of a stock's average daily volume (ADV), because this metric gives a decent heuristic of how much they can execute at a time without having an impact on the market price --- or alternatively, how much they will have to move the market in order to close their position in a short period of time.

-   As a result, when an institutional trade desk needs to get into or out of a desired position, it will typically break up the total desired quantity into many smaller trades and execute over several days (or longer) so as to not move the market all at once.

-   The trade desk will then route the smaller pieces to different brokers with whom they have relationships. This is called sending a "parent order" to a broker. The brokers offer a variety of "execution algorithms" that have different behaviors which the trade desk can select from in order to achieve their target size with the desired market impact and time constraints.

-   When a broker algorithm receives a parent order, it breaks that up into "child orders" to route to different trading venues using a combination of active and passive orders. These venues are often a mix of lit exchanges and dark pools.

-   The overall goal for institutions trading large size is to not "show your hand" and not let any one venue or broker have all the information about the position you're trying to get into or out of. Because if someone knows you're trying to execute 2 days of ADV, they can rush into the position now and then wait while you have an impact on the market.

There are many other mechanisms for moving large size, but given the enormous variety of trading venues and the desire to minimize market impact, it is not surprising that the average trade size would be small.

In general, I think we need to know these sorts of tedious things so that we can make sure we're asking the right questions. If we accept that small average trade sizes aren't evidence of malicious behavior, then we can get to the important question: should we even have all of these dark venues leading to all of this complexity in the first place?
