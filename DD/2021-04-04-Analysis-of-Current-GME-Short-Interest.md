Full analysis of current GME SI, proof from the data it is much higher than stated, and how they are hiding it. DD
==================================================================================================================

| Author       | Source       | 
| :-------------: |:-------------:|
|  [u/boneywankenobi](https://www.reddit.com/user/boneywankenobi/) | [Reddit](https://www.reddit.com/r/GME/comments/mjzx9w/full_analysis_of_current_gme_si_proof_from_the/) | 

---

[DD 📊](https://www.reddit.com/r/GME/search?q=flair_name%3A%22DD%20%F0%9F%93%8A%22&restrict_sr=1)

It's been a few days since I've written a DD, but no worries, back with some more confirmation bias for you lot - this time with way too much research behind it to be healthy. Also, [/u/thr0wthis4ccount4way](https://www.reddit.com/u/thr0wthis4ccount4way/) called my last DD short and I intend to fix that here. But since this has turned into a PhD thesis with how long it has gotten a bit about me: I've been in the AI / data science world for more than 15 years and am now one of the top AI researchers / data scientists at a fortune 50 company. My last job involved doing actual professional DD research for the commodities market (though not pricing, not a financial advisor) before leading the entire department. In short - I like numbers, but then again I'm some random person on the internet, so why should you trust me? I could be a jedi cat for all you know!

Chapter 1: Known data - my data sources for transparency

Let's start with what is known and what isn't known. It's important to acknowledge the fact that the stock market is an information vacuum. Let's start with what can be known:

-Slightly delayed institutional holdings of > 5% - [the key here is that any change for an institution with this high an ownership stake has to be reported if their stake changes by more than 5%, and has to be reported within 10 days of the end of a month.](https://www.investopedia.com/terms/s/schedule13d.asp) So we know this number within a 95% confidence interval for the beginning of March now.

-Delayed institutional holdings - [This data is reported 45 days after the end of each quarter. So any data available outside of large holders and ETFs is likely from 12/31/2020. Studies have shown most will wait the majority of this time](https://pages.business.illinois.edu/finance/wp-content/uploads/sites/46/2016/12/Christoffersen-Paper-April-2017.pdf) so any data is unreliable until the 45 days is up. The next reporting date is May 15th, 2021 which will be current up until March 31st. Note - other data is also available from institutional holdings such as voting and non-voting shares.

-Current ETF holdings - [ETFs report their holdings at the end of each day](https://www.sec.gov/investor/alerts/etfs.pdf)

-Current Insider holdings - [Insiders must disclose any change in ownership within 2 days](https://www.investor.gov/introduction-investing/general-resources/news-alerts/alerts-bulletins/investor-bulletins-69)

-Current option volume - Reported throughout the day

-Delayed option open interest - Reported at the beginning of the next trading day

-Delayed *reported* short interest - Comes from FINRA, but my favorite place to find it is [marketbeat since they also disclose the float along with the percentage of float SI](https://www.marketbeat.com/stocks/NYSE/GME/short-interest/)

-Current short volume - [Reported at the end of each day at 6:00est](http://regsho.finra.org/regsho-Index.html)

-Delayed dark pool data - [This data is a month old and only gives data a month back](https://otctransparency.finra.org/otctransparency/AtsIssueData). Most current data is for the week of February 22nd. The data is transactions which happened outside of the standard markets and are usually direct transactions which don't go through clearing houses.

-Delayed Failure to Deliver data - [Data also comes from FINRA and is several weeks delayed](https://www.sec.gov/data/foiadocsfailsdatahtm)

This is the data available. There are other bits of information out there, but for the purposes of this DD, these are the most important parts of the data.

Chapter 1.5: Dead end data

There are lots of ways to get wrong or inaccurate data. A few of the ways I have seen, and why they can't be used:

-Short volume to calculate short interest - Short volume has no clear correlation with short interest change. Short sales only count the selling action - it is either long (owned) or short (borrowed). The buyer can be covering a short position or going long. If the former, then the net short interest change is 0 - so it is possible to have 100% short volume and no change in short interest. I have run the numbers, and there is no relationship for GME that I can find. This post is too long as it is, so may follow up with that analysis later.

-Current institutional holdings - Sorry, Bloomberg only uses the current filings, which as described above, are extremely delayed

-Retail holdings - This is also something that has no reliable data. Any estimation that has been done has been a complete guess aside from the work by [/u/the_captain_slog](https://www.reddit.com/u/the_captain_slog/) which I will reference later. Guessing based on how many redditors there are in GME or WSB has no way to calibrate it, and therefore estimates of 6-100M shares have all been given. It don't work.

Chapter 2: How shorts are actually hidden

There is a *metric fuckton of speculation* here, so it is time I clear things up. So let's start with a few facts: Any short which fails to deliver a real share within T+2 days, (or T+5 days for a long share) are considered a failure to deliver and are counted in the report I reference above. This means that if Hedge M short sells a share on Wednesday, they have to deliver it by Friday or be put on the list Monday.

Misconception #1: [There is a market maker exception](https://www.sec.gov/divisions/marketreg/mrfaqregsho1204.htm) - The market maker exception was eliminated in 2008, so now they have to follow the same T+2 rules as everyone else does.

Misconception #2: The T+13 number which is being thrown around is only for the punishment for failing to deliver, FTDs get reported after T+2. See above link.

Misconception #3: The T+4 and T+6 numbers are no longer current. [They were based on the T+3 rule for share delivery which ended in 2017, replaced by T+2](https://www.nasdaq.com/articles/t2-coming-2017-03-30). For clarity - those numbers were based on 1 day past the T+3 and T+5 for short and long sales, replaced as stated above by T+2 and T+4. This DD will focus on T+2 since it is for short sales.

Misconception #4: [The stock borrow program is no more](https://www.sec.gov/rules/sro/nscc/2014/34-71455.pdf) - though it hasn't been talked about on Reddit, other sites have cited this rule as a method for naked shorting.

There are three ways that I can tell which hide naked shorts: (1) Options, (2) Dark Pools (Alternative Trading System), (3) Reborrowing. All three of these revolve around one main principle: resetting the timer. A failure to deliver is really a last ditch effort because it reveals information about a true SI. Since we have seen such low FTD numbers, if there are naked shorts being hidden, they must be resetting the timer every 2 days. Something to remember: Since the market is an information vacuum, information is especially valuable.

Options

This one has been covered some, though with key inaccuracies so I won't link to the posts. [The SEC has done a report on this method](https://www.sec.gov/about/offices/ocie/options-trading-risk-alert.pdf) but let me distill it down. The key to hiding naked shorts is to reset the failure to deliver timer (T+2). So an institution has 2 business days to deliver a share, otherwise on the third day it gets added to the list. One thing they can do, and have been known to do, is do a 'buy-write' transaction where they write a deep ITM calls (say at a 15 strike price for GME) and buy shares at the same time. So they sell the calls which are about as expensive as the shares overall, and the buyer immediately exercises the contracts for the shares. However, the seller uses those bought shares to cover their short positions and has no intention of delivering the shares to the call buyer. Now they need to deliver those same shares to the buyer of the call, only this is a new transaction so the timer is reset!

This has been likely happening recently according to [the option chain for the 4/16 expiry](https://imgur.com/gallery/rvOc3gR). Look at all of those deep ITM option volume! But we likely won't see any change in the open interest, as these are immediately exercised by the buyer [since this is most commonly done with a FLEX option, which lets the buyer and seller set their own terms - like an immediate exercising](https://www.investopedia.com/terms/f/flexoption.asp).

Seem odd? Hell yeah it does, and when looking at the historical option data for 4/16, it seems to have happened in early [March as well](https://imgur.com/a/stoHAGo)! This date seems to be very commonly used, but other dates could have been used historically as well. Look for yourselves at [Optionistics](https://www.optionistics.com/quotes/option-prices). But this isn't just theory which was put forward by the SEC, [it has happened](https://www.lexisnexis.com/legalnewsroom/securities/b/securities/posts/sec-sanctions-university-professors-for-naked-short-scheme) in [multiple](https://www.sec.gov/alj/aljdec/2013/id490bpm.pdf) documented [cases](https://www.sec.gov/litigation/admin/2011/34-65941.pdf). Seriously, this happens - but fortunately it's illegal. Unfortunately, it takes forever to find it and prosecute.

What are the signs that this sort of activity is happening and not just retail activity? Let's look at the notes in the SEC report on how to detect it:

> Excessive trading or trading exclusively in hard to borrow or Threshold List securities. check
>
> Large short positions in hard to borrow or Threshold List securities check.
>
> Large failure to deliver positions in an account, often in multiple securities. check, at least for GME
>
> Continuous failure to deliver positions at CNS (Continuous Net Settlement System). check
>
> The use of buy-writes and/or married puts, particularly deep in-the-money buy-writes or married puts.check
>
> Use of buy-writes with little to no open interest outside of that trader's activity, resulting in all or nearly all of the call options being assigned. half a check since we don't know their other activity
>
> Repetitive nature of the use of buy writes. check, same time, same strike
>
> Trading in FLEX options in hard to borrow or Threshold List securities, particularly very short > term (often with one day expirations) FLEX options. check

> Trading exclusively in near term listed options in hard to borrow or Threshold List securities. check
>
> Trading in hard to borrow or Threshold List securities claiming the market maker exception from the locate requirement. Unconfirmed

> Multiple large trades that take place with the same trader acting as a contra party in several hard to borrow or Threshold List securities. Unconfirmed

So that is pretty darn convincing that something big is happening with a few big players. Someone has something to hide.

Dark Pools, Alternative Trading Systems, and Ex-Clearing

All of these boil down to the same principle: [the SEC only tracks FTDs that occur through clearing agencies](https://www.sec.gov/divisions/marketreg/mrfaqregsho1204.htm). Ex-clearing means literally it happens outside of a clearing agency. If you read that entire site (as I did unfortunately), you'll notice all close out rules only apply to clearing agencies and no mention is made to ex-clearing. Completely legal transactions can occur outside these systems [as long as both parties agree](https://www.finra.org/rules-guidance/rulebooks/finra-rules/6350a).

This dark pool data could potentially hide the FTDs for longer since they are not being tracked. However, it is unclear how long a large institution or market maker would accept not being delivered the shares. It could be a reset, or it could be a longer hold - most likely the former. Unfortunately this method has very little data behind it other than the large [dark pool data from the ATS](https://otctransparency.finra.org/otctransparency/AtsIssueData). Other posts have covered this, but if you look at all of the data from before the decapitated January squeeze, no week had more than 9.5M volume. But just before the February gamma squeeze, the week of February 15th which was by all accounts low volume low volatility, 18.9M volume.

This is the most recent data available, so further analysis is difficult to come by - but you get the point. Another method to reset the FTD timer.

Reborrowing

This one is actually super straight forward - if a lender calls back their share for any reason, the shorter can just borrow another share from someone else. The above scenarios are used when they are unable or unwilling to re-borrow shares.

Chapter 3: Estimation of shares

Now that you know the mechanisms of how short interest is hidden, let's dive into the particulars on what we know. Then make some reasoned assumptions on what it means for a true short interest. I will not be using FTDs because well... they are too small to care about right now and as I pointed out above, there are many methods to prevent them.

First, let's talk about my method calculation. For this, I will be using the baseline for total number of shares available of shares issued + *reported* shorted interest. Why? Because each shorted share counts as two: The lender still technically owns it, and so does the person who bought the shorted share. Any shares that exceed this number are hidden / naked shorted shares and represent stock dilution.

Now, to the calculation. Remember the references above? Let's dive in:

Known shares:

Insiders: 17,387,136

Institutions >5%: 48,377,553 (IJR also is listed as having more than 5%, but is an ETF so will be counted there)

ETFS: 10,520,774

*Reported* short interest: 10,189,630

Shares Issued: 69,936,000

Do the math - 69.9+10.2-(17.3+48.3+10.5) = 3,840,167 total legit shares available

So from just what *we know to be accurate, at least within the last month* there are less than 4M shares available for *all other institutions and retail*. That is not a lot of shares. This includes hedge funds, mutual funds, market maker delta hedging, and many more - they composed 62M shares in the last known date, 12/31/2020. Heck, I did analysis back a few weeks ago and [verified the short interest reported actually made sense with the data](https://www.reddit.com/r/GME/comments/lzj00a/super_conservative_calculation_puts_gme_short/). So let's go through a few categories:

Delta hedging

This is a theory that a [market maker needs to remain neutral in trades and profit off the bid-ask spread](https://www.thestreet.com/investing/options/how-to-trade-like-a-market-maker-10890392#:~:text=The%20way%20a%20market%20maker,with%20a%20long%20stock%20position.). One of their big functions is to provide liquidity for options - aka be the writer for the majority of options. In order to remain neutral, they also are theorized to purchase a number of shares equal to the delta at a certain strike / expiry for an option. Calls have a positive delta - aka they need to be long shares equal to the delta since selling a call is a short position - and puts have negative delta.

[The delta](https://www.investopedia.com/trading/using-the-greeks-to-understand-options/) in one sense represents the chance that the option will be in the money. So delta of 0.32 means it has about a 32% chance to be in the money. So for a call with a 0.32 delta, in order to be delta neutral, the market maker should buy 32 shares of that stock (since a contract is 100 shares). [Back in a previous DD,](https://old.reddit.com/r/GME/comments/lzj00a/super_conservative_calculation_puts_gme_short/) I calculated the delta hedging a market maker should have done: 14M shares. This hedging also is one of the causes of gamma squeeze (the gamma is the change in delta, or the rate of change - gamma squeeze is based on the delta changing quickly due to the price increasing).

Retail

Here is one that is really hard to calculate. But I'm going to use a combination of techniques. First, [/u/the_captain_slog](https://www.reddit.com/u/the_captain_slog/) wrote a [super insightful post about using the 13F filings to calculate the retail holdings](https://www.reddit.com/r/GME/comments/m74f7h/how_many_shares_does_retail_own_digging_through/). So I'm going to use that number as part of my baseline. Not going to repeat the calculations, but the number we'll go with here is 3.8M shares. But there is something missing - I don't see Webull or RH for instance in any of those filings. There are still more shares to be counted.

Now back to [my previous post](https://www.reddit.com/r/GME/comments/lzj00a/super_conservative_calculation_puts_gme_short/) - in my calculations, there were approximately 6.5M shares unaccounted for from the insider, institution, ETF, and delta hedging buckets when accounting for the reported short interest. Assuming that short interest was correct (it was so big I'm assuming there was no attempt to hide it), the number left over is likely the remaining retail. So this brings the count up to 10.3M retail ownership. This was before the hype really took off and I am going to use it as my floor for current retail ownership since there are likely similar levels of interest.

Okay, so now we have two other data points to include in this - 3.8M shares available, 14M shares needed to delta hedge, 10.3M shares for retail. That leaves..... 10.5M (edit: 20.5M - [/u/OneFacedCoin](https://www.reddit.com/u/OneFacedCoin/) found my braindead error here, best part about being transparent is I get free peer reviews... worst part is my mistakes are on full display after saying I like math...) shares missing from the inventory.... So far.

Putting it together

Now, back to the data - there were 62M shares that were in the 12/31/2020 *known* data which were either sold or held. So that is a 50% chance giving us 31M shares.... just kidding we can do better than that! Okay, so for a reasonable analysis, we can take the spreadsheet in [/u/the_captain_slog](https://www.reddit.com/u/the_captain_slog/) 's DD and use the average portfolio turnover. Since GME is super volatile, and that turnover is annual, let's make an *assumption* the annual turnover is the 1 quarter turnover for GME. [So if we take that turnover and use it to calculate the remaining GME shares after taking out the large players that gives another 27M shares.](https://docs.google.com/spreadsheets/d/1Fy0OUjIkaoUeyUJV1DkI4xAO_ixJWFeHeWH_fVhzt4o/edit?usp=sharing) - Check out column L for the calculation.

Where does that put us? Well, now this is the 10.5M (edit: 20.5M) missing and another 27M shares missing for 37.5M (Edit: 47.5M) shares missing from the current reports! With these estimation techniques, we are looking at a total of around 48M (Edit: 58M, which does match my last calculations eerily well) short interest! I had [calculated previously that there was about 58M SI](https://www.reddit.com/r/GME/comments/m074n6/gme_short_interest_58m_realistic_number_through/), and according to [S3, the reported SI has decreased by about 6M shares since I last ran the numbers](https://twitter.com/ihors3/status/1376576739854450693/photo/1). As I have said before, the S3 data (as well as Ortex which I don't have access to anymore) follows the reported SI quite well. And as I have said before, I think their algorithms broke during the squeeze because of the naked shorting which happened since they only track reported SI. So these more recent numbers correspond quite well to my original calculations! Honestly, I did not expect it to be that close.

Caveat: There are assumptions in these calculations, and the institutional ownership / retail are big assumptions. But I believe safe assumptions based on *known historical data*. However, 3.8M shares is not enough shares to hold retail / institution / MM hedging shares. Not even a single one of those categories.

[How about one more data point for confirmation bias](https://www.marketbeat.com/stocks/NYSE/GME/short-interest/) - Marketbeat has GME at 102M shares outstanding, making for 33M unreported short interest! Now I have no idea how they came up with this number, but my institutional ownership could be off by 5M, or hedging could be lower than it theoretically should be, etc. Again, grain of salt - but interesting.

Chapter 4: Why I am hodling

Long term potential. That is my reason - I honestly don't care about any squizzing because the long term prospects of the company are amazing. Let's talk about my evaluation - first, with the current price of 191, Gamestop is worth $13.3bln. This is mostly based on it being a brick and mortar store with the *potential* to become an e-commerce company. As a brick and mortar store, it was worth around $2bln. But wait, there's more! If we take the share dilution from heavy short interest calculated above, there are an additional 48M shares out there, so if those were removed from the pool the actual worth right now per share would be.... 322 per share. So the undiluted value of the company is even greater - but we aren't done.

Now, e-commerce companies are evaluated much higher than brick and mortar. I mentioned the current price reflects only the *potential* of becoming an e-commerce company, so let's look at some other companies. First - Amazon: $1.5 trillion with a 75 P/E ratio. Aka they are priced at 75x of their profits they earn in a year. The [average P/E ratio of the S&P500 is 13-15](https://www.investopedia.com/investing/use-pe-ratio-and-peg-to-tell-stocks-future/#:~:text=The%20average%20P%2FE%20for,compared%20to%20the%20overall%20market.) Amazon is a mature company, and is viewed as the pinnacle of e-commerce - but still, that is 6x higher than the average company.

But what about companies who are much younger? [Chewy](https://www.nasdaq.com/market-activity/stocks/chwy) is priced at $35bln, and has yet to generate profits. [Snapchat](https://www.nasdaq.com/market-activity/stocks/snap) is valued at $82bln and has yet to generate a profit. [Roblox](https://www.nasdaq.com/market-activity/stocks/rblx) is priced at $37bln as a gaming platform for a single brand. [Roku](https://www.nasdaq.com/market-activity/stocks/roku) is a TV streaming platform valued at $42bln. [Carvana](https://www.nasdaq.com/market-activity/stocks/cvna) is a used car platform and is valued at $42bln. Getting the drift? On top of all of this, every single one of these companies is considered a strong buy by NASDAQ. The lowest of these is $35bln for Chewy - which would represent $500 / share for GME. The lowest!

So now just think if the *potential* for an e-commerce turnaround gets the stock up to $191, what will the actual plan and execution get when it is being run by Amazon execs and Ryan Cohen who started Chewy. $500 is the floor for the long term potential in my eyes.

Chapter 5: Prediction for the next week

When looking at predictions, forget 'good whales' - all the big players are trying to make money. There isn't any 5D chess happening with the whales, what is happening is the short players *and* long players are waiting for opportunities. The low volatility represents low liquidity (people be hodlin) and waiting for an opportunity. The dip after earnings was an opportunity for the short players. The Cohen announcement and gamma squeeze were opportunities used by the long players. So there are two possibilities I see (1) gamma squeeze or (2) the e-commerce transition plan is announced. The next big activity is likely going to be driven by one of these factors. Outside of this, due to the low liquidity, we'll likely see more of the same from this week. But the longer we see this low volatility, the greater the opportunity for (1).

I have said again and again in my more recent posts that low volatility is great for lowering IV. While some have said the IV is still sky high, [the IV is quickly approaching the same levels that gave us the gamma squeeze in February](https://imgur.com/gallery/lPjVn9d). Look at it plummet! This is amazing. I was right all last week saying there would be low volume and low volatility. I have said that nothing will happen until there is a big announcement or gamma squeeze. Well, the probability of a gamma squeeze is much higher now than last week - all because it was boring. So here is my prediction: Another sideways day tomorrow, maybe a modest gain if any due to the recent jobs report. Tuesday and / or Wednesday could get real interesting with a chance of gamma Squizzing. However, it is far from guaranteed - if it doesn't happen Wednesday, it probably won't happen this week since the theta decay from options gets real high on Thursday / Friday. In which case look for the next week to possibly be exciting.

No guarantees on anything though. Until Gamestop comes out and hits us with a detailed and convincing E-commerce plan, I think the chances of nothing happening are greater than even a gamma squeeze. But remember - a squoze is not why I am hodling.

Epilogue

The good news - all of these naked shorted shares will have to be covered, they were sold to someone who will eventually collect. Everyday the stock remains high, the shorts bleed money through interest fees and doing these timer resets. Be patient, don't trade on fear or excitement - trade on information.

I am not a financial advisor, cat, nor jedi. This isn't financial advice, butthole in your face, nor force lightning. I am not a registered broker, this is only my opinion based on my individual investing style which is not meant appropriate for everyone. I provided links in here for you all to do your own research, because in the end that is what you should base any financial decisions. The stock market is inherently risky, and there is no 100% sure thing, so only invest what you can afford to lose.
