Negative Volume Prints
======================

| Author       | Source       | 
| :-------------: |:-------------:|
|  [u/dlauer](https://www.reddit.com/user/dlauer/) | [Reddit](https://www.reddit.com/r/Superstonk/comments/n772fg/negative_volume_prints/) | 

---

[Education 👨‍🏫 | Data 🔢](https://www.reddit.com/r/Superstonk/search?q=flair_name%3A%22Education%20%F0%9F%91%A8%E2%80%8D%F0%9F%8F%AB%20%7C%20Data%20%F0%9F%94%A2%22&restrict_sr=1)

I have been looking into the negative volume prints, because I agree it's very strange. However, just to be clear, I believe in Occam's Razor, and so am still under the impression that this is a bug or data glitch. Here's what I've done so far:

-   I have two data providers for this kind of information, one for raw market data and the other for historical fundamental data. Neither shows anything strange. This was not something that came in the raw market data feeds. The historical fundamental data provider I use shows this as the last 3 days' trading volumes:

"date": "2021-05-06", "value": 2942802.0

"date": "2021-05-05", "value": 1789186.0

"date": "2021-05-04", "value": 4007512.0

-   I do not see negative volume bars in Fidelity or Interactive Brokers.

-   I reached out to a friend who is very high up at one of the exchanges. He had the same reaction to this as I have. Here is what he said:\
    Corrections to the tape are rarely (if ever) done. It's mostly cancels to ensure last sale is correct. There is no "input" for a negative number. Its cancel old and insert new.\
    If they use like a last sale feed for api from somewhere else - well that could be a bug. Can it be corroborated with other sources?

If this is just TD Ameritrade, then it could simply be a bug on their side. If this is seen in other discount broker platforms, then the likeliest explanation is that they are all using the same data provider and there's some unexpected data coming down the pipe via API.

So here's what I'd ask. First, if you see this somewhere other than TDA, let us know in the comments. My friend at the exchange is interested too.

Second, reach out to your broker if you see it and ask what's going on. Let's see what they say, and I can let you know if they're bullshitting or not.

Finally, I still don't see the mechanism for this to be indicative of any kind of margin call. I don't mean to throw cold water on it, but if there was a margin call of any size, the only way you'd know is from news reports. It would not show up in market data. Trades wouldn't be busted at the end of the day because of no collateral, at least as far as I've ever seen. I don't claim to know everything, but I've seen trades busted before and this isn't what it would look like.

Hope this is helpful!
