Analysis deep dive: looking at historical SI% + FTD data and modelling share borrow fees since Jan
==================================================================================================

| Author       | Source       | 
| :-------------: |:-------------:|
|  [u/broccaaa](https://www.reddit.com/user/broccaaa/) | [Reddit](https://www.reddit.com/r/Superstonk/comments/mma7eh/analysis_deep_dive_looking_at_historical_si_ftd/) | 

---

[Serious DD 👨‍🔬🔬](https://www.reddit.com/r/Superstonk/search?q=flair_name%3A%22Serious%20DD%20%F0%9F%91%A8%E2%80%8D%F0%9F%94%AC%F0%9F%94%AC%22&restrict_sr=1)

TLDR: Figures are presented to show historical GME data and how it compares to other stocks. *Stock borrowing fees are currently way way lower than they should be*. This *suggests fuckery* on the data that we can see. I wonder what the shorts are really paying from other brokers?? Almost every way you look at GME it is the outlier of all outliers. I believe the shorts have only been digging themselves deeper and deeper since Jan. HODL!!!

🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀

In my previous two posts I described how fraudulent short sellers could setup a [naked short selling scam using the married put trade](https://www.reddit.com/r/GME/comments/mgj0j1/the_naked_shorting_scam_revealed_lending_of/) and extended this idea to [how the scam could be performed using SEC rules in 2021](https://www.reddit.com/r/GME/comments/mh6lnz/the_naked_shorting_scam_update_selling_nude_like/).

One of the predictions from those posts was that the low demand for legally obtained short shares could partly explain the low borrow fees in recent months. Another great DD was posted showing that [GME borrow fees were much lower than for other hard to borrow stocks](https://www.reddit.com/r/GME/comments/mgo0go/the_biggest_anomaly_in_gmes_data/).

In this post I conduct an extensive analysis of historical Short Interest (SI), short share availability and borrow fees in GME and other 'meme stocks', as well as 3 other hard-to-borrow stocks. The data is presented across a number of graphs and I'll try to explain the results in ape speak as best I can.

*Note: this is not financial advice. I am not a cat. I gathered some data, created some plots and made some interpretations. Any number of my interpretations could be flawed and wrong. Try to understand the data for yourself and make your own mind up.*

Introduction

When a trader wants to sell a share short via legitimate methods he finds a broker that has located shares available for loan and places an order to borrow them. Depending on the availability of shares, as well as other factors such implied risk in the trade, the broker will charge a borrowing fee for the duration of time that these shares are lent out.

Normally we would expect fees to go up as shares become more scarce but we've not seen this with GME. In recent weeks almost no shares have been available on [iborrowdesk.com](https://iborrowdesk.com/report/GME) but borrow fees remained around 1%. This disconnect has seemed highly unusual.

In this post I use data from multiple sources and statistical models to quantitatively show just how unusual the borrowing rates are for GME.

*Skip this next section unless you're interested in the details of the analysis*.

Data used in the analysis

-   Historical short share availability and borrow fees from <https://iborrowdesk.com/>

-   Historical fail to deliver (FTD) data [from the SEC website](https://www.sec.gov/data/foiadocsfailsdatahtm)

-   Historical short interest (SI) since April 2019 (unfortunately this is a pain to obtain)

-   Historical data on Shares Outstanding from <https://ycharts.com/companies/GME/shares_outstanding>

Methods summary

-   3 meme stocks (GME, AMC & BBBY) and 3 [hard to borrow stocks](https://www.reddit.com/r/GME/comments/mgo0go/the_biggest_anomaly_in_gmes_data/) (ZKIN & IMMP & APTO) selected

-   Figures plotted as part of exploratory analysis

-   Statistical model ([Mixed-Linear](https://www.statsmodels.org/stable/generated/statsmodels.regression.mixed_linear_model.MixedLM.html#statsmodels.regression.mixed_linear_model.MixedLM)) used to quantify relationships

-   Free float was estimated conservatively as outstanding shares minus shares held by insiders

Hypotheses (things I planned to test...)

Null Hypothesis 1: Short share borrow costs did not change from typical levels after the January peak

*Ape Hypothesis 1: Is cost to borrow share same now as in past?*

Null Hypothesis 2: Number of available shares has no relationship to borrow fees

*Ape Hypothesis 2: When no shares to borrow, is cost still cheap?*

Null Hypothesis 3: SI% and FTD numbers do not predict borrow fees

*Ape Hypothesis 3: Lots of shares already borrowed. Is cost still cheap?*

Historical SI%

[![r/Superstonk - Analysis deep dive: looking at historical SI% + FTD data and modelling share borrow fees since Jan](https://preview.redd.it/dcydvxozhsr61.png?width=3438&format=png&auto=webp&s=837e1835cd102b39104e1525ce2a87cbb37222d4)](https://preview.redd.it/dcydvxozhsr61.png?width=3438&format=png&auto=webp&s=837e1835cd102b39104e1525ce2a87cbb37222d4)

Short Interest (SI) percent of float since April 2019. 'Meme-stocks' (GME, AMC & BBBY) are in the upper plot and hard to borrow stocks (ZKIN & IMMP & APTO) in the lower plot. Notice the massive drop in reported SI% for meme-stocks between Jan 1st and mid Feb 2021.

GME SI% has been around or above 100% of float since the end of 2019. After being stable for over a year the reported GME SI% dropped from 110% in early Jan down to 35% in mid Feb 2021. Unfortunately SI% is reported bi-monthly so we do cannot see how it changes day by day, however the big drop off in SI% aligns with the 2 week period after the January peak 'mini-squeeze'.

Bed Bath & Beyond Inc. (BBBY) saw a similar drop off in reported SI% after the mini-squeeze. AMC Entertainment Holdings, Inc. (AMC) had a small drop off in SI% after Jan but as you can see AMC has never had an SI% much larger than 20% of float. The included hard-to-borrow stocks have SI% values less than 5%.

The GME SI% values historically, and even in recent weeks, dwarf the SI% of other stocks. GME really is the outlier among outliers.

[![r/Superstonk - Analysis deep dive: looking at historical SI% + FTD data and modelling share borrow fees since Jan](https://preview.redd.it/8romgm8pmsr61.png?width=3600&format=png&auto=webp&s=e7c4a9824e94f2819be993acaf54f0d503a81960)](https://preview.redd.it/8romgm8pmsr61.png?width=3600&format=png&auto=webp&s=e7c4a9824e94f2819be993acaf54f0d503a81960)

GME share prices and reported SI% in early 2021.

As SI% decreased in Feb the media driven narrative was that the shorts had covered in Jan. *But did they actually cover??*

Fail to Delivers (FTDs)

[![r/Superstonk - Analysis deep dive: looking at historical SI% + FTD data and modelling share borrow fees since Jan](https://preview.redd.it/3uxoutg8nsr61.png?width=3288&format=png&auto=webp&s=0cead25e86699ca085748f86b9a044a5be622c5c)](https://preview.redd.it/3uxoutg8nsr61.png?width=3288&format=png&auto=webp&s=0cead25e86699ca085748f86b9a044a5be622c5c)

FTDs as percent of float from Aug 2020. 'Meme-stocks' (GME, AMC & BBBY) are in the upper plot and hard to borrow stocks (ZKIN & IMMP & APTO) in the lower plot.

FTDs for GME regularly spiked to more than 3% of float throughout 2020. After the Jan mini-squeeze the seem to have magically disappeared, aside from a small blip at the end of Feb. Some great DD by [u/dejf2](https://www.reddit.com/u/dejf2/) shows that much of the [SI% and FTDs is hidden in the options using deep in the money calls](https://www.reddit.com/r/GME/comments/mhv22h/the_si_is_fake_i_found_44000000_million_shorts/).

Short share availability and borrowing fees

[![r/Superstonk - Analysis deep dive: looking at historical SI% + FTD data and modelling share borrow fees since Jan](https://preview.redd.it/tqa9u7osqsr61.png?width=3438&format=png&auto=webp&s=213e2170d87cf1def46a3a1a5a7fcf9b060fb20e)](https://preview.redd.it/tqa9u7osqsr61.png?width=3438&format=png&auto=webp&s=213e2170d87cf1def46a3a1a5a7fcf9b060fb20e)

Short share borrowing fees from https://iborrowdesk.com/report/GME since Aug 2020. Since the end of January GME borrowing fees dropped more than 90%.

After the Jan mini-squeeze GME borrowing fees dropped from a peak of 80% down to around 1%. Throughout much of 2020 borrow fees were rarely less than 20%.

[![r/Superstonk - Analysis deep dive: looking at historical SI% + FTD data and modelling share borrow fees since Jan](https://preview.redd.it/hm0k0qwhrsr61.png?width=1800&format=png&auto=webp&s=b2bb58099545f7dc56b9451da9f03f8b9a710587)](https://preview.redd.it/hm0k0qwhrsr61.png?width=1800&format=png&auto=webp&s=b2bb58099545f7dc56b9451da9f03f8b9a710587)

Short share borrowing fees before and after the Jan mini-squeeze for 'meme-stocks' (GME, AMC & BBBY) and hard to borrow stocks (ZKIN & IMMP & APTO).

Here we see that borrow costs for meme-stocks, particularly GME and AMC, are much lower than usual since Jan. Other hard to borrow stocks have either seen no change in borrow fees or a slight increase.

[![r/Superstonk - Analysis deep dive: looking at historical SI% + FTD data and modelling share borrow fees since Jan](https://preview.redd.it/w8w4xan5ssr61.png?width=4776&format=png&auto=webp&s=3b95ca6e59489abdb1e9d2c76b506a517583c0b3)](https://preview.redd.it/w8w4xan5ssr61.png?width=4776&format=png&auto=webp&s=3b95ca6e59489abdb1e9d2c76b506a517583c0b3)

Short share borrowing fees by short share availability, before and after the Jan mini-squeeze. 'Meme-stocks' (GME, AMC & BBBY) are in the upper row and hard to borrow stocks (ZKIN & IMMP & APTO) in the lower row.

In this plot we clearly see that borrow costs for GME and AMC are massively reduced since Jan compared usual rates. As an example, borrowing GME shares when only 0.5% of the float is available would've cost approx. 20% before the Jan mini-squeeze but now costs only 1.4%.

Modelling GME borrow fees

Here I gathered all the data on FTDs, SI% and short share availability together to build a statistical model. I wanted to test which parameters usually predict short share borrowing fees and to quantify just how different the situation has been since January.

I used an [MLM](https://www.statsmodels.org/stable/generated/statsmodels.regression.mixed_linear_model.MixedLM.html#statsmodels.regression.mixed_linear_model.MixedLM) with random effects of ticker symbol. I won't get into all the boring details of the model but leave a comment if you have questions.

Here are the results...

[![r/Superstonk - Analysis deep dive: looking at historical SI% + FTD data and modelling share borrow fees since Jan](https://preview.redd.it/dpexbhmztsr61.png?width=1536&format=png&auto=webp&s=6f40e74d896188a4e0245ef2d9f24a902e5a81fd)](https://preview.redd.it/dpexbhmztsr61.png?width=1536&format=png&auto=webp&s=6f40e74d896188a4e0245ef2d9f24a902e5a81fd)

Predicting short share borrowing fees before and after Jan mini-squeeze using SI, FTD and short share availability data.

This model shows that *borrowing fees for meme-stocks after January is significantly lower than previous rates* (z-score = -24.749, p-val = 1E-135). This result is so strong you would have more chance winning the lottery millions and millions of times than to see this difference in borrow fees by chance!!!

The model also predicts the following *in normal* share borrowing situations:

1.  Meme-stock borrow fees behaved just like other stocks before the mini-squeeze in Jan (p-val = 0.48)

2.  Fewer available shares as a percent of float predicts increased borrow fees (p-val < 0.001)

3.  Increased FTD numbers as percent of float predicts increased borrow fees (p-val < 0.001)

4.  Increased SI% numbers as percent of float predicts increased borrow fees (p-val < 0.001)

Meme-stocks had borrow fees in line with other stocks but something massive happened to fees after Jan. The change was so big that current borrow fees are disconnected to their usual predictors. What exactly is driving this we can only speculate but *I would not rule out fuckery*.

Conclusion

After the January mini-squeeze we saw decreasing numbers in FTDs, SI% and stock borrowing fees. Stock borrow fees are reported to be so much lower than usual it's hard to understand the significance of the result.

To find a result as significance as this randomly you would have a 1 in 10134 chance. That is 1 in 10,000,...000 with 134 zeros!!!

I believe one of two things is happening:

1.  Interactive Brokers are lying about their borrow fees to scare retail away from GME and other meme stocks. [Interactive Brokers stopped trading in January](https://www.cnbc.com/2021/01/28/interactive-brokers-restricted-gamestop-trading-to-protect-the-market-says-chairman-peterffy.html) and revealed that they might've been completely fucked if prices had kept rising.

2.  [Mass naked short selling](https://www.reddit.com/r/GME/comments/mgj0j1/the_naked_shorting_scam_revealed_lending_of/) and [covering of FTDs using hidden options](https://www.reddit.com/r/GME/comments/mhv22h/the_si_is_fake_i_found_44000000_million_shorts/) has reduced the demand in located shares to borrow so much it's crashed the borrow fees. If New DTCC rules are making it harder to hide FTDs then borrow fees might start to increase again.

I believe that the short funds are so fucked that they are doing anything to hide their tracks and make retail go away. Manipulating data. Paying off media. Digging themselves deeper and deeper.

In my next post I want to look into historical options data to see exactly when the hidden shorts were setup and when we might moon.

🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀
