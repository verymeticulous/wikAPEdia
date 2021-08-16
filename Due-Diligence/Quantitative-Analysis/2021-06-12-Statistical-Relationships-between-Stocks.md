An update on relationships between stocks - STATISTICS ROCKS! - Brought to you by the SuperstonkQuants 🦍🥼🔬🚀
===============================================================================================================

| Author       | Source       | 
| :-------------: |:-------------:|
|  [u/xpurplexamyx](https://www.reddit.com/user/xpurplexamyx/) | [Reddit](https://www.reddit.com/r/Superstonk/comments/nym1ua/an_update_on_relationships_between_stocks/) | 

---

[DD 👨‍🔬](https://www.reddit.com/r/Superstonk/search?q=flair_name%3A%22DD%20%F0%9F%91%A8%E2%80%8D%F0%9F%94%AC%22&restrict_sr=1)

Edit: Some folks have asked for a TA;DR. It's sorta hard to distill this post down into a mere sentence, but I'll try to channel my smooth brain:

TA;DR - A few things are going on in this post; the whole thing is worth reading, but distilled down:

1.  A lot of data science to help wrinkled apes who are attempting to correlate things not fall into the pit of mis-correlation of time series data.

2.  A pretty awesome tool for quickly checking correlation of two stocks over a given time period!

3.  A peer-reviewed confirmation of correlation between GME, AMC, BBBY, KOSS, NAKD, NOK, and VIX."Before we were only looking at the graphs and hand wavingly saying "eh, close enough". That is a far cry from showing a correlation." - [u/half_dane](https://www.reddit.com/u/half_dane/)

Also: CORRELATION != CAUSATION. Nothing in this post attempts to speak to or address the "why".

Edit: Please also check out [u/orangecatmasterrace](https://www.reddit.com/u/orangecatmasterrace/)'s RRP/GME analysis here, which makes use of the tooling this thread talks about: <https://www.reddit.com/r/DDintoGME/comments/nype4f/is_gmes_price_related_to_the_reverse_repo_rate_in/>

Preface:

I ([u/xpurplexamyx](https://www.reddit.com/u/xpurplexamyx/)) am posting this on behalf of one of the [SuperstonkQuants](https://www.superstonkquant.org/) wrinkle brains, [u/braaaaiiinnnsss](https://www.reddit.com/u/braaaaiiinnnsss/), who lurks reddit and as a result does not have sufficient karma to post directly.

Though they call me out in their post as having contributed, I feel that is an overstatement. Most if not all of the interactions I have with the incredible analysts who have joined the dark basement that is the SuperstonkQuants [go along these lines.](https://www.youtube.com/watch?v=SmHl7hKlVj4) I am good at pulling data together for them to sink their collective teeth into though, so I do what I can to support their quest to [generate graphs.](https://www.youtube.com/watch?v=sIlNIVXpIns)

This all to *provide a disclaimer* that while I will act as a conduit for answers to any questions you may ask in the comments, I probably don't know the answer myself and am learning along with the rest of you. If a mod passes by and fancies approving [u/braaaaiiinnnsss](https://www.reddit.com/u/braaaaiiinnnsss/), that would be appreciated! :)

---------------

Hello from SuperstonkQuants (the subreddit's quant group that spawned out of a request for analysis from [u/HomeDepotHank69](https://www.reddit.com/u/HomeDepotHank69/))! I wanted to let you know that there are some seriously amazing things going on there, and we all look forward to sharing them with you!

I am on the low-level analysis side, and wanted to bring you all up to speed on how to answer questions like: *Is X related to Y?* This is one of the most common types of questions we receive, so that is what I have been focused on. It turns out, this is more complicated to answer than you might think. If you google how to see if two stocks are related, even Yahoo Finance will tell you to run a correlation.Correlations are misleading due to the type of data we are working with.

For this reason, I wanted to put a post together, so those of you who are answering such questions on your own will have the tools to do so. Statistics answers the question, *"how confident are you in the effect"*? This is a big deal when you are making claims about worldwide illegal activity, so we want to make the tools available to all apes.

This is not only my work, but that of many other SuperstonkQuants contributors - particularly an extremely stubborn and skeptical analyst who will forever remain in the shadows while demanding *more proof*; [u/orangecatmasterrace](https://www.reddit.com/u/orangecatmasterrace/); [u/xpurplexamyx](https://www.reddit.com/u/xpurplexamyx/); and Hydra - as well as my wife.

Quick qualifications: I am a professor and teach statistics to undergrads. My wife is a PhD statistician, and has way more stats wrinkles than I do - her input has been invaluable.

Side note: I am extremely passionate about education. One of the primary ways the hella rich have stayed in power is to make sure the masses are not educated. *The less educated we are, the easier we are to be manipulated*. Education funding is abysmal in the US, I hope this will change in the future. Superstonk is an AMAZING example of what happens when a large group of people become educated. I have learned a metric shed ton about the financial world from this sub, and I hope to return the favor in this post. I am not approved to post, but I am [u/braaaaiiinnnsss](https://www.reddit.com/u/braaaaiiinnnsss/). Feel free to message me if you have any questions! I would also be happy to do some more educational posts in the future if there is interest.

Now, ON TO STATISTICS...

Let's look at correlations first (basics to why it doesn't work for us)

*This in no way means that any correlation findings posted previously are wrong! Instead, I am suggesting we re-evaluate them to make sure the findings are valid.*

Whenever I run statistics, I want to make sure that they work. I do this by seeing if they show a relationship when they should, and if they show no relationship when there is none.

A correlation is used when you have two continuous variables (like two stocks), and you want to see if they are related. The standard correlation combines two things: how well the two variables move together (covariance) and how spread out the data is (variance). THIS IS AMAZING, correlations are seriously clever. However, every statistical analysis comes with assumptions (the fine print) that even peer reviewed publications do not pay attention to.

The most common correlation is a [Pearson's correlation coefficient](https://en.wikipedia.org/wiki/Pearson_correlation_coefficient) (r). A Pearson's r is a value between -1 and 1, the absolute value of which reflects the strength of the relationship, and the sign indicates the direction (positive -- as one variable increases, the other increases; negative -- as one variable increases, the other decreases). From your r and the size of the dataset, you can get a p-value that is the probability that you found the effect due to chance (sort of). If p = 0.05, that means that there is a 5% chance that there is no effect, even though your stats show one.

A few notes before we look at numbers:

1.  A more accurate explanation of a p-value is the following: if we were to run the same test over and over on different samples from the same population, p is the probability of finding an effect due to chance.

2.  There is a completely arbitrary cutoff of p=0.05 to indicate significance. That is, if p <= 0.05 the effect is significant, if p > 0.05, it is not. I don't necessarily agree with this, but it will be used as a standard for now.

3.  Although I will be using a Pearson's r as an example, a [Spearman's r](https://en.wikipedia.org/wiki/Spearman%27s_rank_correlation_coefficient) is more appropriate for stock data. I have tested Spearman's in the same way and found similar results.

The correlation between GME and AMC is (r = 0.71, p = 2.2 e -16). That's a p value with more zeros than I even thought possible! Now let's look at something that should not be correlated, GME and SPY (r = 0.78, p = 2.2 e -16). *They are basically the same*. They are so similar I had to continually check my code. This is certainly not true for all stocks, I just found it to be a good example.

*Why might this be?*

At the bottom of this linked page, there is a nice list of the assumptions along with an explanations: <https://statistics.laerd.com/statistical-guides/pearson-correlation-coefficient-statistical-guide.php>

The biggest issue with stock data is it breaks the independence assumption (assumption 3). The independence assumption basically says that each observation within a variable should be independent of other observations in the same variable.

So if I were to look at the relationship between size of ape 🦍 and number of bananas 🍌eaten daily, we would likely see a positive correlation:

🐒= 🍌🍌

🦍= 🍌🍌🍌🍌🍌

🦧= 🍌🍌🍌🍌🍌🍌🍌🍌🍌🍌🍌

Here, the number of bananas eaten by one ape 🦍*does not depend* on the number of bananas 🍌 another ape 🦍 has eaten (assuming an all-inclusive banana buffet 🍌🍌🍌🍌🍌🍌🍌🍌🍌🍌🍌🍌).

In stock data, this is not true. The opening price on one day depends on the price in a previous day. This type of data is called *time series data*, which just means it changes over time. One way statisticians talk about this is called autocorrelation, which is simply that observations in a variable are correlated with others in that variable (it is correlated with itself).

[DISCLAIMER: I am not an expert in time series data. I have been doing a lot of research lately to try to catch up. If anyone has a better method than the one below, please let me know!]

Removing autocorrelation from the data:

There are a few ways to deal with this, but we ultimately decided to remove the autocorrelation from the data and do our statistics on the result. The methods used are not developed by us. They were found from an excellent graduate student statistics class at Penn State (<https://online.stat.psu.edu/stat510/lesson/1>) and from this online text book by Rob J Hyndman and George Athanasopoulos (<https://otexts.com/fpp2/index.html>).

We tried A LOT of different methods (filtering data through ARIMA models, transforming data using various functions, etc). The resulting data from many of the methods could only be used specifically for correlations, and there is a lot of other tests we want to do (see future directions below). We recently decided on a simple transformation that does a great job (though not perfect), called differencing. The result will sometimes have small autocorrelation left in the data, but it is simple, clean, and hopefully I will convince you below that it works for our purposes.

Differencing is typically used to stabilize the mean of a time series, so you can focus on fluctuations. It is a transform where you subtract the previous observation from the current observation for all data. So difference(t) = observation(t) -- observation(t-1). There is a lot more to discuss out this, and I would be happy to answer questions, but here I want to get to why I think it works (this post is long enough as is).

After differencing the data, I used a cross-correlation to find out if X and Y were related. Cross-correlation is nice because the data does not have to line up perfectly to find a relationship. For example, if you think a large change in AMC will precede GME, the cross correlation will find that relationship for you.

That was a lot of writing, thank you if you stuck around until now!

Proof of concept

Let's look at some graphs. On all graphs below, the left panel shows price data, and the right shows the cross-correlation results. The results are shown as a bar graph with lag on the x-axis (days in this case) and Pearson's correlation coefficient on the y-axis. If a bar crosses the horizontal blue line, it is significant at the p=0.05 level.

To help with interpreting the data, I messed around with the mini squeeze from GME in January. The following is correlating that data with itself with different lags/transformations, which means that the r = 1 in every result.

[![r/Superstonk - An update on relationships between stocks - STATISTICS ROCKS! - Brought to you by the SuperstonkQuants 🦍🥼🔬🚀](https://preview.redd.it/mq8x1fuovx471.png?width=3024&format=png&auto=webp&s=4a10bc8965c5e261cd6522b97b4ee0935c84cb09)](https://preview.redd.it/mq8x1fuovx471.png?width=3024&format=png&auto=webp&s=4a10bc8965c5e261cd6522b97b4ee0935c84cb09)

Now we can see how to interpret the results, but how do we know if it is actually working? The above examples show that the method can detect a significant result, so let's look at the relationship between GME and SPY again, just like we did in the beginning.

[![r/Superstonk - An update on relationships between stocks - STATISTICS ROCKS! - Brought to you by the SuperstonkQuants 🦍🥼🔬🚀](https://preview.redd.it/hgg0q2tpvx471.png?width=2140&format=png&auto=webp&s=1929d7bdcfaf5755e9fc022a7321894796f5c420)](https://preview.redd.it/hgg0q2tpvx471.png?width=2140&format=png&auto=webp&s=1929d7bdcfaf5755e9fc022a7321894796f5c420)

I WAS SO HAPPY WHEN I SAW THIS. I tested a bunch of other stocks (and simulated data) that shouldn't be related, so now I feel confident that the method works (if you want more information, please let me know). To finish this off, I want to show results from some real data, which is never as clean as my examples above.

[![r/Superstonk - An update on relationships between stocks - STATISTICS ROCKS! - Brought to you by the SuperstonkQuants 🦍🥼🔬🚀](https://preview.redd.it/cicfdenqvx471.png?width=3032&format=png&auto=webp&s=200877f436463a02b344f0f1dd5aa8011279b80c)](https://preview.redd.it/cicfdenqvx471.png?width=3032&format=png&auto=webp&s=200877f436463a02b344f0f1dd5aa8011279b80c)

Replication of Q1: Comparison of GME, AMC, BBBY, KOSS, NAKD, NOK, and VIX

*Ed note:* [*Q1 bitbucket repo is here*](https://github.com/SuperstonkQuants/q1_correlations)

While it is easy to get excited about results (I get overly excited), always remember correlation does not equal causation, so we may have mediators and moderators that are contributing to the effect.

I am going to stay in my lane and not speculate what this all *means*, rather this is just an example with real data. All have significance at lag 0, showing that the two stocks are related with no shift. One result I would like to talk about is GME vs. NOK. Visually, it does not look as though they are correlated, yet the results say it is. I was worried that this was an issue with the method, but if I zoom in on NOK we see a nice bump in opening price at the same time as the spike in GME opening price. *This is why it is so important to do the stats*. Graphical representations are amazing, I've literally drooled over some of the graphs you all have posted, but it is also worth seeing what the stats tell us so we don't miss anything (or make speculations about relationships that do not exist).

IMPORTANT DISCLAIMER: When you run a statistical test over and over on data, the chances that you see an effect do to chance increases. For example, let's say all effects have a p=0.05. If we run 1000 tests, then 50 of those tests will show something that isn't real. A lot of questions we've received ask about more than two stocks, so we will deal with the issue soon (discussed below).

Future directions

Now that we have a good method for correlations, there is a lot we can do! First, we want to compare more than two stocks at once. Since we removed the autocorrelation (ish) from the data, we can use standard approaches like multiple regression to do that. After that we have a few things going on:

-   As I speak, other quant apes are running rolling correlations with the data (see when stocks become related)

-   I would like to get a path analysis script together, which will give us more information on how extensive the market manipulation is.

-   We want to use this method for crypto data (which is even messier than stock data) as many of you have suggested.

-   WHATEVER ELSE YOU COME UP WITH

Our strength comes from the hive mind, so I hope many of you can use these tools to ask your own questions. The code will be [available on the github](https://github.com/SuperstonkQuants/statistics_rocks), so go have a look (and also check out all the other amazing stuff there).

The more we know, the better prepared we will be to make sure the world is a better place. I love all you sexy, hairy apes <3 and a shoutout to the mods who are doing an AMAZING job.
