Delta Neutral Update: Coming up for Air!
========================================

| Author       | Source       | 
| :-------------: |:-------------:|
|  [u/yelyah2](https://www.reddit.com/user/yelyah2/) | [Reddit](https://www.reddit.com/r/Superstonk/comments/oo5c7t/delta_neutral_update_coming_up_for_air/) | 

---

[Possible DD 👨‍🔬](https://www.reddit.com/r/Superstonk/search?q=flair_name%3A%22Possible%20DD%20%F0%9F%91%A8%E2%80%8D%F0%9F%94%AC%22&restrict_sr=1)

All - it looks like this could've been a quick trip underneath the Delta Neutral.

TLDR: Brace yourself for the possibility of hitting the $184 DN mark a couple times before it rebounds back over the DN.

*Delta/Gamma Neutral Graphs*

Here's an update to my graph showing the Close Price (green), delta neutral (blue), gamma neutral (orange) and gamma maximum (red). Log-based 10 scale below so you can see the gamma spikes in all their glory!

[![r/Superstonk - Delta Neutral Update: Coming up for Air!](https://preview.redd.it/0wrvx6fa3ec71.png?width=910&format=png&auto=webp&s=a46bb78da6a63bb09c17d5c0959697386858693e)](https://preview.redd.it/0wrvx6fa3ec71.png?width=910&format=png&auto=webp&s=a46bb78da6a63bb09c17d5c0959697386858693e)

GME 1/4/2021 - 7/19/2021

Log based 10 scale to give you a high-level overview

[![r/Superstonk - Delta Neutral Update: Coming up for Air!](https://preview.redd.it/nyhliedc3ec71.png?width=910&format=png&auto=webp&s=635ff082bad8e984c2e0ff66efb13e612a24ef53)](https://preview.redd.it/nyhliedc3ec71.png?width=910&format=png&auto=webp&s=635ff082bad8e984c2e0ff66efb13e612a24ef53)

GME 1/4/2021 - 7/19/2021 - Log Based 10

Quick Background

My work is built on the idea that the market is largely unpredictable, but one particular kind of behavior is certain - hedgies gonna hedge. It's written into their algorithms. Specifically, they like to delta hedge and gamma hedge. This work tries to profit on this one particular type of buying/selling behavior. If you're lost, please refer to the detailed data dictionary, methodology and assumptions section at the bottom.

Quick Notes

Key Points:

-   The Delta Neutral (DN) is currently at $184.

-   Last February, GME was deep under the DN for a couple weeks, which built up a lot of pressure and contributed to its rebound upwards.

-   This trip under the DN only lasted a couple days, so the rebound may not be as violent.

-   I also want to warn you that it may tap against $184 a couple times before rebounding. A few examples below.

As you can see for Roku below, the underlying close (green) had definitive rebounds back above the DN (dark blue) in March/April, but in May, you can see that it tapped against its DN three times before pushing over.

[![r/Superstonk - Delta Neutral Update: Coming up for Air!](https://preview.redd.it/q13ak3jz4ec71.png?width=910&format=png&auto=webp&s=f59022d187c8e1cab9892e6ef7a89c8d5b9f22f7)](https://preview.redd.it/q13ak3jz4ec71.png?width=910&format=png&auto=webp&s=f59022d187c8e1cab9892e6ef7a89c8d5b9f22f7)

ROKU 1/4/2021 - 6/17/2021

Hard to say what the secret ingredient is for what exactly contributes to the definitive push over the DN versus a couple tests first, but it's likely just some good ol' fashion momentum.

Here's hoping we decisively push through today!

Here are a couple options tid-bits for you before I sign off:

-   The 7/16 expirations did help with the call %, which currently sits at 26%, compared to 25% on 2/16 and 22% last Monday.

-   The key part here is the comparison to last Monday, because historically call buyers have been predominately buying cheaper calls for the next expiration date, hoping to get lucky and catch the next MOASS, so historically, there is a big drop in call % between Mondays/Friday, then slowly builds-up during the week.

-   We haven't had a Monday call % this high since 1/25!! That Monday had a 37% call OI, so were not quite at the same level now.

-   Yesterday, 69% of all volume was for this next expiration date, and 64% of that volume were for calls, so hoping we push the call OI up!

-   GME IV/prices are still relatively cheap, so hoping that will lead to more call buyers

-   The overall put IV is still higher than the call IV, indicating higher put buying pressure

-   Similarly, the OTM put IV (-0.25 delta) is still higher than the ATM call IV (0.5 delta), which indicates higher OTM buying pressure, so we're not out of the woods yet.

-   I've seen a lot of talk about gamma squeezes, and I don't think we're anywhere close to one. Last January, the ATM gamma was between 0.07 - 0.18 prior to the squeeze. Last Friday, we were at 0.0004, and there was an uptick up to 0.02 yesterday. We'll see if the upward trend continues.

TLDR: Brace yourself for the possibility of hitting the $184 DN mark a couple times before it rebounds back over the DN.

Overview

In general, all stock indicators boil down to two things - reversion to the mean and momentum. Every trader wants to accurately predict these two forces better than other guy, and if you use different indicators than the other guy, that an give you an 'alpha' in trading if it's a better predictor.

I make a lot of different indicators, but the two primary ones are the Delta Neutral and Gamma Neutral:

-   Delta Neutral (DN) - This helps identify reversion to the mean, and represents the underlying price that would create a total market delta of 0 across all GME options (all expiration dates) for a given date. In general, it acts like a floor to the underlying price, but if the price drops below the delta neutral, then it tends to shoot back up above that line.

    -   This is generally how I trade my model. I watch for stocks that drop below the DN, and buy them, expecting for traders to identify that the stock is underpriced and will revert back to a higher level.

-   Gamma Neutral (GN) and Gamma Maximum (GM) - This helps identify momentum. The GN represents the underlying price that would create a total market gamma of 0 across all GME options (all expiration dates) for a given date, whereas the GM represents the underlying price that would create the maximum gamma across the market.

    -   In general, a sudden increase in gamma indicates a sharp upward in momentum that continues until that gamma drops.

    -   The GM seems to act like a ceiling, but fun things happen when the underlying crossing that threshold!

This is my own personal 'alpha' that I developed for my own trading purposes, and am sharing with this community because it's given me back so much. This is not financial advice. I'm just a mathematician that likes to play with options data, and I am not a professional trader.

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

*Disclaimer: I'm just a mathematician that likes to play with options data and builds models to trade for a hobby. I have no experience trading professionally or offering any advice to anyone. This is just one indicator for one type of price movement, and there are many other indicators that can help you make investment decisions.*
