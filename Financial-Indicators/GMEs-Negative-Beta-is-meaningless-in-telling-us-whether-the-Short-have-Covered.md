Why GME's negative beta is meaningless and tells us nothing one way or the other about whether the shorts have covered
======================================================================================================================

**Author: [u/Beartholomew](https://www.reddit.com/user/Beartholomew/)**

[DD](https://www.reddit.com/r/GME/search?q=flair_name%3A%22DD%22&restrict_sr=1)

TLDR: GME's negative beta doesn't mean anything, it's caused by the stock's huge increase from December to January and the way that beta is calculated.

This is a response to [a post claiming that GME's negative beta is evidence that the shorts have not covered](https://old.reddit.com/r/GME/comments/m6i4z2/the_mythical_unicorn_aka_extremely_abnormal/). On the face of it, this isn't the stupidest thing that I read today, but it seemed like a reach at best:

> About GME specifically
>
> Here is the historical beta of GME:
>
> 02/28/2021 -2.195
>
> 12/31/2020 1.404
>
> 09/30/2020 1.084
>
> 06/30/2020 1.038
>
> 03/31/2020 0.4512
>
> You can see that GME's beta has only been negative since end of Feb 2021. Before that it had a very normal beta of over 1, meaning when the market was doing well, then its business did well too, i.e. people have money to spend on games, etc. Even during most of the lockdown its beta was still quite a bit above 1. But at the end of Feb, it suddenly went all the way down to -2.195. What happened at that time? The massive crash down to $38. Plotkin himself said that the rapid rise in price was not due to shorts covering right? But have they covered since one way or the other? The beta would indicate no because now the beta is even lower, at -2.09. Since Yahoo confirms Nasdaq, I think the FT is sus and in the best case just doesn't update its data. -1.7413 is still remarkable though.
>
> [...]I don't know how the beta is calculated by these news outlets but I think it must be done automatically by the bots and even if FT were a shill and not simply inaccurate, the beta of -1.7413 is still crazy.

What struck me, however, is that GME's beta supposedly didn't go negative until February. Wasn't GME shorted to shit well before February? Why would beta only plunge in February? The worst part, though, is that the commentary reveals that the writer of the original DD ([u/animasoul](https://www.reddit.com/u/animasoul/) ) didn't look into how beta is calculated. How are you going to start attributing meaning to a number without understanding where it comes from?

So I looked into how beta is calculated, and sadly GME's negative beta is entirely meaningless, an artifact caused by an outlier. Here's what do you need to know:

1.  Beta is easy to calculate. You can do it yourself with Excel following [these steps](https://investexcel.net/how-does-yahoo-finance-calculate-beta/).

2.  The beta reported by Yahoo Finance et al is calculated using only 36 monthly data points. This is not very many, which means the calculation can be skewed by outliers fairly easily.

3.  There is a [HUGE OUTLIER in January that wrecks the whole calculation](https://imgur.com/a/JMEaUZ0). This is why the beta suddenly went negative in February. Basically, when looking at monthly pricing, GME went up 1625% from December to January, while the benchmark went down -1%. This completely warps the beta calculation but wasn't caused by any kind of shorting activity, because the offending data point is one where GME's stock price is RISING, while the market is falling. If you remove this outlier, [GME's beta is POSITIVE 1.58](https://imgur.com/a/iYjrBR3). If the market had risen 1% instead of falling 1% that month, [GME's beta would have been 1.06](https://imgur.com/a/SOTHAG3).

Long story short, GME's negative beta isn't a story about whether or not the shorts have covered, it's a story about a stock going to the moon (+1625%) in a month when the rest of the market went down slightly (-1%) and how that single data point warped the 36 month average because the stock's upward movement was so pronounced. The stock's beta could remain negative for three years, until the outlier falls out of the 36 month calculation period, or it could revert to positive if there's another massive swing in the stock price that is positively correlated with the market, offsetting the January outlier. While the outlier was caused by the FTD/gamma/short squeeze (or not, if you subscribe the theory that nothing has squoze yet), since then, none of this has anything to do with whether the stock is currently being shorted, or whether the shorts are covering.

Anyone with a spreadsheet and an internet connection could have come to this same conclusion, so do a little research before believing everything you read, even if it's long, supports your preconceptions, and ends with diamond hand emojis.
