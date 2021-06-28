Hank's Big Bang: Quant Apes Glitch the Simulation
=================================================

| Author       | Source       | 
| :-------------: |:-------------:|
|  [u/HomeDepotHank69](https://www.reddit.com/user/HomeDepotHank69/) | [Reddit](https://www.reddit.com/r/Superstonk/comments/nu9qq9/hanks_big_bang_quant_apes_glitch_the_simulation/) | 

---

[DD 👨‍🔬](https://www.reddit.com/r/Superstonk/search?q=flair_name%3A%22DD%20%F0%9F%91%A8%E2%80%8D%F0%9F%94%AC%22&restrict_sr=1)

********** I am not a financial advisor, this is not financial advice **********

Edit: Credit for the correlation tables to [u/phalanxhydra](https://www.reddit.com/u/phalanxhydra/)

Edit 2: I am retarded. It's [u/Ivorypetal](https://www.reddit.com/u/Ivorypetal/).

Introduction

Apes, because of the sheer amount of information in this post and because I wanted to get it to you at the beginning of this week because of earnings and the meeting, this post will not have the usual funny intro and memes.

Usually, my DDs are done completely by me with maybe some inspiration from a few apes or a section/link from an ape or two. This one is not that. This DD is an orgy. Apes, I have gathered an army. A fucking army of quant apes. They have been gracious enough to team up and answer the questions that I posed in my previous post and..... I am astonished at what they did. Seriously, I didn't expect this in my wildest dreams. Quant apes, I am eternally grateful for what you've done and I know that this sub is too. Again, this just shows how many extremely smart apes we have in this fight. This is going to be by far my most data-driven DD of all time.

Many of you have probably seen the spoilers that I gave in my request for data that this DD would be about using correlations, models, and data to get to an extremely high level of certainty that shorts have indeed not covered by analyzing GME as compared to the other meme stocks and some other indicators as well. This was inspired by the pretty obvious fact that they all have traded in very similar patterns since around December. I also noticed that they all seemed to have some sort of FTD cycle component to them as well. I really drew the line when all of these stocks started this upward momentum in the past week - it was just too much of a coincidence for there not to be a relationship. A short squeeze is rare. Stocks following the same trading pattern is weird. A stock squeezing two times in less than a year is weird. A stock trading at over 4x it's book value consistently for months is weird. But 6 stocks doing all of those things simultaneously is..... ASININE. Some might call it improbable, but I think we all know what it is. This DD will use data, a shit ton of it, to give us the closest proof next to actually seeing HFs positions that they have indeed not covered..... ENJOY

Roadmap

In this DD, I will discuss why the meme stock craze is not a just a bunch of retail traders pumping up stocks. Instead, it is the product of the greatest shorting fail in the market of all time that was made possible by easy money policies and apes' uncanny ability to buy and hold. Next, I will discuss the statistical significance and origin of the FTD cycle. Finally, I will give you a random dump of DD at the end of my thoughts.

Part 1: A data driven approach to the meme stock craze

A visualization of what you already knew

As many of you know from some of my previous posts, my thesis is that the "meme stocks" are all related. This was based on observations that the charts looked similar from December to now in terms of price action and volume. The quant apes did an excellent job of visualizing this. Below is a visualization of the meme stocks compared to cryptos and boomer stocks for reference. The parameters are volatility and volume.

[![r/Superstonk - Hank's Big Bang: Quant Apes Glitch the Simulation](https://preview.redd.it/sfs0rlgprt371.png?width=1626&format=png&auto=webp&s=f28599498018462de65d04a0663206ff4d64a623)](https://preview.redd.it/sfs0rlgprt371.png?width=1626&format=png&auto=webp&s=f28599498018462de65d04a0663206ff4d64a623)

[![r/Superstonk - Hank's Big Bang: Quant Apes Glitch the Simulation](https://preview.redd.it/ckanpxbqrt371.png?width=1652&format=png&auto=webp&s=553e7ceae6eddd1a387febf88e0e1a3ffe03e117)](https://preview.redd.it/ckanpxbqrt371.png?width=1652&format=png&auto=webp&s=553e7ceae6eddd1a387febf88e0e1a3ffe03e117)

[![r/Superstonk - Hank's Big Bang: Quant Apes Glitch the Simulation](https://preview.redd.it/6wb6ze0rrt371.png?width=1624&format=png&auto=webp&s=46a16bda7b06735d23ed2b6cb9def15472d53703)](https://preview.redd.it/6wb6ze0rrt371.png?width=1624&format=png&auto=webp&s=46a16bda7b06735d23ed2b6cb9def15472d53703)

(Credit for above three charts to u/Ivorypetal)

A visualization of what you already assumed

This is a visualization of what we already know but haven't been able prove: the stocks are related. Looks like there's a relation, right? How can we be sure? If you took a college or high school statistics course, you probably know that there are certain tests you can run to determine if inputs are correlated, the degree of the correlation, the certainty, and the statistical significance. Below, the quant apes used a statistical test (I won't explain it because if you aren't familiar with statistics it'll take too long to explain, but this is not a guess, it uses an equation to determine the level of correlation, so it is extremely accurate) to determine the correlation of GME to other meme stocks and the VIX. I put GME in red because it's all we care about right now. The top is a comparison of these stocks entire data (i.e. all time), while the bottom compares them in the last year:

[![r/Superstonk - Hank's Big Bang: Quant Apes Glitch the Simulation](https://preview.redd.it/92ks0y4trt371.png?width=860&format=png&auto=webp&s=03932694664e27f9dbfde8042d03f3be181a2559)](https://preview.redd.it/92ks0y4trt371.png?width=860&format=png&auto=webp&s=03932694664e27f9dbfde8042d03f3be181a2559)

[![r/Superstonk - Hank's Big Bang: Quant Apes Glitch the Simulation](https://preview.redd.it/hbahq3rtrt371.png?width=862&format=png&auto=webp&s=328a0b47ad63faae068e12c847dacdc1df2ef9bb)](https://preview.redd.it/hbahq3rtrt371.png?width=862&format=png&auto=webp&s=328a0b47ad63faae068e12c847dacdc1df2ef9bb)

(Credit to u/phalanxhydra)

As you can see, the difference between all time and the last year is striking. The above decimals are called correlation coefficients. They go up to 1 (which means they are identically correlated). Anything above 0.7 is considered a strong correlation. As you can see all of them except for NAKD and NOK have a strong correlation to GME. What really struck me was the VIX. Because the market usually goes down when the VIX goes up, the fact that GME and the VIX have such a strong correlation in the past year is extremely important for our thesis that HFs are actively acting against it.

OTC Data

The chart below takes the OTC data from FINRA and plots it for each of the meme stocks. Notice how they all seem to follow a pattern of spiking every few weeks (FTD cycle) except for the blue one. The blue one is not a meme stock, it's Apple. I used Apple as a reference security so you can contrast how weird this is. Sadly, we don't have FINRA data before 2019, so it's difficult to analyze this in terms of when it started, but you can definitely see a related pattern of abnormality:

[![r/Superstonk - Hank's Big Bang: Quant Apes Glitch the Simulation](https://preview.redd.it/psbp9arwrt371.png?width=2766&format=png&auto=webp&s=1286b2fb12123ba6bf01eaf408917a7f47915530)](https://preview.redd.it/psbp9arwrt371.png?width=2766&format=png&auto=webp&s=1286b2fb12123ba6bf01eaf408917a7f47915530)

(Credit to all of the quant apes who made this customizable program that allowed me to do this)

How common are squeezes?

Squeezes are rare. Extremely rare. Whether you think the January price run up was a short squeeze, a gamma squeeze, or just a big price increase does not matter because, in asking the quant apes to find the exact number of short squeezes that have occurred in the stock market, I gave them VERY broad parameters. The parameters I gave them were: any stock that has doubled in price within a week. Because of this, this is undoubtedly a gross overestimate of the number of short squeezes in the history of the market (i.e. some little known penny stock getting FDA approval and going 4x overnight). The numbers that they found show us just how rare a short squeeze is, and remember, even this is an overestimate, so they're probably even rarer. The quant apes used the major exchanges NYSE, NASDAQ, and AMEX. Here are the results:

[![r/Superstonk - Hank's Big Bang: Quant Apes Glitch the Simulation](https://preview.redd.it/o1rcuupyrt371.png?width=2032&format=png&auto=webp&s=a16b8200dde9417a18b25c4eed0e353557879555)](https://preview.redd.it/o1rcuupyrt371.png?width=2032&format=png&auto=webp&s=a16b8200dde9417a18b25c4eed0e353557879555)

(Credit to u/jyzaya)

If you can't understand that data, here's the point: they are rare, even with parameters that purposefully overestimate it. They are so rare that you could call them an anomaly because that's what they are. Remember that's a purposeful overestimate that allows small stocks getting good news, IPOs, etc. to be considered. So yes, short squeezes are rare. Multiple squeezes following the same pattern and all squeezing at the exact same time? Some might call it improbable, but we all know what we call it.

My take

So, you've seen the data. These stocks are correlated. Does a correlation mean that there is some orchestration going on or that something is forcing them to move in concert? No. It means that they typically move in the same direction, reason unknown. A statistical test can't tell us the reason for the correlation, it can just tell us the correlation. I think I know the reason.

What I think many people, especially the media, take for granted is just how weird January was. As you now know from above, short squeezes are rare. Stocks correlating is weird. Stocks correlating for months is weird. Stocks squeezing at the same time is weird. Stocks doing all of those things at the same time is unheard of. The weird thing about January is that brokers, all of them, simultaneously restricted the buying of all of these stocks. Because liquidity works both ways (buy and sell), if they really had liquidity issues, they would've stopped buying and selling. Also, does it make any sense that every single broker would have liquidity issues at the exact same time during the times of the lowest interest rates ever and an easing of banking restrictions? No. None of that makes sense. My thesis is that all of these stocks are related and the data backs that up. I believe that the brokerages saw that these stocks posed a SYSTEMIC risk because of how exposed major market makers and HFs were on the short side. Why else would they all simultaneously ban only buying?

To add even further to that, many brokerages have banned the shorting of these stocks (months after the squeeze). Even more is all of the shill activity of people messaging us saying "I'll pay you to write something bad about GME." Moreover, the brokerages must have seen that retail, and now the rest of the market, was piling on buying orders and that eventually, some of the most important institutions could go bankrupt and cause an economic crisis. So what did they do? They restricted all buying. Even if every single ape hodled, the price would still be able to go down significantly due to shorting and institutional selling. So yes, they forced it to go down. Now, what was that systemic risk I was talking about? What exactly did the HFs do? As most of you know, I was one of the apes that started the talk of FTD cycles and found many of the rules behind it. The FTD cycle has been the only thing that we've been able to consistently predict (well that and the media being retarded but I digress). IMO, the FTD cycle is our clue into what the HFs did to cause a systemic problem. The FTD cycle has been increasing exponentially, which leads me to believe that the systemic risk has only gotten worse, and I think I've discovered it's origins...

PART 2: The statistical significance and origins of the FTD cycle

Now that I've left you with that cliff hanger and probably a half chub, it's time to take an extremely in-depth dive into the FTD cycle. First, I will be demonstrating the statistical significance of the FTD cycle, so that we know it's not just a fluke. Next, I will discuss the origins of the FTD cycle. Finally, I will discuss what I think it all means.

First, let's start with a brief summary and update on the FTD cycle. The FTD cycle is the idea that because of SEC regulations requiring market makers to cover FTDs within 35 calendar days, there is a predictable increase in price and volume every 21ish trading days or 35 calendar days. So far, it has continued to repeat itself. The idea is that shorts are in so deep that they are doing the bare minimum to cover and continue to dig themselves in a deeper hole by kicking the can down the road. It is currently increasing exponentially, which indicates that it is getting more and more expensive for shorts to stay in the game.

[![r/Superstonk - Hank's Big Bang: Quant Apes Glitch the Simulation](https://preview.redd.it/pgikvf01st371.png?width=1412&format=png&auto=webp&s=8eecc3c7176aa22a77b37c302a9d57bc197f7477)](https://preview.redd.it/pgikvf01st371.png?width=1412&format=png&auto=webp&s=8eecc3c7176aa22a77b37c302a9d57bc197f7477)

Orange line represents FTD cycle increases each month. Yellow lines are FTD cycles. Disregard the red lines, those were my trend lines before we broke out

SI by the charts

Below is a chart that the quant apes gathered from Ortex showing the SI of the meme stocks over time. Many of you will say that this is inaccurate because the real SI is hidden. While we have many instances of that being true, this is the best concrete data that we can gather (much better than Fintel and FINRA), so it's what we must use to avoid speculation. So, yes these numbers are probably an understatement but that's a good thing because we do not want to speculate. If we can find significant results on incomplete data, our thesis is strengthened:

[![r/Superstonk - Hank's Big Bang: Quant Apes Glitch the Simulation](https://preview.redd.it/88i9r528st371.png?width=1750&format=png&auto=webp&s=89c540227a2e8d7f969d110a7d0ef60042ec423b)](https://preview.redd.it/88i9r528st371.png?width=1750&format=png&auto=webp&s=89c540227a2e8d7f969d110a7d0ef60042ec423b)

(Credit to u/orangecatmasterrace)

I noticed some very interesting things from this chart. First, I noticed that the SI of most of the meme stocks markedly increased in mid 2019. GME had an exceptional increase (I think because of their issuance of bonds, shorts saw that as a debt death sentence). There was also a slight, but noticeable, rise in SI of most of these in mid 2016 as well. Hmmmmmm. My original thesis was that they were all heavily shorted after the covid crash because HFs predicted a bad economy and the destruction of brick and mortars, so they used the low interest rate and low liquidity environment to their advantage. That is still probably true as I bet they did it with naked shorts, but this chart made me think even more. What happened before Covid that could've led to these SI increases.

Friend of the shorts: The US economy

The first thing I did was get a chart of short volume data in the stock market over time to get the big picture:

[![r/Superstonk - Hank's Big Bang: Quant Apes Glitch the Simulation](https://preview.redd.it/lhxdy8t9st371.png?width=1374&format=png&auto=webp&s=f8f711ef8dab8cc36f77ee6d55fc852ed693393b)](https://preview.redd.it/lhxdy8t9st371.png?width=1374&format=png&auto=webp&s=f8f711ef8dab8cc36f77ee6d55fc852ed693393b)

As you can see SI has increased markedly in 2015 and 2019. So that got me thinking, there must be some kind of law, some correlation with FED policy, or some kind of macroeconomic happening that led to this. So next, I looked at the interest rates for interbank lending:

[![r/Superstonk - Hank's Big Bang: Quant Apes Glitch the Simulation](https://preview.redd.it/z3677egbst371.png?width=1234&format=png&auto=webp&s=ac740b8236851f40bb01e0eb7fce99a80b550396)](https://preview.redd.it/z3677egbst371.png?width=1234&format=png&auto=webp&s=ac740b8236851f40bb01e0eb7fce99a80b550396)

This is not mortgage interest rate, this is federal funds interest rate, which is essentially the interbank interest rate for excess lending. As you can see it's been insanely low since the 1990's, but particularly low as of recently. Next, I looked at the balance sheet of the FED. This essentially shows the Fed's buying of assets over time.

[![r/Superstonk - Hank's Big Bang: Quant Apes Glitch the Simulation](https://preview.redd.it/rd1ye3ddst371.png?width=1630&format=png&auto=webp&s=f284394415c8cd127d750bbcd45f55ef676d0fd0)](https://preview.redd.it/rd1ye3ddst371.png?width=1630&format=png&auto=webp&s=f284394415c8cd127d750bbcd45f55ef676d0fd0)

[![r/Superstonk - Hank's Big Bang: Quant Apes Glitch the Simulation](https://preview.redd.it/ygpfqudest371.png?width=1554&format=png&auto=webp&s=5cf6fa82247426f7a83db8d202be1f85b3c5f8be)](https://preview.redd.it/ygpfqudest371.png?width=1554&format=png&auto=webp&s=5cf6fa82247426f7a83db8d202be1f85b3c5f8be)

The above graph is especially striking. It shows the FED's balance sheet is increasing proportionately with the SP500. The FED's Quantitative easing policies have been extremely aggressive since 2008. QE is where the FED purposefully stimulates the economy by buying assets like bonds. This was necessary after 2008 and the FED kept it going for a while then started tightening (QT). However, and this chart doesn't show it, the FED had to parabolically increase its QE policies duirng covid. You know what else parabolically increased? Yep, the stock market.

The statistical significance of the FTD cycle

[![r/Superstonk - Hank's Big Bang: Quant Apes Glitch the Simulation](https://preview.redd.it/79rg4j9gst371.png?width=1284&format=png&auto=webp&s=33e2deedfeb5f2caa5c1914e8caa828071214862)](https://preview.redd.it/79rg4j9gst371.png?width=1284&format=png&auto=webp&s=33e2deedfeb5f2caa5c1914e8caa828071214862)

[![r/Superstonk - Hank's Big Bang: Quant Apes Glitch the Simulation](https://preview.redd.it/3qzw1f0hst371.png?width=1274&format=png&auto=webp&s=5b591b0a0bfe04debd67f0561a971ac797651e78)](https://preview.redd.it/3qzw1f0hst371.png?width=1274&format=png&auto=webp&s=5b591b0a0bfe04debd67f0561a971ac797651e78)

[![r/Superstonk - Hank's Big Bang: Quant Apes Glitch the Simulation](https://preview.redd.it/y9iekcuist371.png?width=1284&format=png&auto=webp&s=39b9bc492e20a346bdeef2ab210cdf6d9196303a)](https://preview.redd.it/y9iekcuist371.png?width=1284&format=png&auto=webp&s=39b9bc492e20a346bdeef2ab210cdf6d9196303a)

(User wished to remain anonymous for this)

The above charts show GME's FTD cycle increases after a certain number of days. I put TSLA and MSFT in there so that you could see how abnormal GME is. Even compared to a volatile stock like TSLA, GME has a way more recognizable pattern, which gives us further statistical evidence of the FTD cycle. Also, note that there were many other users in different posts on this sub who found the FTD cycle statistically significant, this is another view to add to the body of work. Below shows the short interest of the meme stocks in relation to each other, so you can see when they started and how they've increased together:

[![r/Superstonk - Hank's Big Bang: Quant Apes Glitch the Simulation](https://preview.redd.it/765vp0kqst371.png?width=510&format=png&auto=webp&s=03d70c989c96d63c0d3321acdd8e081b9ed903c8)](https://preview.redd.it/765vp0kqst371.png?width=510&format=png&auto=webp&s=03d70c989c96d63c0d3321acdd8e081b9ed903c8)

(credit to u/orangecatmasterrace)

Keep the above chart in mind while reading below.

The takeaway:

We are in an EXTREMELY easy lending environment. Rates are dirt cheap. The FED is buying up assets, which is pushing up the prices of literally all assets. The market is flush with liquid assets, so much so that the FED was trying to slow it down. This makes the perfect storm for a short-friendly environment. We were also in the longest and biggest bull market run of all time in 2010's, so it would make sense for it to come to an end soon - that's where shorts really make a killing.

What I think happened is that we saw the longest bull market of all time in the 2010 decade. HFs realized that this bull market was propped up on the FED's massive balance sheet and that there would need to be more economic tightening soon and/or a correction. Anticipating an end to the bull market, they initiated a giant short campaign in 2019 with the aforementioned meme stocks and probably tons of others (the meme stocks are just the ones that retail investors took interest in). Once Covid hit, their campaign was successful, but they wanted more. They wanted to hit the bankruptcy jackpot, so they turned it up with the naked shorts, which is why the data doesn't show that, in an attempt to put brick and mortars out of business.

Instead, the FED accelerated its easy money policies and the economy had one of the quickest recoveries of all time. This is why I think we started seeing the FTD cycle in late 2020 - it was a result of their failed mega short during covid. This alone would've made them lose money but they've run into roadblocks like this before so it's not what caused the squeeze and mania. What caused that was the fact that apes literally buy and hold but never sell. This essentially created a giant wall that wouldn't allow the HFs to short down out of their positions and got them into this mess. Then some retail investors caught wind of it and bought into some of their most shorted stocks, which is why we saw what happened in January. They are still in that hole because the brokers' pausing of buying didn't solve the problem, it just delayed it. That's why we see the FTD cycle exponentially increasing. This economic environment has been brewing for this for a long time, and it would have continued if not for reddit (mainly DFV). I mean how crazy is it that GME's SI was over 100% for so long and no one noticed?

I am convinced that this would not have been able to continue to happen if apes didn't hold. That's why this was all able to happen. It's because there has never been a phenomena in the market where a significant portion of investors in a stock will hold it no matter what the market conditions are. So when shorts started aggressively shorting and things turned south because of the FED's recovery policies, retail's refusal to sell just added insult to injury and is why we are in this position now.

(Please note that the above data I only actually displayed a fraction of the quant apes' data. They gave me an amazing amount. I used some of it to inform my/guide myself and displayed charts that went well with my DD, so believe their work is even more in-depth than this post portrays)

Part 3: DD Drop

Alright apes, the above was a mouthful, but wow aren't our quant apes amazing! Now that you've read all of that, I am going to do another one of my DD drops on some random theories, updates, etc.

Everyone remember what happened with Archegos? That was a real funny one wasn't it? Bill Hwang plead guilty to insider trading, so he had to operate a family office. The man lost $20 billion in the span of 2 days, now that's a level of yolo retardation we should all strive for. One of the companies that Hwang invested in was Discovery, here's it's chart:

[![r/Superstonk - Hank's Big Bang: Quant Apes Glitch the Simulation](https://preview.redd.it/4qnz2xesst371.png?width=2206&format=png&auto=webp&s=f4c7320665b27f95a8b9ffe05328d7e93bb26b3a)](https://preview.redd.it/4qnz2xesst371.png?width=2206&format=png&auto=webp&s=f4c7320665b27f95a8b9ffe05328d7e93bb26b3a)

See that purple line? I bet you probably think that's VWAP or a SMA line, right? NOPE. That's VIAC (Viacom CBS), one of the other companies he bet big on. Hwang used an instrument called total return swaps, which basically allow you to "swap" the delta of one baseline security for another. Here's an example: a total return swap of Apple and SPY. You get the returns of APPL. If AAPL outperforms SPY, you make money, but if not, you owe them money. That was all a huge oversimplification but essentially, it allows you to have exposure to a company without owning it (derivative). That above chart was just a 1 year chart, but essentially, Hwang applied so much leverage to these companies through these swaps that they were trading at double their fair market price.

This hypothesis is backed by no data whatsoever and is really just a thought experiment. Based on the fact that meme stocks correlate (as shown above), what if HFs are using some type of swap on them? It would make sense given the extremely low interest rates. It would make even more sense given the negative beta of GME (i.e. SPY would be the reference security). Perhaps they use total return swaps or another instrument to cover or to add more pressure? Idk. Just a thought.

Another hypothesis: could this all be the work of an algo? I mean, there's no more observing the similarities, we now know they are statistically significant and related. IMO, it's impossible for human traders to create this pattern -- it's just too precise and based on too much volume, so the options are either they shorted all of these at the exact same time and are being forced to cover at the exact same time (FTD cycle), an algo is doing that for them, or some algo is orchestrating all of this. I find that unlikely because of the difficulty and obvious market manipulation charge they'd get but we have to consider it! Again, just another thought, not much else to it.

The Midday Spikes: An Answer

Apes, we might have an answer to the midday volume spike phenomena. If you don't know what I'm talking about, see my other post. My hypothesis was that these midday spikes were HFs covering to satisfy some kind of requirement or to avoid some kind of FTD cycle. I had no evidence for the cause, I just had tons of observations for the occurrence. Let tell you though, if there's one thing I know, it's that it's not retail. Whatever is behind the midday spikes is a single entity. It is impossible for a bunch of unorganized people to consistently buy a stock in the same minute interval in mass. That is a single entity doing that and I think whoever it is is our enemy. A beautiful ape by the name of [u/KFC_just](https://www.reddit.com/u/KFC_just/) turned me on to the idea that it may be to comply with net negative rules. I scoured the interwebs and found this on NASDAQ:

[![r/Superstonk - Hank's Big Bang: Quant Apes Glitch the Simulation](https://preview.redd.it/qvze3s1vst371.png?width=1954&format=png&auto=webp&s=296a2ead951725c90722f157d402a86b34854748)](https://preview.redd.it/qvze3s1vst371.png?width=1954&format=png&auto=webp&s=296a2ead951725c90722f157d402a86b34854748)

Notice that it also talks about clearing corporation requirements, which adds another elements into the mix. Though I can't find any information about exact requirements in terms of liquidity/numbers, I think that this is pretty definitive proof of the reasons for the midday spikes. Essentially, it seems as though these midday spikes are some fund covering in order to "maintain net capital sufficient to comply with the requirements of the Clearing Corporation." Also, the final sentence explains why they need to cover (i.e. to remain positive).

Earnings and 6/9

A lot of you are probably extremely excited for earnings and the annual meeting on 6/9. I am too. However, I wanted to make this to tell you to not get your hopes up too much and to not be surprised if it doesn't go our way. What I will say is, I am confident that we will see a dildo candle one way or another. For earnings, remember that last quarter the earnings were not even bad and the stock had a GIANT red dildo candle. Unless earnings are absolutely spectacular, I could see HFs using it as a way to put negative momentum on the stock (remember, it's all about the narrative). Now, earnings could be spectacular. GME has gotten so much more attention this past quarter and I know that apes have been feverishly shopping there, so we do have hope.

As far as the annual meeting I have absolutely no clue what to expect. However, like earnings, I expect another dildo one way or another. If you remember last earnings, we all thought that the guidance/conference call is what would put us over the edge. Instead, it was barebones minimum, and we succumbed to the HFs earnings downward momentum. I expect this to be different. An annual meeting is different from an earnings call and definitely warrants more speaking, more guidance, and more detail. If GME was going to announce some blockbuster move, it would be during this because, assuming they know about the massive short interest, that gives them plausible deniability against market manipulation charges. Some important topics we could hear about are: Ryan Cohen speaking in general, a new CEO, crypto/NFT, acquisitions, digital transformation / direction, and, most importantly, the voting results. Is there a guarantee that these things will be discussed? No. Do I expect many of them to be discussed? Yes. Similar to earnings, we could get great news and see a giant red dildo candle. Remember, expect anything. If we get more shorting on positive news, it just keeps proving we are right.

As for my thoughts on when we moon, I personally don't think we'll moon here almost no matter what. I think that it will be overall good and that we will see a very significant jump, but instead of that being the MOASS, I think it will be what starts the MOASS. The only thing we've been able to predict has been FTD cycles so far. The MOASS will come when a HF gets margin called and we just can't predict the exact time for that. So, I believe that if we see a big jump next week, the MOASS should be coming in the near future but will nevertheless be unpredictable.

Clarification of my statements about retail buying

In one of my past posts, I said something along the lines of "retail is tapped out." Thankfully, another user made a post disagreeing with that and it got tons of replies of apes saying things like "I have tripled my position in the past month." If you haven't seen that post, I'd look at it, the responses are amazing. With that in mind, I wanted to clarify what I said about that. What I meant in that post is that retail is not responsible for the mass, synchronized buying that we've seen in the past week or so, I think that is HFs being forced to cover. Retail, instead, has been holding like champs and steadily buying. IMO it's pretty hard to believe that retail just randomly decided to buy every stock that squeezed in January at the same time. Instead, I think it's something much bigger but apes' ability to hold is why it's able to happen. However, I do think that once we start squeezing again, it will bring in a new wave of retail that formerly wasn't in just like January, so we still do have gas in the tank (or ions in the battery if you drive electric).

Big Thanks to the Quant Apes

I can't tell you how seriously amazing the quant apes are. They deserve all of the credit in the entire world and they are one of the most valuable parts of this sub.

Here is a list of some of the quants who helped with this post (this is not exhaustive as some wanted to remain anonymous)

[u/orangecatmasterrace](https://www.reddit.com/u/orangecatmasterrace/)

[u/spambot9k](https://www.reddit.com/u/spambot9k/)

[u/rubberbootsinmotion](https://www.reddit.com/u/rubberbootsinmotion/)

[u/Ivorypetal](https://www.reddit.com/u/Ivorypetal/)

[u/creativelord](https://www.reddit.com/u/creativelord/)

[u/collegeneral](https://www.reddit.com/u/collegeneral/)

[u/xpurplexamyx](https://www.reddit.com/u/xpurplexamyx/)

[u/jyzaya](https://www.reddit.com/u/jyzaya/)

[u/epk-lys](https://www.reddit.com/u/epk-lys/)

[u/head4headsup](https://www.reddit.com/u/head4headsup/)

[u/squirrel_of_fortune](https://www.reddit.com/u/squirrel_of_fortune/) (he made a great DD as well and I would encourage you to check that out to see another perspective with a very interesting, advanced method)

[u/sudoshu](https://www.reddit.com/u/sudoshu/) (Special thanks to him as he was the organizer of the group. If you are a quant ape, he said to message him if you are interested in being in the group, but serious inquiries only).

Mods: many of these users do not have the karma requirements to comment on posts. If you could somehow waive that requirement for the listed users, I think it would really benefit the sub because the amount of knowledge that these apes possess is amazing. They put so much time into this and gathered so much data (I literally couldn't even show close to all of it) and I believe that they will be integral to the continued success of this sub.

Finally, the quant apes have created a website: <https://www.superstonkquant.org/>

They are still currently working on the mechanics of it but I encourage you to monitor it in the future because I have witnessed first hand what they are capable of and it is nothing short of amazing.

Conclusion

Alright apes, that was very long but I appreciate you for reading. This sub keeps doing a great job of pumping out DD and I think we will be rewarded for it in the very near future. I am going to take a break from making DDs because it is really time consuming and can be extremely tiring, but I will still be looking at this sub, commenting, and possibly making short posts. As always,

*Stay strong, apes.*

********** I am not a financial advisor, this is not financial advice **********
