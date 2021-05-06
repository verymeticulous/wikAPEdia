The naked shorting scam in numbers: AI detection of 140M hidden FTDs, up to 400M naked shorts in married puts and massive dark pool activity by Shitadel and the shorts
=======================================================================================================================================================================

| Author       | Source       | 
| :-------------: |:-------------:|
|  [u/broccaaa](https://www.reddit.com/user/broccaaa/) | [Reddit](https://www.reddit.com/r/Superstonk/comments/mvdgf5/the_naked_shorting_scam_in_numbers_ai_detection/) | 

---

[DD 👨‍🔬](https://www.reddit.com/r/Superstonk/search?q=flair_name%3A%22DD%20%F0%9F%91%A8%E2%80%8D%F0%9F%94%AC%22&restrict_sr=1)

Edit: I made [a new post describing how I trained the binary classifier (AI) used in this post](https://www.reddit.com/r/Superstonk/comments/mwrycd/how_to_train_a_binary_classifier_ai_to_detect/).

This could be it. This could be the whole scam.

TLDR: HODL. Simple as that. HODL and the shorts have no way to escape. They just writhe around in desperation as FTDs escalate, their options expire and New DTCC rulings approach. To support this belief I:

-   Built an AI to detect Deep ITM calls used to create naked shares. *140M naked shares* produced this way since Jan. Deep ITM call covering appears to be their *last resort of illegal desperation*. It's so easy to spot.

-   Investigated married put naked shorting. At the Jan mini-squeeze put open interest went wild and aligns with *the creation of millions of naked shares with married put trades*. Put volumes appear to be sustained at higher levels to keep rolling over FTDs. *Up to 400M naked shares created in total*.

-   Looked through all 13F filings for funds with large GME positions (long/short). We have a clear idea of who is on which side of this battle and what a true idiot short position looks like (hint: Melvin).

-   Gathered all Dark Pool trading data from FINRA and show massive changes in trade behaviour since Jan. Huge increases in shares traded, but each trade is of few shares. And the key players? Known short funds. Supportive evidence for *naked short trades and suppression of retail buy pressure*.

I encourage you to read the post and take a look at the data so you can understand it for yourself. Correct me if I'm wrong somewhere. My suggestions? HODL with patience. Take a break from ticker watching. Take a walk outside. The shorts cannot escape 🚀🚀🚀🚀🚀

*Note: this is not financial advice. I am not a cat. I read gathered some data, made some figures and tried to understand them. Any number of my interpretations could be flawed and wrong. Do your own research, make your own mind up.*

Introduction

In this post I build an AI to detect suspicious Deep ITM Calls volumes used to hide FTDs. Take a look at historical options data to show recent fuckery in the options consistent with naked shorting tricks. And then compare these trends with Dark Pool trading volumes by known short funds.

The post will be broken down into the following sections:

1.  An AI to [detect Deep ITM calls](https://preview.redd.it/4g8izd9godu61.png?width=4500&format=png&auto=webp&s=be0dc2f3937cb050458b23c7f46b79ffd10f0f3a) used to hide FTDs

2.  A recap of the major short funds and their recent positions

3.  A recap of naked short selling and the married put

4.  Options fuckery consistent with naked shorting and the married put

5.  Dark Pool matters

6.  Conclusions

The motivation for the work was to try and test a number of predictions I made in my [first post on the naked shorting scam and the married put trade](https://www.reddit.com/r/GME/comments/mgj0j1/the_naked_shorting_scam_revealed_lending_of/).

These are the main ideas I wanted to test or at least find additional data to support or disprove them:

-   short interest is manipulated through naked shorting

-   the vast majority of options (both puts and calls) might be due to naked short selling

-   short shares are 'washed' and able to be dumped on the market even during SSR

-   the large number of way out of the money calls seen recently are actually part of a naked short trick

-   increased trades in OTC / Dark Pools are due to naked shorting and price manipulation

I've gathered a lot of data to better understand these questions. I believe that some of the data is now conclusive. Other areas more supportive. But the big message is that shorts have no way out and never had a chance to cover 🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀

An AI to detect Deep ITM calls used to hide FTDs

When a share is sold without being owned or borrowed (located) it is sold naked, a "naked short". This can happen as part of normal market activity by market makers and I've described [this process and how it can be abused in a previous post](https://www.reddit.com/r/GME/comments/mh6lnz/the_naked_shorting_scam_update_selling_nude_like/). When this occurs the SEC has clear guidelines on how long the seller has to find a share and deliver it to the buyer. If a share is not located in time it must be reported as a Fail to Deliver (FTD). Funds that have FTDs outstanding are required to resolve the position within a given timeframe and are restricted from selling short until then. I won't go into all the details on this but point you towards [the God Tier DD](https://iamnotafinancialadvisor.com/GME/) that covers this.

One way that a naked short seller can 'resolve' their FTDs without actually covering is through options fuckery. Deep in-the-money (ITM) calls can be bought and exercised immediately to acquire the shares and close the FTDs. [The SEC published a paper on this ILLEAGAL practice](https://www.sec.gov/about/offices/ocie/options-trading-risk-alert.pdf).

[Other great DD has been posted showing when Deep ITM volumes have been used to cover FTDs](https://www.reddit.com/r/GME/comments/mhv22h/the_si_is_fake_i_found_44000000_million_shorts/).

I wanted to train a machine learning algorithm (often called an AI) that could automatically identify this illegal fuckery and point us towards what exactly has been going on with GME this last year and particularly since Jan 2021. I won't go into the full details here. I've made [a separate post describing all the details of the classifier](https://www.reddit.com/r/Superstonk/comments/mwrycd/how_to_train_a_binary_classifier_ai_to_detect/).

-   End of day options data for all strike prices between Jan 1st 2020 and April 6th 2021 was collected

-   I manually labelled more than 10,000 rows of data from mid-Jan to mid-Feb for suspicious volumes likely due to FTD hiding

-   Labelled data was used to train different classifiers (AIs) reserving 30% of the data for testing

-   The best classifier (BalancedBagging-Adaboost) has an accuracy score of 91%

-   I used the model to identify all Deep ITM call options fuckery in the last year

THE AI FOUND EVIDENCE FOR MORE THEN 140 MILLION FTDs BEING HIDDEN SINCE JANUARY!!!

[![r/Superstonk - The naked shorting scam in numbers: AI detection of 140M hidden FTDs, up to 400M naked shorts in married puts and massive dark pool activity by Shitadel and the shorts](https://preview.redd.it/4g8izd9godu61.png?width=4500&format=png&auto=webp&s=be0dc2f3937cb050458b23c7f46b79ffd10f0f3a)](https://preview.redd.it/4g8izd9godu61.png?width=4500&format=png&auto=webp&s=be0dc2f3937cb050458b23c7f46b79ffd10f0f3a)

AI detection of option volumes used to hide FTDs and FTD values since January.

The above figure shows all the suspicious Deep ITM call volumes since January as coloured bars. The colour scheme shows the different strike prices that were used for the trade. FTDs as % of float are drawn on top in the blue line.

As FTDs were spiking and the situation became more and more unsustainable for the shorts towards the end of Jan ILLEAGAL Deep ITM options purchasing was used to naked short and cover FTDs. Smaller increases in Deep ITM volumes also occurred just before FTD spikes at the end of Feb and mid-Feb.

On Jan 27th 25 MILLION shares were magically acquired using this trick. 140 MILLION in total since Jan 1st.

[![r/Superstonk - The naked shorting scam in numbers: AI detection of 140M hidden FTDs, up to 400M naked shorts in married puts and massive dark pool activity by Shitadel and the shorts](https://preview.redd.it/30b6h4qopdu61.png?width=1800&format=png&auto=webp&s=ccafaf7bca99b134b09931bd5a60f11428c190ec)](https://preview.redd.it/30b6h4qopdu61.png?width=1800&format=png&auto=webp&s=ccafaf7bca99b134b09931bd5a60f11428c190ec)

Running total of suspicious call volumes since Jan 1st. 140 million as of April 6th.

[![r/Superstonk - The naked shorting scam in numbers: AI detection of 140M hidden FTDs, up to 400M naked shorts in married puts and massive dark pool activity by Shitadel and the shorts](https://preview.redd.it/m0pd5pwwpdu61.png?width=4500&format=png&auto=webp&s=1cefe0ef8b62b0ca853322c3e4c8b57205e5b641)](https://preview.redd.it/m0pd5pwwpdu61.png?width=4500&format=png&auto=webp&s=1cefe0ef8b62b0ca853322c3e4c8b57205e5b641)

AI detection of option volumes used to hide FTDs and GME price since January.

Here we see that suspicious Deep ITM call volumes often precede big price increases. This suggests that this illegal trick is used as a last resort. It's so easy to see even by eye when looking at the options chains. When shorts get desperate they go to the deep calls.

[![r/Superstonk - The naked shorting scam in numbers: AI detection of 140M hidden FTDs, up to 400M naked shorts in married puts and massive dark pool activity by Shitadel and the shorts](https://preview.redd.it/3tk1ye2jqdu61.png?width=4500&format=png&auto=webp&s=d77b931096e9f42d111565bf550c5639070b6bca)](https://preview.redd.it/3tk1ye2jqdu61.png?width=4500&format=png&auto=webp&s=d77b931096e9f42d111565bf550c5639070b6bca)

AI detection of option volumes used to hide FTDs and Short Interest (SI%) since January.

We see that Short Interest (SI%) decreased massively after all of the suspicious call option activity in late Jan. As well as getting the FTDs under control the suspicious Deep ITM call volumes might have been used to close legitimately borrowed shares to hide the true SI%.

With all the hype and attention the shorts knew they were completely fucked if they couldn't get everyone to believe it was over. But as we've seen after the lows of Feb this ride is far from over.

[![r/Superstonk - The naked shorting scam in numbers: AI detection of 140M hidden FTDs, up to 400M naked shorts in married puts and massive dark pool activity by Shitadel and the shorts](https://preview.redd.it/8mfwrbx6tdu61.png?width=4500&format=png&auto=webp&s=ebd2e26293f59af8d438169bead8b5f46a426d51)](https://preview.redd.it/8mfwrbx6tdu61.png?width=4500&format=png&auto=webp&s=ebd2e26293f59af8d438169bead8b5f46a426d51)

AI detection of option volumes used to hide FTDs and Short Interest (SI%) since April 2020.

Finally, if we look back over the past year very few suspicious Deep ITM call volumes were occurring. This changed in January 2021 as the FTDs started to get out of control and a huge amount of hype followed the price rises. This again makes me believe that the suspicious Deep ITM call volumes are a sign of desperation from the shorts.

Speculation alert: Deep ITM calls are bought in times of desperation by the shorts when FTDs, price and/or SI% are getting out of control. At the end of Jan more than 100 million naked short shares were created this way to hide FTDs, hammer down price and hide SI%. Through Feb and up until April another 40 million naked short shares were created this way when the shorts began to lose control of their hidden positions.

A recap of the major short funds and their recent positions

[![r/Superstonk - The naked shorting scam in numbers: AI detection of 140M hidden FTDs, up to 400M naked shorts in married puts and massive dark pool activity by Shitadel and the shorts](https://preview.redd.it/l0cx2nq85eu61.jpg?width=850&format=pjpg&auto=webp&s=18900ca805bc55c1372d3d2a39d098c4c6d4a803)](https://preview.redd.it/l0cx2nq85eu61.jpg?width=850&format=pjpg&auto=webp&s=18900ca805bc55c1372d3d2a39d098c4c6d4a803)

> Regulation SHO stocks with large, unsettled trades often exhibit a similar characteristic: *"short selling" hedge funds with significant put holdings in 13F filings*.
>
> MARRIED PUTS, REVERSE CONVERSIONS AND ABUSE OF THE OPTIONS MARKET MAKER EXCEPTION ON THE CHICAGO STOCK EXCHANGE
>
> John W Welborn, EconomistThe Haverford Group October 9, 2007

In my earlier post [The naked shorting scam revealed](https://www.reddit.com/r/GME/comments/mgj0j1/the_naked_shorting_scam_revealed_lending_of/) one thing that struck me was coming across the above quote. So I've gone though all the latest 13F filings that contain GME on [whalewisdom.com](https://whalewisdom.com/) to get a clearer picture of the enemy. Note: the last 13F filings were made on December 31st 2020.

First a reminder of the known biggest GME shorting losers:

-   [Melvin Capital suffered a 49% loss in the 1st-quarter](https://markets.businessinsider.com/news/stocks/melvin-capital-gamestop-losses-49-first-quarter-decline-reddit-trading-2021-4-1030292729)

-   [Hedge Fund Maplelane lost 45% on Gamestop](https://www.bloomberg.com/news/articles/2021-04-09/hedge-fund-maplelane-is-clawing-way-back-from-gamestop-losses)

So what does a massive short GME position look like in 13F filings?

[![r/Superstonk - The naked shorting scam in numbers: AI detection of 140M hidden FTDs, up to 400M naked shorts in married puts and massive dark pool activity by Shitadel and the shorts](https://preview.redd.it/cv9fzhxq6eu61.png?width=1810&format=png&auto=webp&s=833bc3e0760af8047ed58f5375aaaadac19951a0)](https://preview.redd.it/cv9fzhxq6eu61.png?width=1810&format=png&auto=webp&s=833bc3e0760af8047ed58f5375aaaadac19951a0)

GME positions from 13F filings for the biggest known losers in GME shorting

That's a lot of puts without any GME shares or calls! *Melvin had 6 million shares in puts* and *Maplelane close to 2 million*. Depending on where you look on whalewisdom Maplelane either has no calls or about 500k shares in calls but never any real shares. For now let's assume Maplelane is all in on puts.

[![r/Superstonk - The naked shorting scam in numbers: AI detection of 140M hidden FTDs, up to 400M naked shorts in married puts and massive dark pool activity by Shitadel and the shorts](https://preview.redd.it/rkj5le8t7eu61.png?width=1856&format=png&auto=webp&s=9b4fc0fcdc4c95204e5394846bef3eeedfa71b81)](https://preview.redd.it/rkj5le8t7eu61.png?width=1856&format=png&auto=webp&s=9b4fc0fcdc4c95204e5394846bef3eeedfa71b81)

Melvin hasn't held any GME shares since 2015.

[![r/Superstonk - The naked shorting scam in numbers: AI detection of 140M hidden FTDs, up to 400M naked shorts in married puts and massive dark pool activity by Shitadel and the shorts](https://preview.redd.it/q71rz0hx7eu61.png?width=1845&format=png&auto=webp&s=75007fcc44dc48023aab5c5b4cd86c0301dda672)](https://preview.redd.it/q71rz0hx7eu61.png?width=1845&format=png&auto=webp&s=75007fcc44dc48023aab5c5b4cd86c0301dda672)

Maplelane hasn't held any GME shares since 2014.

So big short losers have:

-   No shares in GME

-   Large put positions in 13F filings (either exclusively puts or the majority of their position)

What do other funds report for their GME positions?

[![r/Superstonk - The naked shorting scam in numbers: AI detection of 140M hidden FTDs, up to 400M naked shorts in married puts and massive dark pool activity by Shitadel and the shorts](https://preview.redd.it/506p312y8eu61.png?width=5350&format=png&auto=webp&s=98c7bad44cb276a92b8d9c87d7765e0327b72806)](https://preview.redd.it/506p312y8eu61.png?width=5350&format=png&auto=webp&s=98c7bad44cb276a92b8d9c87d7765e0327b72806)

All funds with at least 300k in either shares, calls or puts. Short positions are on the left and long positions on the right chart.

Here we see many of the known offenders. A bunch of short funds with majority puts and sometimes a smaller number of call options. Melvin takes the biggest idiot prize with 6 million shares in puts and nothing else. Here are the main offenders based on their end of 2020 filings:

-   Melvin capital management lp

-   Susquehanna international group llp

-   Ubs group ag

-   Group one trading l.p.

-   Citadel advisors llc

-   Hap trading llc

-   Citigroup inc

-   Wolverine trading llc

-   Maplelane capital llc

-   Jane street group llc

Some of these market participants operate market making and hedge fund activities. It is difficult to completely separate normal versus abusive practices. That being said these are the likely candidates and a good place for future DD digging.

*Wolverine trading llc* had an almost identical position to *Maplelane capital llc* who reported massive losses. *Ubs group ag* is an interesting one with almost 4 million shares in puts and nothing else. Is UBS a final boss?? *Hap trading llc* & *Citigroup inc* each had almost 2 million shares in puts and not much else. *Group one trading l.p.*, *Shitadel advisors llc*, *Susquehanna international group llp* & *Jane street group llc* feature prominently too.

Let me remind you of the earlier quote:

> Regulation SHO stocks with large, unsettled trades often exhibit a similar characteristic: "short selling" hedge funds with significant put holdings in 13F filings.

Many of these funds exhibit this characteristic and around the end of December and early Jan SI% and FTDs were through the roof. This looks like fuckery.

Next 13F filing updates should arrive by May 17th. This will be big.

Speculation alert: Any fund holding predominantly or exclusively a put position is short and likely engaged in illegal married-put naked shorting. The biggest know idiots Melvin and Maplelane have positions that look similar to other large funds (Wolverine, UBS etc.) suggesting we may have a clearer idea of who is up against us. And facing bankruptcy.

A recap of naked short selling and the married put

The reason that large put positions in 13F filings is suspicious is because those puts are likely to be the by-product of naked shorting. For a detailed description of how options trading can be used to sell naked shares you can [take a look at this post](https://www.reddit.com/r/GME/comments/mgj0j1/the_naked_shorting_scam_revealed_lending_of/) and [the follow-up post](https://www.reddit.com/r/GME/comments/mh6lnz/the_naked_shorting_scam_update_selling_nude_like/). Here is a brief description:

> Being a 'bone-fide' market maker grants you special privileges. One big privilege is to sell shares without needing to fulfil the 'locate' requirement. In other words, 'bone-fide' market makers are allowed to naked short sell, but they must find the shares after a certain amount of time.
>
> What is a 'bone-fide' market maker? No one really know. The SEC did a shitty job defining it so many brokers can likely pretend they deserve the title.
>
> How can the 'bone-fide' market maker privileges be abused? Well...
>
> If a hedge-fund wants to short sell but no shares are available to borrow, or they're too expensive, the hedge-fund can go to their 'bone-fide' market maker friend and follow this simple *'married put'* recipe:
>
> 1 Buy puts from the market maker covering the number of desired shares.
>
> 2 Buy shares from the market maker at the same time. The 'bone-fide' market maker can sell the shares naked as he remains net neutral on the trade.
>
> 3 Make the 'bone-fide' market maker happy by paying a tasty premium for the puts.
>
> 4 Dump the bought shares on the market to suppress prices and remain net short on the puts!
>
> For an extra spicy recipe that is harder to detect add the following step before step 4:
>
> 3b Sell way way out of the money call options equal to the bought shares that you never expect to be worth anything (800c calls anyone?) to the 'bone-fide' market maker for a small premium. The trade now looks like an innocent [reverse conversion](https://www.investopedia.com/terms/r/reverseconversion.asp).

Options fuckery consistent with naked shorting and the married put

So, if massive naked short selling via the married put trade has been used to cover up FTDs and SI% since Jan we should see some anomalies in the options chain. Let's take a look.

[![r/Superstonk - The naked shorting scam in numbers: AI detection of 140M hidden FTDs, up to 400M naked shorts in married puts and massive dark pool activity by Shitadel and the shorts](https://preview.redd.it/is3e6vn3heu61.png?width=4500&format=png&auto=webp&s=3ced765a93d48245b0a8b9a6d2394280b42289e5)](https://preview.redd.it/is3e6vn3heu61.png?width=4500&format=png&auto=webp&s=3ced765a93d48245b0a8b9a6d2394280b42289e5)

Total open interest for puts & calls as well as FTDs & SI% since Jan 2020.

HOLY FUCK THATS A MASSIVE JUMP IN OPEN PUT INTEREST!! And it's been sustained since the end of Jan. for the last year open interest in puts and calls remained very similar. At the end of Jan put open interest increased by more than 300% and completely disconnected from call interest. Immediately after this change FTDs and SI% dropped massively.

[![r/Superstonk - The naked shorting scam in numbers: AI detection of 140M hidden FTDs, up to 400M naked shorts in married puts and massive dark pool activity by Shitadel and the shorts](https://preview.redd.it/cdh81j9yheu61.png?width=3808&format=png&auto=webp&s=dc589f91495376dc303dbbff8cdec756fa62f712)](https://preview.redd.it/cdh81j9yheu61.png?width=3808&format=png&auto=webp&s=dc589f91495376dc303dbbff8cdec756fa62f712)

Cumulative open interest for puts & calls since Jan 2020.

If we look at the cumulative open interest over time we see the number of newly opened put contracts has remained steady throughout Feb and into early April. The rate at which these contracts are being bought is far greater than anything seen in 2020.

Speculation alert: The huge jump in open put interest could've provided up to 150 MILLION naked short shares to fight the January price spike and hide FTDs and SI%. When combined with certain brokers restricting retail buying, media FUD, January paper hands etc. their ploy appeared quite successful. Since pushing the price back to 40$ in Feb the constant and significant opening of new put contracts has been used to roll over the FTDs and do their best to keep their naked asses covered. Since Jan up to 400 MILLION naked short shares could've been used to hide FTDs and manipulate the price.

Dark Pool matters

Previously I speculated that Dark Pools could be used to facilitate the naked shorting trades. This hypothesis can be supported with data by looking at the [OTC data made available by FINRA](https://otctransparency.finra.org/otctransparency/OtcDownload).

Getting this data was a pain in the ass but I now have all Dark Pool volume data for GME since Nov 2020. This includes [Alternative Trading System (ATS)](https://www.investopedia.com/terms/a/alternative-trading-system.asp) and [Over-the-Counter (OTC)](https://www.investopedia.com/terms/o/otc.asp) volume data.

[![r/Superstonk - The naked shorting scam in numbers: AI detection of 140M hidden FTDs, up to 400M naked shorts in married puts and massive dark pool activity by Shitadel and the shorts](https://preview.redd.it/ulkgw6e0qhu61.png?width=3076&format=png&auto=webp&s=6447fbe7e5e730f9d90d0525d7db539fff3f4b97)](https://preview.redd.it/ulkgw6e0qhu61.png?width=3076&format=png&auto=webp&s=6447fbe7e5e730f9d90d0525d7db539fff3f4b97)

Dark Pool trade data for OTC and ATS trade pool.

Dark Pool activity ramped up massively at the start of Jan, particularly in the OTC pool. Towards the end of Jan as prices spiked during the mini-squeeze the total number of trades more than quadrupled and the average trade size dropped to around 50 shares per trade, remaining there ever since.

Re-routing of order flow anyone? Short ladder attacks in small share batches anyone?

If OTC trading was being used to suppress retail buy pressure we'd probably expect to find the worst of all the brokers **Robinhood** involved in the trading pool.

[![r/Superstonk - The naked shorting scam in numbers: AI detection of 140M hidden FTDs, up to 400M naked shorts in married puts and massive dark pool activity by Shitadel and the shorts](https://preview.redd.it/83iw1c15rhu61.png?width=3600&format=png&auto=webp&s=d7db9804c36d863a17be7d7bc8d0ce9f6a1c1586)](https://preview.redd.it/83iw1c15rhu61.png?width=3600&format=png&auto=webp&s=d7db9804c36d863a17be7d7bc8d0ce9f6a1c1586)

Total shares trades by firm for OTC and ATS pools since Jan. Note: using Log10 scale for comparison. Citadel actually traded 400M shares OTC!!!

Well what a surprise. Citadel trading 400M dark pool shares. Robinhood trading 2 million shares on OTC. The average trade size was ≈1 share which is fucking weird. Interactive Brokers only traded 9559 shares OTC but they made 9559 trades. Exactly 1 share per trade. Fucking weird.

Looking at the OTC market participant names, does anything look familiar? Oh yeah! Some of our market participants with massive puts in 13F filings also love to trade OTC!!

-   CITADEL SECURITIES LLC

-   JANE STREET CAPITAL, LLC

-   UBS SECURITIES LLC

-   WOLVERINE SECURITIES, LLC,

And the [worst offenders for Robinhood payment for order flow (PFOF)](https://www.washingtonpost.com/business/2021/01/29/robinhood-citadel-gamestop-reddit/):

-   CITADEL SECURITIES LLC

-   VIRTU AMERICAS LLC

-   G1 EXECUTION SERVICES, LLC

-   JANE STREET CAPITAL, LLC

-   TWO SIGMA SECURITIES, LLC

TWO SIGMA SECURITIES, LLC is an interesting one. As well as benefiting from PFOF they are also a known short. They don't show up in the 13F filings but they were [reported to take a big hit from short positions in Gamestop](https://www.ft.com/content/1ed2b0de-ea10-4a50-8f33-9f0a1cd38be9).

COMHAR CAPITAL MARKETS, LLC is a Chicago based firm just minutes away from Citadel. What are they doing trading 14 million GME shares OTC?!? I'm calling bullshit and suggesting this firm can be added to the short fund list.

COWEN AND COMPANY have 100k shares in puts from 13F but didn't show up in the earlier list as I set a minimum of 300k shares to be included. Another short hedge.

LEK SECURITIES CORPORATION don't have any obvious short positions in GME or news reports of losses. However they were [slapped by the SEC for large scale market manipulation in the recent past](https://finance.yahoo.com/news/sec-obtains-final-judgments-against-200100044.html).

Edit 1: G1 EXECUTION SERVICES, LLC is actually owned by [Susquehanna International Group](https://www.google.com/search?client=safari&rls=en&sxsrf=ALeKk02CdiMwg65ehzWH2qt2q3fRl_b4Jw:1619079033994&q=Susquehanna+International+Group&stick=H4sIAAAAAAAAAOPgE-LVT9c3NEwzMDQ3ys1KVuLSz9U3MCrMMUjL0TLIKLfST87PyUlNLsnMz9PPL0pPzMusSgRxiq0KEotS80oUkAUXscoHlxYXlqZmJOblJSp45pWkFuWBZRJzFNyL8ksLdrAyAgBfDMKMdAAAAA&sa=X&ved=2ahUKEwjYury1s5HwAhUF2aQKHZzNDa4QmxMoATAWegQIDxAD), one of the funds with tons of puts in 13Fs.

Edit 2: Some helpful comments point out that there can be some confusion with market makers and hedge-funds. Citadel is often referred to on this sub as the firm with the most to lose in GME. They operate market making and hedge fund activities. So do a number of other firms (Wolverine, Jane Street etc.). *For naked shorting the participation of 'bone-fide' market makers is crucial*. This is how they can abuse the locate rule and naked short. None of this contradicts the data in this post or the conclusions but it remains difficult to completely separate normal market making activities from abusive ones.

Speculation alert: OTC trades have seen massive volume and order size changes since early January. Many of the participants are known short funds. Changes in OTC trading align with evidence of manipulative naked short selling (Deep ITM calls and married-puts). OTC trading has been used to create millions of naked short shares and reroute retail orders to suppress buying pressure.

Conclusions

Hedgies are fucked. Just look at the amount of effort they've had to put into keeping a lid on this thing!!! *When they lose control of the FTDs they lose control of the price*. Millions of illegal naked short shares created in a desperate effort to make retail go away. But guess what??

[](https://preview.redd.it/zz5eu179biu61.gif?format=mp4&s=4b1aca79969f4d3653b39582fb94e9a3de4dfc8b)

Speculation alert: Here are my thoughts for what's happened with GME in 2021:

-   FTDs and SI% were getting out of control in early Jan

-   As prices increased and more hype came to GME the shorts got more and more desperate

-   Dark Pool OTC volumes went through the roof and Deep ITM call volumes were used to create naked shares ahead of the end of Jan price spike

-   When prices really started to move from Jan 25th - 29th more than 100 million shares were created with Deep ITM call and married-put naked shorting and used to hammer down price and hide SI%

-   A coordinated blocking of buy orders on key retail brokers and media induced FUD helped the shorts knock down the price and scare off some of the FOMO paper hand gang.

-   [Something happened to the short share borrow fees](https://www.reddit.com/r/Superstonk/comments/mma7eh/analysis_deep_dive_looking_at_historical_si_ftd/) that completely disconnect from normal pricing.

-   From Feb onwards average trade size on OTC decreased to around 50 shares per trade. That's a 70%+ drop in trade size. Retail orders were funnelled through Dark Pools to control buying pressure and 'short ladder attacks' used to control price.

-   ETFs were used to hide more and more FTDs from the apes. I have data on ETFs but its such a pain to analyse (70+ funds, all different GME allocations, rebalancing over time etc..).

-   DFV doubled down. RC tweeted an ice-cream cone. Deep ITM calls increased. FTDs remerged and on Feb 25th prices started flying again.

-   All this time FTDs and prices have been manipulated with tricky options trades. Up to 200 million naked short shares could've been made from Feb through to April 6th using married put trades.

-   But the apes are still here. Millions of short fund options have expired. FTDs are shown to get uncontrollable over time. An unprecedented FTD squeeze will come. New DTCC rules, a stronger SEC, GME annual meeting and share recall. So many catalysts. Shorts are fucked.

🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀
