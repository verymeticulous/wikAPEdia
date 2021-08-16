Yes, those patterns y'all keep posting are real! The similarity in meme stock price movement is statistically significant and differs significantly from a control group of boomer stocks (answer to u/HomeDepotHank69).
========================================================================================================================================================================================================================

| Author       | Source       | 
| :-------------: |:-------------:|
|  [u/squirrel_of_fortune](https://www.reddit.com/user/squirrel_of_fortune/) | [Reddit](https://www.reddit.com/r/Superstonk/comments/ns8dhk/yes_those_patterns_yall_keep_posting_are_real_the/) | 

---


[DD 👨‍🔬](https://www.reddit.com/r/Superstonk/search?q=flair_name%3A%22DD%20%F0%9F%91%A8%E2%80%8D%F0%9F%94%AC%22&restrict_sr=1)

So, this post is in response to [u/HomeDepotHank69](https://www.reddit.com/u/HomeDepotHank69/) 's request for DD into correlation between stock price movements.

TL/DR:

1.  Two different scientific methods showing that there is similarity and correlation between certain meme stocks and that this increased since Jan.

2.  A machine learning method asked to put stonk data into clusters based on their patterns over the last half year put the meme stonks GME, AMC, KOSS, and others together regardless of which bit of price data you choose to look at. Look at the pictures!

3.  Before Jan 2020, meme stocks (as a group) were not particularly correlated with each other, after Jan they were very well correlated with each other. (In fact before Jan AMC and GME were negatively correlated, after Jan they were very closely correlated).

4.  On average, a control basket of boomer stocks have not changed in their correlation to each other. The basket of meme stonks have changed (after Jan 2021) to become highly correlated with each other (to a high statistical significance).

Pearson R2 (r-squared) is a quick n dirty way to do the comparison between stonks, so I also wanted to put the data into an ML algorithm that would look for clusters in it, and see if that algorithm, knowing nothing about the situation other than the stock price and volume info, would group the stocks the same way we might by eye.

Question 1: Would a machine learning algorithm cluster the stocks into meme and boomer? As in, what general patterns exist in these stock movements?

Question 2: Are meme stocks significantly correlated with each other? Are they correlated more than a control set of boomer stocks?

Bag of meme stocks as suggested by [u/HomeDepotHank69](https://www.reddit.com/u/HomeDepotHank69/): GME, AMC, KOSS, NAKD, NOKK, BBBY, VIX

Control bag of boomer stocks: AMZN, CVS, GSK, RDS-B, WEN, GM, IBM. These were selected semi-randomly to try and come from different areas of the economy. And I added Wendy's just cos. And I think I picked general motors randomly, but maybe I was primed by GME's ticker.

See picture below: normalising the daily high price to the highest price over the year to date, boomer stocks are dotted lines, meme stocks solid lines, they look different to me.

[![r/Superstonk - Yes, those patterns y'all keep posting are real! The similarity in meme stock price movement is statistically significant and differs significantly from a control group of boomer stocks (answer to u/HomeDepotHank69).](https://preview.redd.it/glxb4bjuk9371.png?width=815&format=png&auto=webp&s=c3260c91c53b7919792481bd61364514a87c72fb)](https://preview.redd.it/glxb4bjuk9371.png?width=815&format=png&auto=webp&s=c3260c91c53b7919792481bd61364514a87c72fb)

This is the high price, after normalisation to the higher price seen in the last year to date. I don't wanna lead you apes, but I would say that the boomer stocks (dashed) look different to the meme stocks (non-dashed). But that is not scientific enough!

Next picture: after the normalisation described in the methods section below to remove the general background movement of the stock market. I did not expect KOSS to be that similar. Maybe Hank did. The numbers in this plot are large due to the normalisation, but we don't care about the exact numbers we care about the patterns here. This graph shows us that GME and its friends are doing something really fucking odd this year to date!

[![r/Superstonk - Yes, those patterns y'all keep posting are real! The similarity in meme stock price movement is statistically significant and differs significantly from a control group of boomer stocks (answer to u/HomeDepotHank69).](https://preview.redd.it/g85bn2a6l9371.png?width=832&format=png&auto=webp&s=84af213daa4b5c9857416b8691766e128f283a2b)](https://preview.redd.it/g85bn2a6l9371.png?width=832&format=png&auto=webp&s=84af213daa4b5c9857416b8691766e128f283a2b)

Normalised as described to remove the NASDAC background

Question 1. Are meme stocks similar to each other? Would they be clustered together?

We get very similar results for the 5 dimensions of the data (high price, low price, open price, close price , adjusted close price and volume). Low and high prices results showed the largest effect. The algorithm doesn't have a great time clustering over the entire time period, but we see something interesting when we split the data into June-Dec 2020 (before) and Jan-June 2021. I think low price is the most interesting so I will use this as an example. All the data from here on is the Low price of the day, although similar things were seen with the other prices.

How to 'read' these pictures, the grey lines are the stocks over the time period, the red line is what the algorithm thinks is the middle of this cluster of stocks (sort of like a corrected average). The data is normalised for the algorithm, so the y axis is a relative price, the days are days since the start of the time period (6 june 2020 (before) or 1st Jan 2021 (after)).

Before (in 2020):

[![r/Superstonk - Yes, those patterns y'all keep posting are real! The similarity in meme stock price movement is statistically significant and differs significantly from a control group of boomer stocks (answer to u/HomeDepotHank69).](https://preview.redd.it/hfgwsop9m9371.png?width=539&format=png&auto=webp&s=2bd45d3443dcd41e46fbd395ee4a4b2aee8dfeac)](https://preview.redd.it/hfgwsop9m9371.png?width=539&format=png&auto=webp&s=2bd45d3443dcd41e46fbd395ee4a4b2aee8dfeac)

Stonks behaving normally. Note AMC and GME are in different clusters. Cluster 1 is stocks that go down, cluster 2 is stocks that go up. This is for the June 2020 to Dec 2020

The best answer is 2 clusters:

Cluster 1: ['AMC', 'NAKD', 'NOKK', 'VIX', 'CVS', 'GSK', 'RDS', 'WEN', 'IBM']

Cluster 2: ['GME', 'KOSS', 'BBBY', 'AMZN', 'GM']

After (2021):

The two measures gave the best answer 2 clusters and four clusters.

The two cluster answer:

[![r/Superstonk - Yes, those patterns y'all keep posting are real! The similarity in meme stock price movement is statistically significant and differs significantly from a control group of boomer stocks (answer to u/HomeDepotHank69).](https://preview.redd.it/05djchs4n9371.png?width=539&format=png&auto=webp&s=fcc287bcdf9b010c49df232ecaa990412e486c58)](https://preview.redd.it/05djchs4n9371.png?width=539&format=png&auto=webp&s=fcc287bcdf9b010c49df232ecaa990412e486c58)

Meme stonks in cluster 1, boomer stocks in cluster 2, roughly. (y axis is mislabelled sorry, these are low prices). This is Jan 2021-June 2021

*2 clusters (best on one measure)*

Cluster 1: ['GME', 'AMC', 'KOSS', 'NAKD', 'BBBY', 'GM']

Cluster 2: ['NOKK', 'VIX', 'AMZN', 'CVS', 'GSK', 'RDS', WEN, IBM]

The 4 cluster answer

*4 clusters (best on another measure)*

[![r/Superstonk - Yes, those patterns y'all keep posting are real! The similarity in meme stock price movement is statistically significant and differs significantly from a control group of boomer stocks (answer to u/HomeDepotHank69).](https://preview.redd.it/o1jdl6vcn9371.png?width=802&format=png&auto=webp&s=720b780ca6a28d6db78c354b6f3eff8c9fc59ad3)](https://preview.redd.it/o1jdl6vcn9371.png?width=802&format=png&auto=webp&s=720b780ca6a28d6db78c354b6f3eff8c9fc59ad3)

Cluster 1. Some meme stocks and GM, peak around Jan, cluster 4, GME and AMC, doing their squeeze thing? Cluster 2 and 3, normal stocks doing normal things. (Again mislabelled y axis, sorry, is defo low prices). Jan 2021- June 2021

Cluster 1: ['KOSS', 'NAKD', 'BBBY', 'GM']

Cluster 2: ['VIX', 'AMZN', 'GSK', 'RDS']

Cluster 3: ['NOKK', 'CVS', 'WEN', 'IBM']

Cluster 4: ['GME', 'AMC']

I got the same general pattern on the high price as well. AMC GME KOSS BBBY tend to be clustered together.

Look at cluster 4's graph, isn't it pretty? And after the normalisation and all that shit (removing market background), we see that GME and AMC are higher than they were in Jan. Maybe they got a way to run?

Conclusion 1:

There is something similar in the meme stock price movement that causes the algorithm to put them together and this is seen across the 5 data dimensions (high price, low price etc). Looking at the four cluster answer, we see there are two different meme stock behaviors, the Jan price increase then settle for KOSS NAKD BBBY and GM (GM is following GME possibly cos of fat fingers, see later), whilst our meme stonks AMC and GME are increasing from Jan til now...

Question 2.

Is there a statistically significant correlation between the price action of meme stocks?

Significance: how this works:

The Pearson R2 measure (R2, should be R2 but I don't know how to superscript) is a measure of how correlated the stocks are. An R2 of +1 means an exact positive correlation (e.g. $GME goes up when $MEH goes up), an R2 of -1 means an exact negative correlation ($GME goes down when $MEH goes up), and R2 of 0 means no correlation (i.e. the two stonks are unrelated). It's not the best method to do this comparison, but it's the one we got!

The p value is a measure of significance, if it is over 0.05 then the results are considered not statistically significant at all. The smaller the p value is, the more significant. (In more statistical language, a small p value relates to a small chance that the result seen is due to random fluctuations and not a relationship between the stonks). A p value under 0.0001 is highly significant. Where I've put p << 0.0001 I saw some TINY numbers, like a p values in the 1x10^{-20} region. You need to have significant results for your results to mean anything. (Any stats geeks in da house? Yes, we could discuss the difference between statistical significance and scientific significance, here, but we didn't. soz).

If we have a large R2 there is a correlation, if it is backed up by a small p number it is a significant correlation and therefore we believe it is not a spurious correlation (i.e. bullshit).

We use IBM as our archetypal boomer stock as no one ever got fired for buying IBM!

OK so looking at GME's price movement against other stonks before 2021:

Looking at the R2 on low and high prices BEFORE (June - Dec 2020):

MEME to MEME

GME to AMC : R2 = -0.73, p ~<<0.0001 (Negative CORRELATION! Very significant) (p value is 1X10^(-25)!)

GME to KOSS : R2 = 0.55 , p <<0.0001 (middling correlation, Very significant)

MEME to Boomer

GME to IBM : R2 = -0.7, p << 0.0001 (neg correlation, very significant)

BOOMER to BOOMER

IBM to GSK -- R2 = 0.94, p << 0.0001 (high correlation, highly significant

Fat fingered test

GME-GM -- R2 = 0.79. p << 0.0001 (high correlation, highly significant)

Looking at the R2 on low and high prices AFTER (Jan-Jun 2021):

MEME to MEME

GME to AMC : R2 = 0.83, p << 0.0001 (positive CORRELATION! Significant)

GME to KOSS : R2 = 0.77 , p << 0.0001 (positive CORRELATION, very significant)

MEME to Boomer

GME to IBM : R2 = 0.47, p << 0.0001 (positive CORRELATION, significant)

BOOMER to BOOMER

IBM to GSK : R2 = 0.62, p << 0.0001 (mid correlation, highly significant

Fat fingered test

GME to GM : R2 = 0.72. p << 0.0001 (high correlation, highly significant)

With a p value of p << 0.0001, GME is correlated with AMC (before and after, although switches direction), KOSS (before and after), NOKK (after), BBBY (before and after).

*Fat fingers*: Humorously, there is a correlation between GME and GM, obviously people are buying the wrong ticker, so I guess my 'random' choice of GM was actually not that random, as I made the same mistake! N.B. GME-GM's correlation is the outlier in the boomer stock basket, but I left it in anyway.

So what have we found?

After January the meme stocks (GME, AMC, KOSS, BBBY) became positively correlated if they weren't and the positive correlation increased. So these stocks started to move together and only GME and KOSS were moving together before. The IBM-GSK comparison shows two different boomer stocks from the control group, they come from different industries (GSK was affected more by covid than IBM) and we see a standard sort of movement, they're both positively correlated and generally following the wider economy.

And here's the data for all (average used is the median, error is standard error, 42 pairwise comparisons).

Average R2 of meme stock before : -0.42 (+/- 0.09)

Average R2 of meme stock after : 0.32 (+/- 0.05)

Average R2 of boomer stock before : 0.34 (+/- 0.08)

Average R2 of boomer stock after : 0.25 (+/- 0.05)

Difference in meme stocks: + 0.74, this is a huge change.

Difference in boomer stocks: -0.11, this is small, (but is it actually significantly different from no change?)

So from this and the graphs we can see before both boomer stocks were on average not particularly correlated with each other. On average, meme stocks were weakly anti-correlated. But after, meme stocks on average move to be more positively correlated.

Another hypothesis test! Yay! My favourite thing!

Are these populations significantly different? i.e. is the change of the r2 of these stonks before and after significant. (geek note, we use the mann whitney u test here, and I used the Hedges effect size test (thought you'd like that!)).

For the meme stocks:

Yes! The correlation after is GREATER with a p-value of 0.0079 (so statistically significant) and an effect size of 0.7 (a medium sized effect). So the average change in correlation between the meme stocks is a (statistically) significant increase.

For the boomer stocks:

No! The correlation after is LESS with a p-value of 0.54 (so NOT statistically significant) and an effect size of 0.1 (no real effect). So no real correlation either way, I,e, the relationship between the boomer stocks hasn't changed over the last year to date (cos the change I found is small above enough that it could be random noise). So the average change in correlation between the boomer stocks is (statistically) insignificant.

So what's the point?

The meme stocks have become significantly more correlated since January, and our control basket of boomer stocks have not. I will not speculate as to why this is the case. Again, Hank asked on here for this information, so I presume he has an idea. At the very least, it is nice to know that the similarity in the price action that everyone keeps posting is statistically significant. I only looked at daily data (where do you get the 5 minute data?) and I expect that the GME AMC correlations on this timescale would be fun to look at, and perhaps something of a smoking gun.

Final point, correlation does not imply causation. Although I've not made any comments as to why these correlations exist. All we've got here is two different scientific methods showing that there is similarity and correlation between certain meme stocks and that this increased since Jan.

The end unless you want to know the details:

Methods:

*Data pre-processing:*

We want to look at the patterns in the data and relative change rather than overall price movement, so we normalise the data to try and compare the datasets.

Data was taken a year to date from yesterday (6/3) and all stocks were normalised to the first day, so that the first day normalised prices was 100. The NASDEC ($IXIC) was also normalised the same way to the same day. To remove the background effect of the stock market's general movements, each dataseries was then divided by the normalised IXIC (day for day), and then renormalized back to 100 at the start of the data. The numbers get huge for GME due to it's huge price movement.

*Time horizon:*

The data for the whole year to date was compared but more interesting results were seen if we split the data into pre and post January 1st. Data was daily price data, including, high, low, open, close, adjusted close and volume).

*Correlation tests:*

After normalisation, datasets were tested for how correlated they were using the Pearson R2 measure and corresponding p-value using SKlearn.

*Clustering!*

We want to find similar patterns in the stock movements without assuming a. that we would see exact changes at the exact same time point and b, that the changes will be the same size. We cope with assumption a by using dynamic time warping distance metric (and b was the reason we did some of that normalisation). We use a machine learning clustering algorithm that can work with time-series data and compare the stonks using this dynamic time warping stuff. We test from 1 cluster up to 7 clusters using standard methods to determine which cluster is the best (inertia+elbow method and silhouette score), then we look at the clusters and see which stocks were put where.

(see <https://github.com/tslearn-team/tslearn> <https://towardsdatascience.com/how-to-apply-k-means-clustering-to-time-series-data-28d04a8f7da3>)

We do all this with each of the data dimensions (i.e. high, low, open, close, adjusted close and volume) and also with ALL OF THEM. And get pretty much the same results, btw, only LOW data is covered in this write up.

Appendix:

Comparing GME, AMC\
Before: Pearson r: -0.73 and p-value: 1.1e-25\
After: Pearson r: 0.83 and p-value: 7.6e-27

Comparing GME, KOSS\
Before: Pearson r: 0.55 and p-value: 2.8e-13\
After: Pearson r: 0.77 and p-value: 1.1e-21

Comparing GME, NAKD\
Before: Pearson r: -0.68 and p-value: 3.2e-21\
After: Pearson r: 0.043 and p-value: 0.66

Comparing GME, NOKK\
Before: Pearson r: -0.87 and p-value: 1e-47\
After: Pearson r: 0.39 and p-value: 3.9e-05

Comparing GME, BBBY\
Before: Pearson r: 0.8 and p-value: 1.9e-34\
After: Pearson r: 0.53 and p-value: 7.3e-09

Comparing GME, VIX\
Before: Pearson r: -0.42 and p-value: 1.5e-07\
After: Pearson r: -0.3 and p-value: 0.0022

Comparing IBM, AMZN\
Before r: 0.25 and p-value: 0.0024\
After Pearson r: 0.15 and p-value: 0.12

Comparing IBM, CVS\
Before r: 0.75 and p-value: 4.8e-28\
After Pearson r: 0.83 and p-value: 6.9e-28\
Comparing IBM, GSK\
Before r: 0.94 and p-value: 5.8e-72\
After Pearson r: 0.62 and p-value: 2.4e-12\
Comparing IBM, RDS\
Before r: 0.64 and p-value: 3.1e-18\
After Pearson r: 0.16 and p-value: 0.11\
Comparing IBM, WEN\
Before r: 0.82 and p-value: 1.2e-36\
After Pearson r: 0.85 and p-value: 5.8e-30\
Comparing IBM, GMBefore r: -0.6 and p-value: 9.9e-16\
After Pearson r: 0.39 and p-value: 4.6e-05

If people want, I can run the code to do this for the whole set of measurables and write it out to a .csv file?

Final disclaimer: I know fuck all about finance, but I know about data science and stats! Yay stats!
