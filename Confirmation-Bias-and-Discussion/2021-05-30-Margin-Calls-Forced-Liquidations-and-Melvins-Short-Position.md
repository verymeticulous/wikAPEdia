Margin calls, forced liquidations, and estimating Melvin's short position!
==========================================================================

| Author       | Source       | 
| :-------------: |:-------------:|
|  [u/yamayakuzaki](https://www.reddit.com/user/yamayakuzaki/) | [Reddit](https://www.reddit.com/r/DDintoGME/comments/nod4sg/margin_calls_forced_liquidations_and_estimating/) | 

---


[𝗗𝗶𝘀𝗰𝘂𝘀𝘀𝗶𝗼𝗻](https://www.reddit.com/r/DDintoGME/search?q=flair_name%3A%22%F0%9D%97%97%F0%9D%97%B6%F0%9D%98%80%F0%9D%97%B0%F0%9D%98%82%F0%9D%98%80%F0%9D%98%80%F0%9D%97%B6%F0%9D%97%BC%F0%9D%97%BB%22&restrict_sr=1)

EDIT 4- I apologize in advance if any apes have seen this on the other sub. I realized I cannot cross post, and was advised to create a new post, so here it is.

I'm seeing a lot of Apes assume that "When Marge comes calling, Team Shitadel will be forced to cover". This is not entirely accurate, and here's a post to help Apes understand how Margin calls work. Also, scroll down to Edit 2 and Edit 3 for my ballpark of how many shares Melvin shorted on Jan 25.

Margin calls are not necessarily always going to result in shorts covering

While margin calls CAN lead to shorts having to cover, this only happens in one of two scenarios:

1.  the short seller voluntarily chooses to close their position because they do not have the funds to increase their collateral requirements

2.  the short seller cannot fulfill its collateral requirements (defaults) and the lending broker takes the short seller's collateral and if required, any other assets owned by the short seller, liquidates it, and goes out to the market to buy back the share

If the short seller is able to post sufficient collateral when they get margin called, nothing happens. They do not cover.

How does a margin call actually work?

To short a stock, you need to borrow it. To borrow it, you need to post your initial collateral (which is typically 150% the value of the short sale at minimum...) and pay those insanely low borrowing fees. Let's ignore the borrowing fees and why they're so low and focus on the collateral aspect.

If and when the current stock price increases over the initial collateral amount each day, you face a margin call and are asked to close the position or increase your collateral (maintenance collateral) based on what the maintenance margin is (which ranges from 25% - 40% depending on the broker, but typically 30% on the NYSE) together with the total current value of the short sale value. I'm seeing margin requirements for RETAIL going up to 300%, but afaik, institutions are still at the 25% - 50% range.

Initial collateral posted for short sales is short sale value + margin requirement

So let's say, purely as an example (they very likely shorted WAAY more than this example), Shitadel initiated a short sale for 1,000,000 shares when it was at $40. The initial collateral required was short sale value + margin requirement, or $40 x 1m = $40m + 50% of $40m = $60m posted to the lending broker. This example also assumes they did NOT continue to add more shorts (which we know they did), or naked short (as naked shorts don't require collateral and are a whole different discussion).

As and when the stock price increases, Shitadel needs to deposit additional margin (the Margin call) if the total margin requirement is more than the existing collateral. If they can't do that, they can choose to voluntarily close their short position, or get force liquidated.

It's not WHEN Shitadel gets margin called. They already got margin called many times. It's when they can't meet the collateral.

This is not a one time thing - it happens EVERY TRADING DAY the price rises to the point where collateral needs to be increased. Shitadel has been margin called multiple times since the time the stock price was $40. They've just been able to either bring the stock price down so they don't need to post as much collateral, or they've liquidated assets to meet collateral. Let's look into this a little bit more.

After the initial collateral, maintenance collateral is calculated as short sale value (based on current price) + maintenance margin requirement

(let's use 30% as the maintenance margin for example).

When the price went up to $45, the total margin requirements for Shitadel were $45x1m = $45m + 30% of $45m = $58.5m, so they wouldn't have got margin called since the requirements are still less than the initial collateral of $60,000.

When the price went up to $50, the total margin requirements were $50x1m = $50m + 30% of $50m = $65m. They would have gotten margin called for the difference of $65m - $60m = $5m.

Fast forward to when the price went up to $277 ish ... the total margin requirements were $277x1m = $277m + 30% of $277m = $360.1m.

At this point, Shitadel would have had 5 days to meet that margin requirement (by liquidating other assets including crypto), or try to push down the stock price to a more manageable level.

Shitadel gets money back if the price goes lower than what the initial short sale value was

If the short sale value decreases (which is what the short seller was banking on) relative to what the share value was when the short sale was initiated, margin requirements also decrease, and they get money back.

So taking the initial example where Shitadel shorted 1,000,000 shares when it was at $40, if they were successful in dropping the price to $20, the margin requirement would have been $20 x 1m = $20m + 50% of $20m = $30m and they would have gotten $60m - $30m = $30m back. (whenever price falls, short sellers are required to have an additional 50% additional margin instead of the maintenance margin of 25-40% when price increases).

What does this all mean?

Well, it means that the margin call resulting in Shorts having to cover will only happen when the price of GME increases to the point Team shitadel would not be able to post the additional required collateral. This is not one magical price, but one that could be triggered in a domino effect, like countless DDs have speculated, where the smallest SHF gets forced to cover, share price increases, forcing the next SHF down the line to cover etc....all the way to the point where ALL SHORTs run out of funds to cover, upon which the responsibility goes to the lending broker, and then up the chain all the way to the DTCC and their insurance.

That's why we see them trying so hard to keep the price down so they can keep their collateral requirements "manageable", and days where the entire market (and crypto) are red because they need the liquidity to satisfy maintenance margin.

Short positions opened recently

The above examples all use shorts opened $40 and below. As we all know and speculate, team shitadel's also opened short positions ABOVE $40, but the concept still applies. They'd still have to post the collateral and maintain the margin requirements as and when the price fluctuates, and IF AND ONLY IF they can't meet that margin requirement, the collateral is used by the lending broker to go out to the market to buy a share back to close the position.

EDIT: The obligatory link that apes like. [See here](https://www.tdameritrade.com/retail-en_us/resources/pdf/AMTD086.pdf) - this document is from TD Ameritrade called the Margin Handbook and describes margin, margin requirements, and margin calls in detail.

EDIT2: [u/lvprentiss9](https://www.reddit.com/u/lvprentiss9/) asked a question in the comments about Melvin getting their $2b+ cash infusion. This gave me an interesting thought. We can estimate Melvin's short position as of that date. Not exact of course, just a ballpark to get a feel for what we're talking about here.

SPECULATION TIME

- After the trading day on Jan 25, Melvin reported receiving a cash infusion of $2.75 billion. The stock price closed at $76.79

- The previous closing price on Jan 22 (before the weekend) was $65.01. So between these two days , the collateral required for Melvin not to get margin called and default would have been whatever they already posted for collateral as of Jan 22 (when the price was $65.01) + $2.75 billion.

Jan 22 - the total collateral required would have been 1.3x 65.01x # shorted shares, or 84.513 x # of shorted shares

Jan 25 - the total collateral required would have been 1.3x76.79 x # shorted shares, or 99.827 x # of shorted shares

The above is assuming their lending brokers charged them 30% of the short sale value. could have been more, or could have been the FINRA minimum of 25%, but 30% is pretty standard. We don't care about when Melvin opened their position, or at how much...we just know that from Jan 22 - Jan 25, they had to increase their collateral or risk defaulting.

So Jan 25's 99.827 x # of shorted shares minus Jan 22's 84.513 x # of shorted shares = 15.314 x # of shorted shares. This is the delta that required that 2.75 billion cash infusion.

What do we get when we solve for # of shorted shares? 2.75 billion / 15.314 = 179,574,245.79 shares shorted.....Melvin alone shorted the entire float and the shares outstanding MANY MANY times over..... since then, since we know they didn't cover, there could only be MUCH HIGHER shares shorted....especially when you add in naked shorts and regular shorts from other short sellers! This is not even accounting for the January squeeze as it's before that, and they could have been required to post even more collateral, or it could have been the reason RH and others prevented buying...regardless, this is speculation across two data points..

Edit 3: BUT WAIT, that's just a little too optimistic. GME is likely not Melvin's only short position

Exactly - 179M shares shorted is very optimistic, but gives you an idea. For years, GameStop was the no-brainer go to for short sellers, so it would be reasonable to assume GME would constitute a large portion of a short seller's position. Let's look at more conservative numbers:

1.  If GME was only 25% of Melvin's total short position at risk of default, then it stands to reason that the 2.75 billion cash infusion was not JUST for GME....if 25% of the 2.75 billion was flagged for GME (and the rest for all of Melvin's other short positions at risk of margin default), then (2.75 billion / 15.314)x25% = 44.89m GME shares shorted. Which is more than the float. We also know Melvin was not the only short seller. So imagine this, multiplied across the many short sellers and add in naked shorts... it's no wonder they only reported the maximum allowable short interest back then (140%) and tried to hide those numbers since.

2.  If GME was 30% of Melvin's total short position at risk of default, that would be $53.87m shares shorted.

3.  If GME was 50% of Melvin's total short position at risk of default, that would be $89.79m shares shorted.

That's why I've come to the conclusion that even though my numbers are ballpark and that there is a possibility that not all 2.75 billion was put towards the collateral maintenance specifically for GME as of that date (they definitely would have needed it during the jan spike), it'd still be f'in high!!!

DISCLAIMER - I've made assumptions in these calculations, but I believe the theory behind it is sound/reasonable. Let me know what you think! Of course, this is an estimate and doesn't account for things like the 2-5 day margin call response period, or what happened after jan 25th, or whether Melvin needed the 2.75b to cover other short positions that are not gme or planned to keep part of the 2.75b to do other fuckery.

TLDR: Margin calls do not necessarily guarantee shorts having to cover. This only happens when they can no longer fulfill their maintenance margin requirements. I ballparked Melvin's short position on Jan 25th using these formulas. it's between 44.89m if you're conservative, up to 179.5 m if you want to be very optimistic!!!! Remember, this is only Melvin's short position....factor in ALL the other short HF's positions, and naked shorts...and this, fellow apes, is also one of the reasons why I am pretty zen like when i see the price fluctuate - it does not matter what the price is now...as one day, they will need to cover all these shorts and then fellow apes, we'll party.
