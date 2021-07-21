Delta/Gamma Neutral Update - Hold strong!
=========================================

| Author       | Source       | 
| :-------------: |:-------------:|
|  [u/yelyah2](https://www.reddit.com/user/yelyah2/) | [Reddit](https://www.reddit.com/r/Superstonk/comments/og9pcv/deltagamma_neutral_update_hold_strong/) | 

---

[DD 👨‍🔬](https://www.reddit.com/r/Superstonk/search?q=flair_name%3A%22DD%20%F0%9F%91%A8%E2%80%8D%F0%9F%94%AC%22&restrict_sr=1)

TLDR: This is just a quick update for the Delta Neutral/Gamma Neutral/Gamma Maximum indicators. The DN is currently ~$157, which isn't ideal for red days like we've been having, but GME always bounces back if it does drop. Hold strong!

*Background*

My work is built on the idea that the market is largely unpredictable, but one particular kind of behavior is certain - hedgies gonna hedge. It's written into their algorithms. Specifically, they like to delta hedge and gamma hedge. This work tries to profit on this one particular type of buying/selling behavior.

[![r/Superstonk - Delta/Gamma Neutral Update - Hold strong!](https://preview.redd.it/sk94lr67d0a71.png?width=300&format=png&auto=webp&s=2d69b060bbd94a962f23985309109832a9031764)](https://preview.redd.it/sk94lr67d0a71.png?width=300&format=png&auto=webp&s=2d69b060bbd94a962f23985309109832a9031764)

Hedgies Hedgin'

In general, all stock indicators boil down to two things - reversion to the mean and momentum. Every trader wants to accurately predict these two forces better than other guy, and if you use different indicators than the other guy, that an give you an 'alpha' in trading if it's a better predictor.

I make a lot of different indicators, but the two primary ones are the Delta Neutral and Gamma Neutral:

-   Delta Neutral (DN) - This helps identify reversion to the mean, and represents the underlying price that would create a total market delta of 0 across all GME options (all expiration dates) for a given date. In general, it acts like a floor to the underlying price, but if the price drops below the delta neutral, then it tends to shoot back up above that line.

    -   This is generally how I trade my model. I watch for stocks that drop below the DN, and buy them, expecting for traders to identify that the stock is underpriced and will revert back to a higher level.

-   Gamma Neutral (GN) and Gamma Maximum (GM) - This helps identify momentum. The GN represents the underlying price that would create a total market gamma of 0 across all GME options (all expiration dates) for a given date, whereas the GM represents the underlying price that would create the maximum gamma across the market.

    -   In general, a sudden increase in gamma indicates a sharp upward in momentum that continues until that gamma drops.

    -   The GM seems to act like a ceiling, but fun things happen when the underlying crossing that threshold!

This is my own personal 'alpha' that I developed for my own trading purposes, and am sharing with this community because it's given me back so much. This is not financial advice. I'm just a mathematician that likes to play with options data, and I am not a professional trader.

There is a detailed data dictionary, methodology and assumptions section at the bottom that gives my method in full detail.

*Delta/Gamma Neutral Graph*

Here's the graph you're used to seeing, and it includes the Close Price (green), delta neutral (blue), gamma neutral (orange) and gamma maximum (red), on a log-based 10 scale so you can see those spikes in all their glory.

[![r/Superstonk - Delta/Gamma Neutral Update - Hold strong!](https://preview.redd.it/c01cdyzfb0a71.png?width=910&format=png&auto=webp&s=80f628b1d49d920ef5ceaf49911ea5678c267e52)](https://preview.redd.it/c01cdyzfb0a71.png?width=910&format=png&auto=webp&s=80f628b1d49d920ef5ceaf49911ea5678c267e52)

A few things that happened since I last posted:

-   I've been working hard on updates to my model and creating new indicators that I hope to share soon. I know I keep saying that, but research takes time. There are a lot of twists/turns/unexpected results. May post what I have so far soon, and see if the group has any ideas to explain what I'm seeing.

-   I refined my IV methodology, which caused the DN optimization to break during the January squeeze (not surprising), but that's why you see it crash out in January. I'm working on identifying why that's happening.

-   The delta neutral floor is currently holding steady around $157, which obviously isn't ideal during these red days, but just know that GME always bounces back if it does drop.

-   GME likes to hang out between 10% and 30% higher than the delta neutral price if nothing unusual happens, which gives a range of $172 - $204 for the underlying.

-   GME's high is 214% higher than the DN back on 1/27, so certainly able to break higher, but it will see resistance to break higher.

-   No significant action with the GN since 6/8

-   The GM is currently at $247, indicating fun things COULD happen if we can bounce over that point.

*Methodology and Assumptions*

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

Gamma Neutral

The Gamma Neutral price that creates a total market gamma of 0 across all GME options (all expiration dates) for a given date. See the "Methodology and Assumptions" section for full detail on how I develop this indicator.

General notes below for observations on how this indicator behaves:

-   It acts like support/resistance between the delta neutral and the underlying, and typically bounces around between the two prices for most symbols (like we have seen with GME since April).

-   It also goes crazy in periods of high volatility, as you can see by the very higher spikes.

-   A gamma spike indicates the presence of POTENTAILLY slippery option market conditions, which COULD lead to a gamma squeeze. There were certainly spikes present back in January, but we had a few one-day false starts this last month.

-   They are often triggered by high price movement in a day, which can lead to continue high growth if underlying volume supports it.

-   Gamma spikes can also be triggered by unusual options purchases during the day. These are the one ones to find, because you can often catch the high increase waves before they actually start.

-   If I'm trading this indicator, I often either wait for a gamma spike to continue for 2 days in a row and supported by increased volume. Otherwise, I invest straight away if I find a gamma spike just based on options movement (i.e. no significant underlying increase yet).

I write my own algorithms to produce the results above. The following lists some key methodology and assumptions I use:

-   I rely on daily options and stock summaries produced by [www.historicaloptionsdata.com](http://www.historicaloptionsdata.com/)

-   For the Implied Volatility (IV), I use the following method:

    -   Calculate the raw IV of the mid-point between bid/ask price at close.

    -   Calculate a "blend" IV, which represents the IV where the call/put parity holds, i.e. where call delta -- put delta = 1, using the same IV.

    -   Smooth the mid-point call/put and blend IV using a gaussian smoothing algorithm with a 20-strike window.

    -   Apply the smoothed call/put relativities to the smoothed blended IV curve

    -   Fill any missing values with a linear interpolation of the neighboring strikes.

-   Using the final call/put IV estimates described above, I calculate my own Greeks. I like this source if you're interested in the formulas: <https://www.macroption.com/option-greeks-excel>

-   For the total market delta and total market gamma, I rely on the OI x delta and OI x gamma for each strike price.

    -   Note that the delta of a call is usually equal to (1 - put delta), so not adjustment is needed to the delta signs when calculating the total market delta.

    -   However, the call/put gammas are both positive based on the B-S calculation. If you're calculating the total gamma for a portfolio, or the total market, you have to add the call gamma and subtract the put gamma.

-   To estimate the delta neutral and the gamma neutral, I have an algorithm that relies on the optimization toolbox in Matlab to identify an underlying price that achieve a total market delta and a total market gamma.

-   Note that the IV would change with higher/lower prices for the delta/gamma neutral and the sensitivity tests, but the impact is not significant enough to make a meaningful difference and takes significant processing time to apply the IV curves. However, it is an important simplifying assumption to be aware of.

-   Open Interest (OI) is always lagged one day for options summaries. The OCC releases final open interest on a given day, and it represents the OI for the close of the prior day. Therefore, the OI I get in my summaries on 6/28 does not represent the OI as of close on 6/28. It represents the OI as of close on 6/25. If you see a source like Yahoo give live OI throughout the day, they are only estimates, and their algorithm methodology for estimating the OI based on various price/volume movement is a closely guarded secret. Using the prior day OI is currently a limitation of the data available to me.

*Disclaimer: I'm just a mathematician that likes to play with options data and builds models to trade for a hobby. I have no experience trading professionally or offering any advice to anyone. Nothing is certain in trading. It's all probabilities and what increases/decreases your chance at a profit. This is just one indicator for one type of price movement, and there are many other indicators that can help you make investment decisions.*

*I'll do my best to respond to all comments, including the negative ones. I'm happy to have a productive chat about any of my logic. I've gotten a lot of good ideas from posting on this forum, so thank you! However, if I can defend myself in a dark parking lot with nothing but my high heels, I can certainly defend myself against online trolls. So be nice.*

TLDR: This is just a quick update for the Delta Neutral/Gamma Neutral/Gamma Maximum indicators. The DN is currently ~$157, which isn't ideal for red days like we've been having, but GME always bounces back if it does drop. Hold strong!
