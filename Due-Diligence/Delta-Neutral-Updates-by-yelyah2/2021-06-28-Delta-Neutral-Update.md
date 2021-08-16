Delta Neutral Update: Any meaningful underlying price increase today will significantly increase our chances at a squeeze in the near future.
=============================================================================================================================================

| Author       | Source       | 
| :-------------: |:-------------:|
|  [u/yelyah2](https://www.reddit.com/user/yelyah2/) | [Reddit](https://www.reddit.com/r/Superstonk/comments/o9qb4n/delta_neutral_update_any_meaningful_underlying/) | 

---

[DD 👨‍🔬](https://www.reddit.com/r/Superstonk/search?q=flair_name%3A%22DD%20%F0%9F%91%A8%E2%80%8D%F0%9F%94%AC%22&restrict_sr=1)

TLDR: any meaningful increase today (>2%) will significantly increase the chances of a squeeze in our near future.

Edit1: We obviously finished at ~1.8% today instead of 2%. Green is green and any increase is good (like always). Think of it like we were playing in a special bonus round today that would've quadruple our daily GME points, and we probably didn't get those bonus point. Still a good day! I'm excited to process my options data dump when I get it in an hour or so, and will be sure to share the results.

Edit2: AH price movements still definitely help! My options data dumps are near end of day (~15 min before close), so I won't see the impact of AH movement when I process tonight, but it's all still good!

Edit3: Just to be clear, I was not predicting a >2% increase today. My sensitivity testing goes from 2% to 10%, so I was saying that my sensitivity tests show even a 2% increase will get some awesome bonus delta today (more than usual). Since we were at ~1.8% today, that doesn't mean we get nothing. I'm sure we will still get bonus delta, but my sensitivity tests just didn't go below 2%, so I couldn't tell you what was it was. We're good though! It was a good day!

I apologize for my absence. I've been on vacation for the first time since 2019! California was beautiful. Definitely making me think about a move :)

Since it's been a couple of weeks, I'll do a full refresher below.

*Background*

My work is built on the idea that the market is largely unpredictable, but one particular kind of behavior is certain - hedgies gonna hedge. It's written into their algorithms. Specifically, they like to delta hedge and gamma hedge. This work tries to profit on this one particular type of buying/selling behavior.

[![r/Superstonk - Delta Neutral Update: Any meaningful underlying price increase today will significantly increase our chances at a squeeze in the near future.](https://preview.redd.it/ck93r8xvg1871.png?width=168&format=png&auto=webp&s=ab98f88b94e4fa0198174029e71061abe2891686)](https://preview.redd.it/ck93r8xvg1871.png?width=168&format=png&auto=webp&s=ab98f88b94e4fa0198174029e71061abe2891686)

Hedgie doing its Hedgin'

There is a new methodology/assumptions section at the bottom that gives my method in full detail. This section gives a high-level of the key pieces of the analysis described in this post.

Delta

The Delta of an option represents the expected change to an option's price based on a $1 change in the security's underlying price. For example, if the GME underlying price is at $100,000,000 and a GME $102,000,000 strike call has a delta of 0.2, then that call option price will increase by $0.2 if the GME underlying price moves up to $100,000,001. Note that the price is also affected by gamma so will actually be higher than the $0.2 price increase estimated by delta, which will be covered later.

[![r/Superstonk - Delta Neutral Update: Any meaningful underlying price increase today will significantly increase our chances at a squeeze in the near future.](https://preview.redd.it/ugpgf1wjg1871.png?width=987&format=png&auto=webp&s=8ecf759c7f1119d70b9f5765674590f866168fb5)](https://preview.redd.it/ugpgf1wjg1871.png?width=987&format=png&auto=webp&s=8ecf759c7f1119d70b9f5765674590f866168fb5)

Call versus Put Delta by Strike Price for an Underlying @ $100

Delta hedging is a trading strategy employed by market makers (MM's) to minimalize the directional risk associated with price movements in the underlying security. Traditionally, you can think of a MM buying 20 (0.2 x 100) stocks of the underlying security if the price increases by $1 (using the example above). However, it's important to note that hedge funds often use other derivatives to hedge, not just buying/selling stocks because it requires less capital to do so. However, these indicators can be used as a directional proxy for some of the MM behavior as the underlying price increases/decreases.

The total market delta share equivalent represents the sum of delta x OI across all strikes/expiration prices in a given trading day. I will say it one more time, hedge funds are not actually holding this number of shares on a given day to hedge. They often hedge with other market derivatives. However, it can give us an indicator for hedge funds buying/selling underlying equity relativities.

Delta Neutral

The Delta Neutral price that creates a total market delta of 0 across all GME options (all expiration dates) for a given date. It can also be though of as the intersection of a supply/demand curve for hedged stocks. See the "Methodology and Assumptions" section for full detail on how I develop this indicator.

Notes below for general options on how the delta neutral interacts with the underlying price:

-   There is a large influx of call option purchases, because:

    -   The call prices get less expensive as the underlying price approaches the delta neutral

    -   Stock prices usually rebound/revert back to the mean after large crashes, so the price often rebounds anyways.

-   With the large influx of call volume, market makers have to start buying stocks to delta hedge, which turns the price back around and creates an upward trajectory.

    -   Important note that hedgies often hedge with derivatives instead of buying stocks, so there isn't a 1-to-1 relationship between the delta and shares bought/sold by hedge funds.

-   Historically, you can see that GME often bounces off the delta neutral prices during drops. The exception is the February drop. When the underlying goes below the delta neutral price, a lot of pressure builds up that results in a significant increase when that pressure is released.

    -   Note this is the primary way that I trade my model. I made a scanner that looks for equities that fall below the delta neutral.

Gamma

The Gamma of an option represents the rate of change of the Delta of an option with respect to a $1 underlying price movement. From our example above, if the GME underlying price is at $100,000,000 and a GME $102,000,000 strike call has a delta of 0.2 and a gamma of 0.05, then that call option price would actually increase by $0.25 (0.2 + 0.05) if the GME underlying price moves up to $100,000,001.

[![r/Superstonk - Delta Neutral Update: Any meaningful underlying price increase today will significantly increase our chances at a squeeze in the near future.](https://preview.redd.it/14jxduhrk1871.png?width=670&format=png&auto=webp&s=b3d64c2e70ae8961359d1b1c5f708ea70f1ed9c8)](https://preview.redd.it/14jxduhrk1871.png?width=670&format=png&auto=webp&s=b3d64c2e70ae8961359d1b1c5f708ea70f1ed9c8)

MM also hedge against gamma risk, but the impact of buying/selling securities to hedge is often much lower than the impact of delta hedging (also remember that they use derivatives to hedge too). However, you are probably familiar with gamma because of the "gamma squeeze" that happened back in January. A gamma squeeze happens when the underlying stock price begins to go up very quickly in a short period of time. This forces more buying activity from rapidly increasing deltas/hedging, which continues to inflate the price.

Gamma Neutral

The Gamma Neutral price that creates a total market gamma of 0 across all GME options (all expiration dates) for a given date. See the "Methodology and Assumptions" section for full detail on how I develop this indicator.

General notes below for observations on how this indicator behaves:

-   It acts like support/resistance between the delta neutral and the underlying, and typically bounces around between the two prices for most symbols (like we have seen with GME since April).

-   It also goes crazy in periods of high volatility, as you can see by the very higher spikes.

-   A gamma spike indicates the presence of POTENTAILLY slippery option market conditions, which COULD lead to a gamma squeeze. There were certainly spikes present back in January, but we had a few one-day false starts this last month.

-   They are often triggered by high price movement in a day, which can lead to continue high growth if underlying volume supports it.

-   Gamma spikes can also be triggered by unusual options purchases during the day. These are the one ones to find, because you can often catch the high increase waves before they actually start.

-   If I'm trading this indicator, I often either wait for a gamma spike to continue for 2 days in a row and supported by increased volume. Otherwise, I invest straight away if I find a gamma spike just based on options movement (i.e. no significant underlying increase yet).

*Delta/Gamma Neutral Graph*

Here's the graph you're used to seeing, and it includes the Close Price (green), delta neutral (blue), and gamma neutral (orange), on a log-based 10 scale so you can see those spikes in all their glory.

[![r/Superstonk - Delta Neutral Update: Any meaningful underlying price increase today will significantly increase our chances at a squeeze in the near future.](https://preview.redd.it/3w8in2bxn1871.png?width=910&format=png&auto=webp&s=8ee0e0f575df7fcc96a93eef105b6107024dc69a)](https://preview.redd.it/3w8in2bxn1871.png?width=910&format=png&auto=webp&s=8ee0e0f575df7fcc96a93eef105b6107024dc69a)

GME 1/4/2021 - 6/25/2021

A few things that happened the last two weeks:

-   The delta neutral floor continues to rise (yay!) It's currently at $176.

-   GME likes to hang out between 10% and 30% higher than the delta neutral price if nothing unusual happens, which gives a range of $194 - $230 for the underlying.

-   GME's high is 214% higher than the DN back on 1/27, so certainly able to break higher, but it is hard to break through that resistance.

-   No significant action with gamma since 6/8

*Total Market Delta*

The graph below summaries the total market delta share equivalents (dark blue) versus the underlying close price (green). See the "Delta" section above for information on what the total market delta share equivalent amounts represent.

[![r/Superstonk - Delta Neutral Update: Any meaningful underlying price increase today will significantly increase our chances at a squeeze in the near future.](https://preview.redd.it/valw8po1s1871.png?width=909&format=png&auto=webp&s=5241a6231a0d442eb3cfa268e37ea5957827fbf5)](https://preview.redd.it/valw8po1s1871.png?width=909&format=png&auto=webp&s=5241a6231a0d442eb3cfa268e37ea5957827fbf5)

GME Total Market Delta Share Equivalent versus Underlying Close

You will notice above that the total market delta increased significantly BEFORE the January and February/March squeezes. This helped to contribute to the buying pressure to push GME upwards.

The graph below provides a sensitivity test for the total market delta share equivalent (blue) based on +5% (light red) and -5% (dark red) shifts to the underlying price.

[![r/Superstonk - Delta Neutral Update: Any meaningful underlying price increase today will significantly increase our chances at a squeeze in the near future.](https://preview.redd.it/g01npebyr1871.png?width=909&format=png&auto=webp&s=3720955ff7a40a4e03937176115c34e9f736301c)](https://preview.redd.it/g01npebyr1871.png?width=909&format=png&auto=webp&s=3720955ff7a40a4e03937176115c34e9f736301c)

+/- 5% Underlying Price Sensitivity Test

Now you can see that the impact to the total market delta increases significantly BEFORE large changes to the total market delta share equivalent, which happens BEFORE large changes to the underlying price.

Note that there are also potential for large DECREASES if there is also a potential for large INCREASES. The total market delta sensitivity tests have also been indicating a potential for a large decrease as the market has been dropping the last few weeks.

For example, back in January:

-   The sensitivity test on 1/8/2021 showed a 5% increase to the underlying on 1/8/2021 ( a Friday) would've increased the total market delta by 91%.

-   On 1/11/2021 (Monday), the price increased by 13%, and the total market delta increased by 305%.

-   The underlying price then increased by 200% between 1/11/2021 to 1/14/2021.

Now! My sensitivity tests as of 6/25/2021 close showed that a 5% increase today would lead to a 60% increase in the total market delta equivalent! As of writing this, we have already been up > 5% at a high for the day, and currently at a 3% gain. I expect this will lead to a significant increase in the total market delta shares, which will put us well on our way towards another squeezy squeezy lemon peezy.

[![r/Superstonk - Delta Neutral Update: Any meaningful underlying price increase today will significantly increase our chances at a squeeze in the near future.](https://preview.redd.it/leipjjemu1871.png?width=1280&format=png&auto=webp&s=eceb696974c5897f08ffe7b3c51e9d5d936931c3)](https://preview.redd.it/leipjjemu1871.png?width=1280&format=png&auto=webp&s=eceb696974c5897f08ffe7b3c51e9d5d936931c3)

*Methodology and Assumptions*

I write my own algorithms to produce the results above. The following lists some key methodology and assumptions I use:

-   I rely on daily options summaries produced by <https://www.orats.com/>

-   Their options summaries use "near end of day" snapshots (i.e. 15 minutes before close), because they say its more reliable for producing Greeks. They say the last 15 minutes is not a reliable source for options prices to represent the rest of the market day. Therefore, you may notice

-   I still rely on [www.historicaloptiondata.com](https://www.historicaloptiondata.com/) for my stock information, but working on converting to orats.

    -   Note that the Underlying Price in the graphs above is the Close price, not the near end of day price.

-   For the Implied Volatility (IV), I use the following method:

    -   Orats produces a smoothed IV that I like, which I use in conjunction with the mid-price call/put IV's to produce a final IV.

        -   The orats smoothed IV cleans the quotes, and solves for a residual yield based on the put-call parity formula. This lines up the call and put implied volatilities, to account for estimating hard-to-borrow stocks, or stocks with differing dividend assumptions.

        -   Next, the IV curve is smoothed through the strike IV's using cubic splines. This is helpful for producing reasonable IV's in low volume stocks or strike prices.

    -   The smoothed IV methodology above produces the same set of IV for both calls and puts. Theoretically, the IV should be the same for both calls/put, because it should represent the estimated volatility of the underlying price for both calls and puts, which wouldn't differ.

    -   However practically, the IV never actually just represents the estimated volatility of the underlying. The IV used in the Black-Scholes (B-S) price calculation is usually always higher than the historical volatility, because options sellers attach an IV premium to the raw IV that helps make them money.

    -   Because calls can produce infinite losses to options sellers, the IV premium tends to be higher for calls than for puts. I use the following methodology to adjust the orats call/put smoothed IV:

        -   I pull the orats options database for each ticker, trade date and expiration date.

        -   Calculate the relativities of the raw mid-price call / smoothed IV, and the raw mid-price put / smoothed IV for each strike price.

        -   Fill in any missing relativities with the nearest relativity, within its own ticker/trade date/expiration date. This mostly just applies to far OTM strikes.

        -   Smooth the relativities using rloess, which is a local regression using weighted linear least squares and a 2nd degree polynomial model. This method assigns zero weight to data outside six mean absolute deviations.

        -   Apply the smoothed call/put mid-price relativities to the smoothed orats IV estimates to get the final call/put IV estimates.

-   Using the final call/put IV estimates described above, I calculate my own Greeks. I like this source if you're interested in the formulas: [https://www.macroption.com/option-greeks-excel](https://www.macroption.com/option-greeks-excel/#gamma-in-excel)

-   For the total market delta and total market gamma, I rely on the OI x delta and OI x gamma for each strike price.

    -   Note that the delta of a call is usually equal to (1 - put delta), so not adjustment is needed to the delta signs when calculating the total market delta.

    -   However, the call/put gammas are both positive based on the B-S calculation. If you're calculating the total gamma for a portfolio, or the total market, you have to add the call gamma and subtract the put gamma.

-   To estimate the delta neutral and the gamma neutral, I have an algorithm that relies on the optimization toolbox in Matlab to identify an underlying price that achieve a total market delta and a total market gamma.

-   For the sensitivity tests, I adjust the underlying price in the snapshot by +/-5%, and run the algorithms as described above, to estimate what the total market delta/gamma would be at the different underlying price.

-   Note that the IV would change with higher/lower prices for the delta/gamma neutral and the sensitivity tests, but the impact is not significant enough to make a meaningful difference and takes significant processing time to apply the IV curves. However, it is an important simplifying assumption to be aware of.

-   Open Interest (OI) is always lagged one day for options summaries. The OCC releases final open interest on a given day, and it represents the OI for the close of the prior day. Therefore, the OI I get in my summaries on 6/28 does not represent the OI as of close on 6/28. It represents the OI as of close on 6/25. If you see a source like Yahoo give live OI throughout the day, they are only estimates, and their algorithm methodology for estimating the OI based on various price/volume movement is a closely guarded secret.

    -   Note that I'm currently working on my own algorithm to estimate same-day OI, but I'm not done yet.

    -   However, it should be noted that using the prior day OI is a limitation of the data available to me.

*Disclaimer: I'm just a person that likes to play with options data and builds models to trade for a hobby. I have no experience trading professionally or offering any advice to anyone. Nothing is certain in trading. It's all probabilities and what increases/decreases your chance at a profit. This is just one indicator for one type of price movement, and there are many other indicators that can help you make investment decisions.*

*I'll do my best to respond to all comments, including the negative ones. I'm happy to have a productive chat about any of my logic. I've gotten a lot of good ideas from posting on this forum, so thank you! However, if I can defend myself in a dark parking lot with nothing but my high heels, I can certainly defend myself against online trolls. So be nice.*
