Delta Neutral Update - $176 Floor Today
=======================================

| Author       | Source       | 
| :-------------: |:-------------:|
|  [u/yelyah2](https://www.reddit.com/user/yelyah2/) | [Reddit](https://www.reddit.com/r/Superstonk/comments/nwrzba/delta_neutral_update_176_floor_today/) | 

---

[Education 👨‍🏫 | Data 🔢](https://www.reddit.com/r/Superstonk/search?q=flair_name%3A%22Education%20%F0%9F%91%A8%E2%80%8D%F0%9F%8F%AB%20%7C%20Data%20%F0%9F%94%A2%22&restrict_sr=1)

TLDR: If you believe in my delta neutral theory, the current floor for this crash is $176.

There are a lot of very valid theories out there on the floor to this crash, and here's mine that has worked pretty well in the past.

Recap

My work is built on the idea that the market is largely unpredictable, but one particular kind of behavior is certain - hedgies like to hedge. It's written into their algorithms. Specifically, they like to delta hedge and gamma hedge. This work tries to profit on this one particular type of buying/selling behavior. I have a little data dictionary at the bottom if you need a refresher on terminology.

This post is mostly an update to the delta neutral (underlying price where the total market delta is zero). My general theory is that as the underlying approaches the delta neutral a few things happen:

-   There is a large influx of call option purchases, because:

    -   The call prices get less expensive as the underlying price approaches the delta neutral

    -   Stock prices usually rebound/revert back to the mean after large crashes, so the price often rebounds anyways.

-   With the large influx of call volume, market makers have to start buying stocks to delta hedge, which turns the price back around and creates an upward trajectory.

-   Historically, you can see that GME often bounces off the delta neutral prices during drops. The exception is the February drop. When the underlying goes below the delta neutral price, a lot of pressure builds up that results in a significant increase when that pressure is released.

    -   Note that this is how I trade my model. I look for equities that fall below the delta neutral.

    -   If you're interested in prior posts that helped reassure during the dips, here you go:

        -   [5/10 Post](https://www.reddit.com/r/Superstonk/comments/n9cutk/gme_bouncing_off_delta_neutral_price_today/)

        -   [5/11 Post](https://www.reddit.com/r/Superstonk/comments/na952e/gme_delta_neutral_price_update/)

Graph Update

Here's the graph you're used to seeing, and it includes the Close Price (green), delta neutral (blue), gamma neutral (orange), and max pain (light blue)

[![r/Superstonk - Delta Neutral Update - $176 Floor Today](https://preview.redd.it/6kfa4wojtg471.png?width=910&format=png&auto=webp&s=c43b15b11696f544540f536b68020061204961ff)](https://preview.redd.it/6kfa4wojtg471.png?width=910&format=png&auto=webp&s=c43b15b11696f544540f536b68020061204961ff)

GME 1/4/2021 - 6/10/2021

The delta neutral through 6/9 was $173, and I am projecting a delta neutral today of $176.

Don't panic. Just buy the dip.

*Data Dictionary*

-   Delta Neutral: price that creates a total market delta of 0 across all GME options (all expiration dates) for a given date. General observation is it acts like a theoretical floor (although the price can go lower, as seen in February). My theory is that as the underlying approaches the delta neutral, call options go on sale. As people buy call options, MM have to buy the stocks which increases the price. Most stocks like to hang out above the delta neutral, some dip below and create pressure that can shoot them back over the delta neutral (like what happened in February), and some like to hang out below (like the VIX).

-   Gamma Neutral: price that creates a total market gamma of 0 across all GME options (all expiration dates) for a given date. General observation is it acts like support/resistance between the delta neutral and the underlying, and typically bounces around between the two prices for most plan (like we have seen with GME since April). It also goes crazy in periods of high volatility (as you can see by the infinite spikes).

-   Max Pain: price that creates largest loss for option buyers and largest gain for option sellers. This is a controversial topic because underlying prices can drift towards this point. There are typically large areas around the max pain that doesn't make a lot of difference to the profits for option buyer/sellers. It can be used to help gauge where the equilibrium of the options data is, but there is often a wide range around this price point that does not meaningfully affect MM profits.

Disclaimer: I'm just a person that likes to play with options data and builds models to trade for a hobby. I have no experience trading professionally or offering any advice to anyone. Nothing is certain in trading. It's all probabilities and what increases/decreases your chance at a profit. This is just one indicator for one type of price movement, and there are many other indicators that can help you make investment decisions.
