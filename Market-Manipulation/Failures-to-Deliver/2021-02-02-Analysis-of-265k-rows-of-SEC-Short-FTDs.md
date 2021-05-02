Data-Driven DD: I analyzed 265,000 rows of SEC Short Fails-to-Deliver data so you don't have to! (Extremely important data for Counterfeit Stock theories)
==========================================================================================================================================================

| Author       | Source       | 
| :-------------: |:-------------:|
|  [u/556YEETO](https://www.reddit.com/user/556YEETO/) | [Reddit](https://www.reddit.com/r/wallstreetbets/comments/lb8hjc/datadriven_dd_i_analyzed_265000_rows_of_sec_short/) | 

---

[DD](https://www.reddit.com/r/wallstreetbets/search?q=flair_name%3A%22DD%22&restrict_sr=1)

The GME SEC Data and Hedge Fund Shitfuckery: A Deep Dive

As I'm sure many of you who have been following the "Counterfeit Shares" theory about the various short attacks on $GME have seen, the SEC publishes lagged data on the cumulative number of Fails to Deliver for every company. If you aren't caught up with the latest info on the counterfeit share theory, take a second and read [u/johnnydaggers](https://www.reddit.com/user/johnnydaggers/)'s [post](<https://www.reddit.com/r/wallstreetbets/comments/l97ykd/the_real_reason_wall_street_is_terrified_of_the/>) laying out the issue with hedge funds counterfeiting shares and how it relates to GME. Much of the analysis in Johnny's post comes from an article ["Counterfeiting Stock 2.0"](<http://counterfeitingstock.com/CS2.0/CounterfeitingStock.html>) which is definitely worth a read if you have the time and patience to do a deep dive into the evil shit carried out by hedge funds.

TLDR of Johnny's post: Hedge funds create a bunch of stock out of thin air and short it, selling the counterfeit shares on the open market and driving the price of a company down. They then fail to come up with the shares they sold in time, so the "counterfeit" shares are never backed up by real shares. This could be happening on a massive scale with GME, and Hedge Funds could have far greater exposure to GME than previously thought.

The Data:

I noticed that while [u/johnnydaggers](https://www.reddit.com/user/johnnydaggers/) and later [u/Peteskies](https://www.reddit.com/user/Peteskies/) used data from the SEC releases in their posts, the data they actually showed was only a small piece, and lacked very important context. So, with that in mind, I took the SEC Fails-to-Deliver data [releases](<https://www.sec.gov/data/foiadocsfailsdatahtm>) for both halves of November and December and the first half of January and took a look at what was going on using some pivot tables. I thought given the sheer amount of data (1.5 million cells) it would be tough to load in Excel but it actually ended up being pretty easy. (probably helped that my day job is just alternately making pivot tables and slamming my head into the wall, I've gotten pretty good at both)

IMPORTANT NOTE: THIS RELEASE EXTENDS TO JANUARY 14TH, 2021. THESE ARE NOT CURRENT CUMULATIVE OUTSTANDING FAIL-TO-DELIVER LEVELS

Fails-to-Deliver Distributions:

First, take a look at this handy histogram(ish) of companies with outstanding Fails-to-Deliver and their outstanding "counterfeit share" (cumulative Fails-to-Deliver) numbers:

[![r/wallstreetbets - Data-Driven DD: I analyzed 265,000 rows of SEC Short Fails-to-Deliver data so you don't have to! (Extremely important data for Counterfeit Stock theories)](https://preview.redd.it/6dmfpfql47f61.png?width=1440&format=png&auto=webp&s=bf38fea8f5de2e45b36b48853f4d7afaca8f6c28)](https://preview.redd.it/6dmfpfql47f61.png?width=1440&format=png&auto=webp&s=bf38fea8f5de2e45b36b48853f4d7afaca8f6c28)

As you can see, GME is way outside of the pack when it comes to Fail to Delivers, and has significantly more "counterfeit shares" (FTDs) than almost any other company. The exact number comes in at a cool 621,483 shares. The x-axis scale isn't even linear, and you can see significant jumps in the last quarter.

If you think that's some crazy shit, wait until you see the distribution of Fail-to-Delivers per company by the dollar value of counterfeit shares ((Closing Price)*(# of Outstanding Fails-to-Deliver)):

[![r/wallstreetbets - Data-Driven DD: I analyzed 265,000 rows of SEC Short Fails-to-Deliver data so you don't have to! (Extremely important data for Counterfeit Stock theories)](https://preview.redd.it/024mdiv147f61.png?width=1616&format=png&auto=webp&s=270fc53a5455994545a864e8b8e9c304b0e57b5c)](https://preview.redd.it/024mdiv147f61.png?width=1616&format=png&auto=webp&s=270fc53a5455994545a864e8b8e9c304b0e57b5c)

GameStop has the SECOND HIGHEST Fails-to-Deliver net dollar value of all 5,147 stocks with current fail-to-delivers (as of 1/14/21). NINETEEN MILLION DOLLARS of stock floating around that was simply created out of thin air. Here the x-axis isn't even linear either --- if it were to scale, GME would be several meters to my right. Wild.

Cumulative Fails-to-Deliver of GME over Time:

Moving on to more interesting (and potentially more troubling) data, I took a look at the Fails-to-Deliver values over time for GME. I decided to go back to the beginning of November, then look at every number the SEC had released since on FTDs for GME. This is crucial context for the numbers that have been thrown around by [u/johnnydaggers](https://www.reddit.com/user/johnnydaggers/) and [u/Peteskies](https://www.reddit.com/user/Peteskies/).

[![r/wallstreetbets - Data-Driven DD: I analyzed 265,000 rows of SEC Short Fails-to-Deliver data so you don't have to! (Extremely important data for Counterfeit Stock theories)](https://preview.redd.it/myt4zxy347f61.png?width=1328&format=png&auto=webp&s=603b5d5f0a623dc0dc9ef0df1f3da05e7361340f)](https://preview.redd.it/myt4zxy347f61.png?width=1328&format=png&auto=webp&s=603b5d5f0a623dc0dc9ef0df1f3da05e7361340f)

Now, this one is a lot less clear-cut than those histograms I just wrote about. As you can see, there have been huge fluctuations in the amount of "counterfeit stock" (Fails-to-Deliver) on the market. There is a definite pattern of Hedge Funds running up Fails-to-Deliver during GME surges and then covering once the price slumps a bit. I've talked with one of my sources involved with hedge fund operations, and he said this is pretty standard procedure --- when you sell a naked short and the price spikes, you talk it out with your broker and get a few more days to cover. So really, this pattern is more or less normal. It's the stupidly large amounts Fails-to-Deliver that are getting churned that is the irregular part.

Here's a good spot to bring up my main concern with the kind of analyses that [u/johnnydaggers](https://www.reddit.com/user/johnnydaggers/) and [u/Peteskies](https://www.reddit.com/user/Peteskies/) were putting out. You can see that there were 1.8 million Fails-to-Deliver on GME on December 2nd, but that number was basically completely covered by the 16th. Based on that data it seems at first glance that, for the most part, these reported Fails-to-Deliver are Hedge Funds/Brokers trying to avoid covering while high and simply waiting for the next dip. This data alone IS NOT SUFFICIENT to prove that there is an enormous, market-moving quantity of Fails-to-Deliver floating around the market. Of course, right after this data cuts out, GME shoots to the moon (300+), and I would expect a lot of naked short vendors were caught with their pants down. Maybe they all covered on the recent dips, maybe loads of Fails-to-Deliver are still out there.

A table with that GME info from the graph above for any lurking nerds:

[![r/wallstreetbets - Data-Driven DD: I analyzed 265,000 rows of SEC Short Fails-to-Deliver data so you don't have to! (Extremely important data for Counterfeit Stock theories)](https://preview.redd.it/0pj2hh0647f61.png?width=1090&format=png&auto=webp&s=dcf2d64f6777218dece7735075b779fb51e28cca)](https://preview.redd.it/0pj2hh0647f61.png?width=1090&format=png&auto=webp&s=dcf2d64f6777218dece7735075b779fb51e28cca)

Some Questionable Inferences and My Retarded Conclusions:

So, what's the takeaway here, other than don't trust everything you read on WallStreetBets? I think there are a few lessons. First, even though Fails-to-Deliver numbers were bouncing all over the place, including being completely covered on 12/16, I think it's important to keep in mind that GME having this volume of Fails-to-Deliver, both in shares and in dollars, is extremely irregular compared to everything else. Could just be the fact that GME is an insane stock with insane volatility,* or could be indicative of something more.

**Yet, this data is from back before GME became mainstream --- GME in December was not an "unprecedented situation" like we have now. Thinking back to then, the high Fails-to-Deliver numbers are even more significant.*

A Possibility of Hedge Fund Armageddon:

I want to take a second to talk about one of the diagrams from the good folks who wrote ["Counterfeiting Stock 2.0"](<http://counterfeitingstock.com/CS2.0/CounterfeitingStock.html>), detailing both the "surface level" indicators of Disclosed Shorts and Fails-to-Deliver, and the below-the-surface hidden pathways that they believed pumped counterfeit shares into our financial system. Here it is:

[![r/wallstreetbets - Data-Driven DD: I analyzed 265,000 rows of SEC Short Fails-to-Deliver data so you don't have to! (Extremely important data for Counterfeit Stock theories)](https://preview.redd.it/v3io9bj847f61.jpg?width=1086&format=pjpg&auto=webp&s=21d67bbec3d7d4e3b2012b3d51cdaf462ae3318d)](https://preview.redd.it/v3io9bj847f61.jpg?width=1086&format=pjpg&auto=webp&s=21d67bbec3d7d4e3b2012b3d51cdaf462ae3318d)

As you can see, the Counterfeiting 2.0 authors believed that Fails-to-Deliver were just the tip of the iceberg. Below the surface (and out of the sight of the SEC), they believed there was a massive volume of shares that had been "laundered," through foreign exchanged, offshore funds, or even gaps in the Continuous Net Clearing system at the DTCC. These stocks, theoretically, go from Fails-to-Deliver to simple counterfeit shares, or even straight to counterfeits. The arguments in the Counterfeiting 2.0 paper go way over my head as a simple retard, but I get the gut feeling at least some of them are accurate.

If, hypothetically, (please read this part in your best Ben Shapiro voice), the arguments in Counterfeiting 2.0 are true, then it is highly likely that the huge Fails-to-Deliver churn on the surface is just the tip of a massive illegal counterfeit short position. GME BULLS, listen up. If this counterfeit short position does exist, then it was probably entered back when GME was being driven towards bankruptcy, at a share price somewhere in the $15/20 range, and possibly expanded when GME was being driven down below $5. There are actually interesting data to suggest that this is a plausible scenario. First, the fact that, as [/u/DeepFuckingValue](https://www.reddit.com/u/DeepFuckingValue/) noted a year ago, the market cap of GME was driven below the net value of its assets. Obviously, this happens from time to time, but it's indicative of an extremely artificially depressed valuation. Secondly, the central use of illegal naked shorting is in driving companies to bankruptcy, and it did seem like GME was on its way out. Looking at GME as a scummy hedge fund manager, it would have made a very attractive target for a naked-short dilution attack.

These illegal short positions, if they were not covered by cautious (lol) Hedgies at the beginning of the GME runup, would have increased 50-100x in dollar value as the share price of GME rose. That's 5,000-10,000% for those who can't do basic math. Now I don't know if this scenario would be enough to crash the market, but it would certainly be enough to make a lot of extremely powerful people (currently engaged in a criminal enterprise) desperate and very, very angry. This hardly needs saying, but rich bastards have killed for far less than a billion dollars. Here, there could be tens of billions on the line.

So, that's the mega-bull case. We, the tards of WSB, expose billions in financial crime. The SEC rappels into Citadel and arrests everyone, Robinhood goes bankrupt, and all our wives and their boyfriends get filthy rich. However, there is also a very significant BEAR case here. If the regular, everyday investors who wrote Counterfeiting 2.0 were in fact retards like us, then there's a significant chance that they simply got it wrong. Maybe there is no sea of hidden counterfeit short positions, and maybe this whole Fails-to-Deliver thing is just rich assholes using extra trading days to cheaply sell shorts. What then? In that case, I would bet my left nut that all of the outstanding Fails-to-Deliver have been covered in the recent slump, and this whole exciting report is largely irrelevant to the future performance of GME.

I'm not going to make the case that either the bulls or the bears are right (even though my gut is with the bulls) because I simply don't have the information or mental capacity to make that call. Look at the data yourself, and draw your own conclusions. Retail is facing an enemy with more capital, more information, more experience, and fewer morals. Whichever way it goes, it's going to be an ugly fight.

Positions: 12 shares (Bought 50 at $20, sold 50 at $250, bought back in 12 at $300). I plan to hold until either $4,000 a share or things go to shit.

I am not a financial advisor, and I do not advise any readers to make financial decisions based on my opinions or the information presented in this report.

TLDR: the cumulative Fails-to-Deliver volume on GME is massive compared to the rest of the market. However, is also extremely volatile, and small compared to the float. It is possible that high Fails-to-Deliver volume is a result of massive illegal share counterfeiting by shorts.

Edit: shout out to [/u/zjz](https://www.reddit.com/u/zjz/) for finally approving the post, may you live long and stay retarded!
