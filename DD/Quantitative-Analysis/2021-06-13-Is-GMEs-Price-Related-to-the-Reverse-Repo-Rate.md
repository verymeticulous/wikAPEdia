Is GME's price related to the Reverse Repo Rate in some way? - Lets find out! - Brought to you by the Superstonk Quants 🦍👨‍💻🧐🚀
===================================================================================================================================

| Author       | Source       | 
| :-------------: |:-------------:|
|  [u/orangecatmasterrace](https://www.reddit.com/user/orangecatmasterrace/) | [Reddit](https://www.reddit.com/r/DDintoGME/comments/nype4f/is_gmes_price_related_to_the_reverse_repo_rate_in/) | 

---

[𝘜𝘯𝘷𝘦𝘳𝘪𝘧𝘪𝘦𝘥 𝘋𝘋](https://www.reddit.com/r/DDintoGME/search?q=flair_name%3A%22%F0%9D%98%9C%F0%9D%98%AF%F0%9D%98%B7%F0%9D%98%A6%F0%9D%98%B3%F0%9D%98%AA%F0%9D%98%A7%F0%9D%98%AA%F0%9D%98%A6%F0%9D%98%A5%20%F0%9D%98%8B%F0%9D%98%8B%22&restrict_sr=1)

Hi everyone! I'm [u/orangecatmasterrace](https://www.reddit.com/u/orangecatmasterrace/) - a longtime reddit lurker, but I've been involved in GME since January. I'm posting here as I don't yet have enough karma to post directly to [r/Superstonk](https://www.reddit.com/r/Superstonk/). I wanted to share an analysis that I, along with the incredibly talented apes at [Superstonk Quants](https://www.superstonkquant.org/) pulled together over the past couple days. We're the group that initially banded together to aid [u/HomeDepotHank69](https://www.reddit.com/u/HomeDepotHank69/) in his [quest for data-driven DD](https://www.reddit.com/r/Superstonk/comments/nu9qq9/hanks_big_bang_quant_apes_glitch_the_simulation/?utm_source=share&utm_medium=web2x&context=3).

The Superstonk Quants want to ensure that data-driven insights around GME and the surrounding market are arrived at correctly, with the correct methodology, in conjunction with an internal peer review process. We're hoping that this analysis will be a small step towards providing this incredible community with accurate data behind what is going on right now. We've got many more irons in the fire right now, which we're super excited to share soon! 🚀

Brief background: I'm a data analyst by trade, with a background in psychology, data science, and behavioral analysis. I work with data 5/7 days of the week (now more like 7/7 since joining the Quants) but financial/stock market data is certainly a new flavor for me. This work has already allowed me to learn a lot and stretch my data legs a lot further than I thought!

Without any further ado, lets jump into this, shall we? 😏

This analysis was brought about after we saw a post that got some traction recently, seeking to derive [correlation between the Reverse Repo rates and the share price of GME](https://www.reddit.com/r/Superstonk/comments/nx2mg4/statistical_proof_that_hedgies_r_fuk_and_the_repo/).

While the idea behind this analysis was sound, and the hypotheses that [u/bobsmith808](https://www.reddit.com/u/bobsmith808/) developed were an interesting starter to the analysis, unfortunately, the methodology behind the comparisons and the conclusions were not completely accurate. (Its ok Bob! You're still a true ape and we love you!)

In order to properly determine the answer to the question, "Is GME's price related to the Reverse Repo Rate in some way?" we needed to approach this with a methodology that controls for some of the tricky nuances that come with working on time series data.

My partner in crime, the incredibly bewrinkled statistics sensei [u/braaaaiiinnnsss](https://www.reddit.com/u/braaaaiiinnnsss/), did an amazing job introducing and explaining many of the factors we had to take into consideration when conducting this analysis in his [recent DD](https://www.reddit.com/r/Superstonk/comments/nym1ua/an_update_on_relationships_between_stocks/).

I'd strongly recommend reading through his post before continuing, as the concepts that I'll be covering build directly off of those established there. I've got to give a huge shout out to our resident golden (data) retriever [u/xpurplexamyx](https://www.reddit.com/u/xpurplexamyx/) and an unyieldingly anonymous Wendy's-fueled analyst for their input and perspective on solving this problem; this was absolutely a team effort! 🐒🦍🦧

Ok! So now that you're all a tad bit wrinklier about working with time series data, I want to run you through what I found through the course of my analysis.

First, I loaded up the GME OHLC and Reverse Repo data from 1/1/2020 through 6/10/2021, and wanted to make sure I could reproduce the scatter plots that [u/bobsmith808](https://www.reddit.com/u/bobsmith808/) pulled together in his analysis in order to validate I was using the same data :) Reproducibility is important here!

I plotted the GME Open price against the Reverse Repo Daily Totals, and arrived at a very similar looking dinosaur(?)-shaped plot.

[![r/DDintoGME - Is GME's price related to the Reverse Repo Rate in some way? - Lets find out! - Brought to you by the Superstonk Quants 🦍👨‍💻🧐🚀](https://preview.redd.it/9qy00vbdry471.png?width=763&format=png&auto=webp&s=ed89a492727673f4634b9084ce464fbde8fce805)](https://preview.redd.it/9qy00vbdry471.png?width=763&format=png&auto=webp&s=ed89a492727673f4634b9084ce464fbde8fce805)

🦕 says rawr

Ok, so now that we know we're looking at the same thing, lets start to use the methodology that [u/braaaaiiinnnsss](https://www.reddit.com/u/braaaaiiinnnsss/) shared in his post to determine if a relationship exists here.

I applied an [ARIMA model](https://www.rdocumentation.org/packages/forecast/versions/8.15/topics/Arima) to the GME Open price to see if there was any reasonable lag in GME's price that could have a relationship with the Reverse Repo. Basically, what I wanted to look for here was if GME's Price changing (both direction and magnitude) could be related to the Reverse Repo at some leading or lagging interval. The ARIMA model gives me values called residuals, which are the differences between each of the daily GME Open prices. Running this model controls for autocorrelation and allows us to run a CCF (cross-correlation) between the model's residuals and the Reverse Repo Daily Totals.

After running the CCF, here's what we get:

[![r/DDintoGME - Is GME's price related to the Reverse Repo Rate in some way? - Lets find out! - Brought to you by the Superstonk Quants 🦍👨‍💻🧐🚀](https://preview.redd.it/7ndp686try471.png?width=735&format=png&auto=webp&s=b719c9feb750cc2ecf8fa9fb8c12a6e109bde73a)](https://preview.redd.it/7ndp686try471.png?width=735&format=png&auto=webp&s=b719c9feb750cc2ecf8fa9fb8c12a6e109bde73a)

The lines Mason! What do they mean?!

These might look like a whole bunch of useless lines, but these lines tell us...*things!* What we're looking at here is how strong of a relationship the changes in GME's price has with the Reverse Repo Daily Totals, at various daily offsets (lags), both forward and backward.

BUT -- In order for a statistically significant relationship to exist, we'd have to see one of these lines extending past the blue dotted line. That's our threshold for significance at the p=0.05 level.

Since none of the vertical lines crossed the blue dotted lines, we can initially assume that these 2 variables are not correlated with each other, at least at any level of statistical significance.

BUT LET'S NOT THROW IN THE TOWEL YET!

I'm not gonna let 1 measly chart tell me that nothing's there!

Perhaps there's another way we could investigate this relationship?

Well, I'm glad you asked, because there absolutely is!

Now, before I go into what this methodology is, I have to preface: I'm a huge data visualization guy. It's probably my favorite aspect of working with data. I have to be able to *see the data* to really, fully understand it most of the time. So I wanted to find a methodology that was able to satisfy both the statistical *and* the visual aspect of this question.

After spending an unhealthy amount of time scouring through scholarly papers and too many Google results telling me to just "run a correlation" I stumbled on the *very cool* approach of Rolling Correlation.

Rolling Correlation is an approach to analyzing time series data that uncovers specifically WHEN and HOW MUCH two series are related to each other in time, at dynamic time windows. Rather than taking a static, overall calculation of correlation between two series over the entire span of time, rolling correlation brings the aspect of TIME into center stage -- allowing you to see *visually* when the two series might be related to each other and when they're not, on our favorite correlation scale of -1 to 1: -1 being perfectly negatively correlated, 1 being perfectly positively correlated, and 0 being no correlation.

Now before we go comparing every ticker on the planet to each other, there's another important wrinkle that we need to develop.

Remember back to the wise words of Papa [u/braaaaiiinnnsss](https://www.reddit.com/u/braaaaiiinnnsss/): *"The biggest issue with stock data is it breaks the independence assumption."* That's fancy statistical ape speak for "every single data point in your series is related to the ones before and after it."

We can't just chuck raw price data into a rolling correlation and walk away with results; we need to remove the autocorrelation from the data in order to have a meaningful result. We're going to use the method that [u/braaaaiiinnnsss](https://www.reddit.com/u/braaaaiiinnnsss/) -sama introduced of differencing here again.

So I then calculated the differences for the daily GME Open prices and the Reverse Repo Totals. These differenced values are what we're going to compare, not the raw price values.

Next, within the rolling correlation function, we need to supply a "window" for the span of time that we want our correlations to span. This value is extremely important, as using too small of a value will result in an wild, noisy output that doesn't make a lot of sense, and too large of a value will result in a calculation that isn't sensitive enough to changes within the data. The general rule of thumb with time series data is that you need *at minimum* 25 observations in order to get a reliable correlation. After a little bit of trial and error, I settled on using a 60-day window. This gave a nice balance of interpretability in the results, and it wasn't too over or under sensitive in changes with the data.

After running the rolling correlation, here's what we get:

[![r/DDintoGME - Is GME's price related to the Reverse Repo Rate in some way? - Lets find out! - Brought to you by the Superstonk Quants 🦍👨‍💻🧐🚀](https://preview.redd.it/poiviqtpty471.png?width=1077&format=png&auto=webp&s=f27eb0fbdce33f99d3f48e98e22209f12a17526f)](https://preview.redd.it/poiviqtpty471.png?width=1077&format=png&auto=webp&s=f27eb0fbdce33f99d3f48e98e22209f12a17526f)

Well that's certainly *something!*

This plot shows the degree at which the two differenced variables are related to each other, at each of the 60-day rolling windows over time. each point along the line represents a window of 60 days, advancing through time, left to right. The closer the correlation line is to the bright red or blue lines at -1 and 1, the stronger the relationship between the variables, either negative or positive. The closer to the light blue center line, the weaker the relationship.

Since the points are between 0.5 and -0.5, mostly along the center line at 0, we can assume that the GME Open price and the RRP Daily Totals are generally not strongly correlated with each other, *particularly so* after the January run-up.

If a correlation actually existed there, we'd see those black dots much closer to either of the red lines, and it might look something like.... oh, I don't know.... the comparison between GME and AMC? 😏

[![r/DDintoGME - Is GME's price related to the Reverse Repo Rate in some way? - Lets find out! - Brought to you by the Superstonk Quants 🦍👨‍💻🧐🚀](https://preview.redd.it/qefqa015uy471.png?width=1198&format=png&auto=webp&s=a43a2b3dbf2e9ba8bec872c43416246b671005fa)](https://preview.redd.it/qefqa015uy471.png?width=1198&format=png&auto=webp&s=a43a2b3dbf2e9ba8bec872c43416246b671005fa)

.98 is a VERY strong correlation during that window 😤

...but that's the subject of my next DD for another day 😏🚀

Anyways! I didn't want to stop with just *one comparison.*

I wanted to see if potentially the number of Reverse Repo Counterparties might have some kind of relationship, even if the Totals themselves didn't. So I ran a similar analysis with differenced values for GME's Open again along with the Counterparties, and here's the result:

[![r/DDintoGME - Is GME's price related to the Reverse Repo Rate in some way? - Lets find out! - Brought to you by the Superstonk Quants 🦍👨‍💻🧐🚀](https://preview.redd.it/qrt9rp2vuy471.png?width=1076&format=png&auto=webp&s=ddb96385a984b31d33c9a42a953b53023cd79e25)](https://preview.redd.it/qrt9rp2vuy471.png?width=1076&format=png&auto=webp&s=ddb96385a984b31d33c9a42a953b53023cd79e25)

Nope, nothing significant here either.

BUT I WASN'T DONE YET.

I ran a third analysis on the amount of Reverse Repo Totals per Counterparty against GME's Open price.

Third time's the charm?

[![r/DDintoGME - Is GME's price related to the Reverse Repo Rate in some way? - Lets find out! - Brought to you by the Superstonk Quants 🦍👨‍💻🧐🚀](https://preview.redd.it/mmw3xfc1vy471.png?width=1076&format=png&auto=webp&s=707dd17844502824c53e778654e9f1bacbec7c17)](https://preview.redd.it/mmw3xfc1vy471.png?width=1076&format=png&auto=webp&s=707dd17844502824c53e778654e9f1bacbec7c17)

Nope, still no significant relationship to speak of.

I feel pretty confident based on this approach that no statistically significant relationship exists, or has ever really existed between GME's price and the Reverse Repo.

But worry not fellow apes! Just because the Reverse Repo isn't statistically related to GME's price movements doesn't mean the squeeze ain't gonna squoze!

The exciting part about these analyses is that they've been a catalyst for the Superstonk Quants to develop a methodology for running these comparisons. We're planning to share more results of this approach very soon!

In the meantime, if you'd like to check out the code along with a brief summary of the analysis, we've hosted the R markdown on the Superstonk Quants website [here](https://rrpgme.superstonkquant.org/)!

Additionally, the full R code is available on our [Github repo](https://github.com/SuperstonkQuants/reddit_RRPGME_corr)!

If there's one thing that I've taken away from doing this work so far, its that:

APES ARE TRULY STRONGER TOGETHER 🐒🦍🦧💎🙌🚀🚀🚀🌝

BUCKLE UP.
