Some additional thoughts on statistical analysis: DD for March 4 and 5
======================================================================

| Author       | Source       | 
| :-------------: |:-------------:|
|  [u/oaf_king](https://www.reddit.com/user/oaf_king/) | [Reddit](https://www.reddit.com/r/GME/comments/lxhatz/some_additional_thoughts_on_statistical_analysis/) | 

---

[DD](https://www.reddit.com/r/GME/search?q=flair_name%3A%22DD%22&restrict_sr=1)

Hi all,

This is a follow-up to my post "[Y'all, this is statistically significant action!](https://www.reddit.com/r/GME/comments/lx4gbv/yall_this_is_statistically_significant_action/)"

I replied to comments I could quickly address, but there were a few topics I'd like to spend more time on. This is not meant to be financial advice, but rather information to elaborate on my use of statistics. Consider this DD for March 4 and 5, but possibly beyond those dates as well.

Regarding confirmation bias and correlation

First, in [my morning post yesterday](https://www.reddit.com/r/GME/comments/lwsiai/just_for_fun_for_your_confirmation_bias_needs/) I state up front that it's "an educational / fun post to keep up the motivation during hump day this week." In my post following market close yesterday, I state "Warning: more confirmation for your bias ahead." Playful tone aside, I trust most of you recognize both the allure and dangers of an echo chamber. While I take what I post seriously, you ultimately decide what you do with your money. Both here and in everyday life, I believe critical thinking means being responsible for one's convictions---the more work that goes into the process, the more durable the result.

Second, with respect to any statistical model, I cannot stress enough that correlation =/= causation. Just because one data set is congruent with another, it does not mean one is the result of the other. Here's [a fun website](https://tylervigen.com/spurious-correlations) with examples.

On the use of Spearman's Rho

Also known as Spearman's rank correlation coefficient, Spearman's *ρ*, and---for the initiated---"Spearmint Rhino" (JK. Don't cite this in an academic paper.) This technique assigns a rank to each data point in a set in either ascending or descending order, and then the set of ranks is compared with another ranked data set. Here's an illustration:

[![r/GME - Some additional thoughts on statistical analysis: DD for March 4 and 5](https://preview.redd.it/7ol3lsbxazk61.png?width=749&format=png&auto=webp&s=78ca1777ea8e333e0117df9a76c94035e996e98b)](https://preview.redd.it/7ol3lsbxazk61.png?width=749&format=png&auto=webp&s=78ca1777ea8e333e0117df9a76c94035e996e98b)

The values under "Set A Rank" are equal to the rank (in ascending order) of the values under "Set A Close"; these values are then compared to those under "Set B Rank."

This approach removes the effects of price volatility: the magnitude of price change does not matter; what matters is the relative order as a result of price change. A [minimum sample size of 7](https://www.researchgate.net/post/Sample_size_in_Spearman_rank_correlation) is needed for the analysis to hold weight. This is why my data includes several dates prior to a large price spike in each data set (denoted as Day 6: January 13 in set A and February 24 in set B).

Here's the graph I shared after market close yesterday:

[![r/GME - Some additional thoughts on statistical analysis: DD for March 4 and 5](https://preview.redd.it/w7zgoqwxbzk61.png?width=925&format=png&auto=webp&s=7becd18b253d38ecccdb2ed27abc52217766d1b8)](https://preview.redd.it/w7zgoqwxbzk61.png?width=925&format=png&auto=webp&s=7becd18b253d38ecccdb2ed27abc52217766d1b8)

A comparison of price activity between the January run-up and our (apparent) current one.

The activity can be summarized as:

-   Relatively flat prices from Day 1 to 5 (inclusive)

-   A dramatic jump occurs on Day 6 (from $19.95 to $31.40 in Set A and from $44.97 to $91.71 in Set B)

-   An increase from Day 6 to Day 7

-   A slight decrease from Day 7 to Day 8

-   An increase from Day 8 to 9

-   A slight decrease from Day 9 to 10

-   An increase from Day 10 to 11

Let me be clear: the above summary of activity is identical (up to the time of writing) across both sets. This is why the current values of Spearman's *ρ* = 0.9455 and a p-value (2-tailed) of 1E-05 (more or less 0.00001) is noteworthy. A p-value this low is statistically significant: random chance alone is incredibly unlikely to produce the matching pattern described above.

Some quick tests, using adjusted dates

One recurring question was what the results would look like if the compared sets were different. I conducted two tests that produced the following values:

1.  Keeping Set A the same, but adjusting Day 1 of Set B to be February 16, Spearman's *ρ* = 0.74546; p-value (2-tailed) = 0.00845

2.  Keeping Set A the same, but adjusting Day 1 of Set B to be February 12 [February 15 was President's Day; NYSE was closed], Spearman's *ρ* = 0.48182; p-value (2-tailed) = 0.13343

So, while I concede I approached the test in a non-random manner because the day of the price spike jumped out at me, even if we adjusted the data set by one and two trading days, the correlation is reduced. Find me five days of flat pricing followed by a large jump and then a back-and-forth pattern of increase and decrease---with the changes following a magnitude that does not skew ranks---and you'll have found a run-up we all apparently missed.

Comparison with other tickers

Another recurring question was what the correlation would be compared to other tickers. While my original intent was to demonstrate the bizarre similarity in both cases of a GME run-up, a comparison with other tickers can showcase just how significant our current numbers are.

I conducted some tests that compared Set B with corresponding dates and closing prices from tickers I figure most are interested in. I chose to use Set B (February 17 to March 3 inclusive) and not Set A here because they are statistically equivalent and I'm more interested in our current run-up. I don't know where we're at with naming other tickers at the moment, so as a precaution I'm using descriptions to describe what I compared with GME. Just in case though, [here's my input data set](https://imgur.com/v0vOBpQ.png).

| Ticker | Spearman's *ρ* | p-value (2-tailed) |
| --- | --- | --- |
| Theatre | 0.80909 | 0.00256 |
| Non-Apple Fruit Company | -0.38269 | 0.24539 |
| Indestructible Cell Phone | -0.35781 | 0.27996 |
| S&P 500 | 0.61818 | 0.04265 |
| Common Volatility Index | -0.58182 | 0.06042 |
| Particular Retail Index Fund | 0.81818 | 0.00208 |

This is neat to see: the theatre and the retail index fund have a healthy level of correlation and a low p-value. Conversely, it looks like sentiment has dispersed for two certain companies that were popular back in January. With respect to the S&P 500, I would say the correlation is lukewarm as that fund tracks companies based on market cap: I wouldn't expect activity in this fund to follow (positively or negatively) too closely the activity of GME (though note the low p-value). In terms of the volatility index, there's some indication that GME and volatility are inverted, but I don't know enough of that particular index to comment further.

I ran these comparisons because they were requested. I leave it to smarter folks to discern possible explanations for the strong (Spearman's *ρ* > 0.8) correlations above, as well as the index funds.

What to look out for on March 4 and 5

In case it was missed, I updated my last post with a quick analysis of volume. It was one of the common requests made in the comments, and I'm glad people thought to ask. Here's the chart comparing volume for GME (returning to the original data for Sets A and B):

[![r/GME - Some additional thoughts on statistical analysis: DD for March 4 and 5](https://preview.redd.it/4278cbv7fzk61.png?width=1036&format=png&auto=webp&s=4e6c3b76da363da0b956cb085517e0a319a63981)](https://preview.redd.it/4278cbv7fzk61.png?width=1036&format=png&auto=webp&s=4e6c3b76da363da0b956cb085517e0a319a63981)

Spearman's ρ = 0.7364 with p-value (2-tailed) = 0.00976

Observe that in the January run-up, volume had declined just before the explosion in price. As of market close on March 3, the situation is similar (and supported by the really low p-value). So, veteran GME holders know the game: if volume is low, pay no attention to price drops because it's artificially suppressed. Instead, take comfort and remember the price has steadily increased following a major spike. Like I said in my last post: History is rhyming hard. Keep an eye on volume in the next several days: the next time it surges dramatically, say bye to the earth. (Note that in the last 20 minutes of March 3, there was a boost in volume that led to the price increase.)

I also suggest keeping an eye on the Moving Average Convergence Divergence (MACD) indicator. [u/Bootheskies](https://www.reddit.com/u/Bootheskies/) messaged me and brought it to my attention. I'm still learning about what a MACD even is (and am now craving McDonald's for my next meal), but here's a quick overview that I hope others can build on. [u/Bootheskies](https://www.reddit.com/u/Bootheskies/) says she doesn't want credit or karma, but I want to acknowledge her role in these observations:

-   Here's a picture she took of a MACD chart for GME: <https://imgur.com/gallery/r3rHAtu>. Note that it covers approximately the last two months

-   When the white curvy line is on top of the red line, the price is moving up; note the run-up in late January

-   Conversely, when red is over white, the price moves down; note how the red curve overtaking the white curve coincides with the red weeks in February

-   Take note of the blue arrow on the right (where white has once again overtaken red); these lines have now also risen above the middle line (also known as the "signal line," which as I understand it is a trigger for buy and sell signals)

-   Compare this with the blue arrow on the left, where the same observations occurred prior to the January run-up. This time around, *we are starting with a much higher price entering a run-up*.

-   Admittedly, I'm leaving out some of the comments she shared with me because I don't understand it myself, and I don't want to create confusion. While she and I agree that the MACD indicator supports the models I charted, we do not know what date the buying will spike.

Sorry, [u/Bootheskies](https://www.reddit.com/u/Bootheskies/), for not doing your explanation justice. But this is where the community is at its best: Might those with more knowledge of MACD provide more insight?

Closing thought

I've made several posts here over the last week or so and what keeps me going is the enthusiasm and energy for making meaning of events as they happen. After everything I've said, please remember that while no date is certain, the probability of an upcoming price spike similar to that of January 22 and after (up to January 28) is almost certain. Whether or not external forces halt that spike is impossible to say. All I know is that I'm ready for take off with you beautiful apes.
