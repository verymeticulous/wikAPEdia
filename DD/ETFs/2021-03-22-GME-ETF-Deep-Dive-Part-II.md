GME ETF Deep Dive - Analysis of Failures to Deliver and Short Volume
====================================================================

| Author       | Source       | 
| :-------------: |:-------------:|
|  [u/the_nebraskan](https://www.reddit.com/user/the_nebraskan/) | [Reddit](https://www.reddit.com/r/GME/comments/manyso/gme_etf_deep_dive_analysis_of_failures_to_deliver/) | 

---


[DD](https://www.reddit.com/r/GME/search?q=flair_name%3A%22DD%22&restrict_sr=1)

this is a follow on to my earlier post regarding ETFs holding GME [here](https://www.reddit.com/r/GME/comments/makcor/etf_holdings_of_gme_compiled_current_as_of_22_mar/).

to start, i would like to cover the sources i pulled all of my data from. here is the [spreadsheet](https://docs.google.com/spreadsheets/d/1SWK2krtYHqrGu222bVGhRwTP9niW-0t-_9Bbpwru3jY/edit?usp=sharing) i created with all the data i used, see various tabs.

*SOURCES*

ETF outstanding shares - annual reports pulled from [Fidelity](https://screener.fidelity.com/ftgw/etf/goto/snapshot/quote.jhtml?symbols=XRT)

ETF GME holdings - a combination of daily reports, monthly, or annual, links on first tab of [spreadsheet](https://docs.google.com/spreadsheets/d/1SWK2krtYHqrGu222bVGhRwTP9niW-0t-_9Bbpwru3jY/edit?usp=sharing)

short volume - [regsho.finra.org](http://regsho.finra.org/regsho-January.html)

failures to deliver - [sec.gov](https://www.sec.gov/data/foiadocsfailsdatahtm)

because someone is bound to ask ... no my smooth brain didn't copy all the data by hand. i went to computer monkey school where papa ape taught me python, if you want the scripts dm me

*SHORT VOLUME*

now for some smooth brained anal-ysis. first graph is a pie chart showing the major ETFs holding GME. [link to pie chart](https://imgur.com/0N6gGmf). there have been a lot of posts the past few weeks concerning ETFs, specifically in regards to short selling, so I wanted to dig a little deeper.

i pulled all the short volume data from finra and failure to deliver data from the sec starting in Sep 2020. i filtered for only GME and GME ETF data using my python scripts.

this [first graph](https://imgur.com/3wmidrW) shows the total trade volume of GME over the past 6 months as reported by finra. nothing too special here. what is more interesting is if you look at the short volume of the same securities as a percentage of the total trade volume. these two graphs [1](https://imgur.com/6rVeSTB) [2](https://imgur.com/JBObY0q) show how for both GME and ETFs holding GME, the ratio of short volume has been trending upwards and are now both over 50%!

*FAILURES TO DELIVER*

now onto failures to deliver (ftds). this [first graph](https://imgur.com/vPe3lLp) shows the total number of GMEs shares (including those held by ETFs) that failed to deliver as a percentage of float. I estimate the number of GME shares that fail to deliver from ETFs (see footnote if interested). Also worth mentioning is that I choose to use the float reported by GME in their annual filing to the SEC of 43.6 million as we are concerned with all shares not held by GameStop Corporation.

while the trend of this graph, doesn't show that ftds have been trending upwards the past two months, it does highlight how they all somehow magically disappeared in late January when this whole saga began. many others have posted regarding this phenomena, so i leave it to you to draw your own conclusions from their posts. i was more intrigued by this [second graph](https://imgur.com/HeWny1E) which compares the ratio of ftds of ETFs holding GME to the ftds of GME. As you can see, during the entire month of February, close to the majority of ftds for GME came from ETFs holding GME, not GME itself. furthermore, if we look at the trendline, there has been a consistent increase in FTDs coming from ETFs, rather than GME stock. does this mean that GME shorters attempted to hide their positions by shorting the ETFs instead of continuing to short the standard security? again, that's up to you to decide. because FTD data is reported only twice a month, and a month after the fact, we will have to wait a week or so to see if this trend to continue into march.

*SUMMARY*

tldr - etfs holding gme have been shorted the past 6 months and continue to be so. there is an emerging trend for the majority of ftds to be stemming from ETFs holding GME, not GME itself.

i love the stock and am as bullish as ever. haven't sold a single share and have been buying since feb. that's all i got for today. i'm gonna get some sleep. catch yall when the market closes.

footnote: formula for approximating the # of GME shares that fail to deliver held by ETFs: FTD amount reported by finra for the given ETF divided by the outstanding shares of that ETF then multiplied by the number of GME shares that ETF currently holds.

**mandatory disclaimer: not a financial advisor, this is just my opinion, primarily a data dump for you to draw your own conclusions from
