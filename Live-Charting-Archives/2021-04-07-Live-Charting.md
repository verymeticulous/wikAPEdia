Live Charting for 4/7/2021, predicting the day's price action in detail with Warden.
====================================================================================

**Author: [u/WardenElite](https://www.reddit.com/user/WardenElite/)**

[Serious DD 👨‍🔬🔬](https://www.reddit.com/r/Superstonk/search?q=flair_name%3A%22Serious%20DD%20%F0%9F%91%A8%E2%80%8D%F0%9F%94%AC%F0%9F%94%AC%22&restrict_sr=1)

This is not financial nor investment advice. These are ideas and opinions for information purposes only.

*This post will read bottom to top. It's easier for people to refresh the page and see edits at the top*

Historical supports and resistances:

116.5, 125.5, 132.5, 141, 145, 147.5, 150, 152.5, 156.5, 162.5, 172, 176.5, 179, 180.5, 182, 183.5, 184.5, 186, 187.5, 190.5, 192, 195, 196.5, 197.5, 200, 209, 211.5, 214.5, 218, 226, 230, 234, 243, 250, 253, 256.5

Edit 27 4:10PM:

Odds of a discount tomorrow is 90 - 10. This is an educated guess. Not a certainty.

Edit 26 4:01PM:

Ended around 178.24, down 3.39%. Overall IV seems to have bottomed out. Not bad!

The options calculator code from today's power hour stream.

<https://pastebin.com/15syqnAk>

Edit 25 3:07PM:

9:50am-10:10am I meant*

Edit 24 2:56PM:

Hop on my power hour stream and I'll explain how I know about tomorrow's discount!

<https://www.youtube.com/watch?v=rvhxEULG34w&ab_channel=WardenElite>

Edit 23 2:49PM:

Listen up my beautiful apes. There will likely be a major discount at 9:50am-10:00am tomorrow! Could go as low as 162, then it should recover quickly!

🏷️ 🏷️ 🏷️ 🏷️

Edit 22 2:46PM:

Is it just me or did Wall Street DDOS <https://www.optionsonar.com/>?

Edit 21 1:55PM:

The volume is so low that this is trading like a penny stock again. Look at all these gaps between the candles!

[![r/Superstonk - Live Charting for 4/7/2021, predicting the day's price action in detail with Warden.](https://preview.redd.it/2wrvk1yfisr61.png?width=2146&format=png&auto=webp&s=f142c71d8c1f6bbe122fe3f2daed1d8ca8cb36a1)](https://preview.redd.it/2wrvk1yfisr61.png?width=2146&format=png&auto=webp&s=f142c71d8c1f6bbe122fe3f2daed1d8ca8cb36a1)

Edit 20 1:19PM:

Holy pepperoni pizza. The deep ITM calls are back. Expect a great 5-10% discount tomorrow morning at 9:50 am!

[![r/Superstonk - Live Charting for 4/7/2021, predicting the day's price action in detail with Warden.](https://preview.redd.it/4nc0issybsr61.png?width=2475&format=png&auto=webp&s=720ed773e81735df4774948ae7e4989fef338046)](https://preview.redd.it/4nc0issybsr61.png?width=2475&format=png&auto=webp&s=720ed773e81735df4774948ae7e4989fef338046)

Data courtesy of https://www.optionsonar.com/unusual-option-activity/GME/latest-trades

Edit 19 1:18PM:

This is the formula for calculating an option price "C". You can basically take the current price of options on the market, and do an iterative search to try and guess the volatility. The volatility affects "d1" and "d2".

[![r/Superstonk - Live Charting for 4/7/2021, predicting the day's price action in detail with Warden.](https://preview.redd.it/szeok562asr61.png?width=922&format=png&auto=webp&s=a51ef17b9c05953cd26effce0f059b5bcc87c6a4)](https://preview.redd.it/szeok562asr61.png?width=922&format=png&auto=webp&s=a51ef17b9c05953cd26effce0f059b5bcc87c6a4)

https://www.wallstreetmojo.com/implied-volatility-formula/#:%7E:text=The%20calculation%20of%20implied%20volatility%20can%20be%20done,search%20by%20trial%20and%20error.%20More%20items...%20

-   C is the Option Premium

-   S is the price of the stock

-   K is the [Strike Price](https://www.wallstreetmojo.com/exercise-price-strike/)

-   r is the [risk-free rate](https://www.wallstreetmojo.com/risk-free-rate/)

-   t is the time to maturity

-   e is the exponential term

So if you plug in all those numbers and know what C is, you can guess the IV and plug it into the equation until you get the right C.

`def calc_d1(self):`

`return (m.log(self.S / self.K) + (self.r_dec + self.v_dec**2 / 2) * self.t_yrs) \`

`/(self.v_dec * m.sqrt(self.t_yrs))`

`def calc_d2(self):`

`d1 = self.calc_d1()`

`return d1 - self.v_dec * m.sqrt(self.t_yrs)`

That's code for how I calculate d1 and d2.

Where

`self.t_yrs = time_to_exp_days / 365`

`self.v_dec = annual_vol_pc / 100`

`self.r_dec = risk_free_rate_pc / 100`

Don't worry it can be a bit confusing. I'll cover it on stream and explain how it works.

Edit 18 12:50PM:

So a lot of my posts revolve around Implied Volatility. I figure you guys would be interested in learning how to calculate it and understand what causes IV to go up or down.

I'll be extensively covering how IV is calculated in depth during my power hour stream today. It's a bit involved so I will use my whiteboard to go over how it all works.

I'm currently working on a script that can calculate option premiums and IV. It can also print out the greeks. Will include this in my stream if I get it fully working.

Edit 17 12:32PM:

Pretty bullish bet for mid may.

[![r/Superstonk - Live Charting for 4/7/2021, predicting the day's price action in detail with Warden.](https://preview.redd.it/n7wp97zk3sr61.png?width=2273&format=png&auto=webp&s=ebc365ffd2a0a59ccc9b1ef99f128cf5533ba012)](https://preview.redd.it/n7wp97zk3sr61.png?width=2273&format=png&auto=webp&s=ebc365ffd2a0a59ccc9b1ef99f128cf5533ba012)

Edit 16 12:30PM:

A block of 300 strike calls came in, lemme take a look.

Edit 15 12:18PM:

New support added at 179. Haha at this rate I will have listed every single price GME has ever been at ;)

On a more serious note, you can use a percentage based method and even bollinger bands to narrow in on 1 support that you think it will reach for the day. The multitude of lines are just there as options. It's ultimately up to the technical analyst to pick the ones that are significant for the day.

Edit 14 11:54AM:

IV seems to have bottomed out today. Very interesting... seems to have trouble going any lower. We're nearing pre January levels of IV. Ignore the weird gaps in volatility. That's caused by after hours trading. What I think has caused the uptick in IV is the moderately fast move downwards today. Remember that volatility goes up when the price moves fast. It's still rather slow today, but relatively faster than historical movements.

[![r/Superstonk - Live Charting for 4/7/2021, predicting the day's price action in detail with Warden.](https://preview.redd.it/e1y8atxswrr61.png?width=2201&format=png&auto=webp&s=0656daf6944b9d7755ddf44840491baac4435993)](https://preview.redd.it/e1y8atxswrr61.png?width=2201&format=png&auto=webp&s=0656daf6944b9d7755ddf44840491baac4435993)

If we zoom out to a larger timescale, it would be pretty exceptional if we can drop down to circle 1's IV. However it seems like with the current level of volatility, we might be bottoming out at the same IV as circle two from before the January squeeze.

[![r/Superstonk - Live Charting for 4/7/2021, predicting the day's price action in detail with Warden.](https://preview.redd.it/vypy77caxrr61.png?width=2173&format=png&auto=webp&s=e1f048a7c032f545ddd211f7de71373671a7a7bb)](https://preview.redd.it/vypy77caxrr61.png?width=2173&format=png&auto=webp&s=e1f048a7c032f545ddd211f7de71373671a7a7bb)

Edit 13 11:46AM:

My in depth analysis for the day:

----------------->

*Bows. Thank you. Thank you.*

Edit 12 11:32AM:

Broader market turning around, headed downwards. Even though GME has negative beta, downwards market moves still tend to drag it down. It's more during PM and AH that GME inverts the market. What happens is HFTs go short biased during broader market downtrends, so GME can follow the broader market during HFT only trading hours like midday.

[![r/Superstonk - Live Charting for 4/7/2021, predicting the day's price action in detail with Warden.](https://preview.redd.it/06h9shkzsrr61.png?width=290&format=png&auto=webp&s=da6bce5c111fc7e8b2e87610038f05e11fd6c641)](https://preview.redd.it/06h9shkzsrr61.png?width=290&format=png&auto=webp&s=da6bce5c111fc7e8b2e87610038f05e11fd6c641)

Edit 11 11:17AM:

You know I just noticed something about OptionSonar. They added this watermark. I swear this wasn't here in the past like maybe a week or two ago.

Must be because some people including me forget to link the data below the screenshot so people get confused where this data is coming from (I'm sorry optionsonar!!! I promise I will promote your product ;) It's honestly really great.)

[![r/Superstonk - Live Charting for 4/7/2021, predicting the day's price action in detail with Warden.](https://preview.redd.it/w596xit9qrr61.png?width=2503&format=png&auto=webp&s=10f70dc40255f35f4a4bfa35ebc0bee94bb6ebf0)](https://preview.redd.it/w596xit9qrr61.png?width=2503&format=png&auto=webp&s=10f70dc40255f35f4a4bfa35ebc0bee94bb6ebf0)

https://www.optionsonar.com/unusual-option-activity/GME/latest-trades

Edit 10 11:13AM:

As for 500 strike calls, these are 2022. Someone sold this below the bid. Long term bearish bet that the stock will remain below 500. It could be used as a part of a more complicated options strategy.

[![r/Superstonk - Live Charting for 4/7/2021, predicting the day's price action in detail with Warden.](https://preview.redd.it/lo1vwbjhprr61.png?width=2284&format=png&auto=webp&s=4b00dd7239f7146a87ec7b6bcf3bc441bbbe121e)](https://preview.redd.it/lo1vwbjhprr61.png?width=2284&format=png&auto=webp&s=4b00dd7239f7146a87ec7b6bcf3bc441bbbe121e)

https://www.optionsonar.com/unusual-option-activity/GME/latest-trades

Edit 9 11:11AM:

These are November strike Calls, $440. Long term bullish bet.

[![r/Superstonk - Live Charting for 4/7/2021, predicting the day's price action in detail with Warden.](https://preview.redd.it/3wpz6jj7prr61.png?width=2280&format=png&auto=webp&s=c3bfd9365063b1d08ecb251ca27895698b162713)](https://preview.redd.it/3wpz6jj7prr61.png?width=2280&format=png&auto=webp&s=c3bfd9365063b1d08ecb251ca27895698b162713)

https://www.optionsonar.com/unusual-option-activity/GME/latest-trades

Edit 8 10:59AM:

Most of the downward movements today are on extremely low volume. I remember 2/24 was like this until things picked up mid day. From a technical perspective, it makes the most sense for long side to keep the IV crush going through the week.

Could we see a larger move this week? It's possible because IV is already so low, however keep in mind that Max Pain for this week is higher than next. A larger move next week would make a lot more options expire worthless. Perhaps those large Put purchases yesterday was a setup for a 4/16 battle.

Edit 7 10:26AM:

Hovering around 180, possible support at 176.5 below.

[![r/Superstonk - Live Charting for 4/7/2021, predicting the day's price action in detail with Warden.](https://preview.redd.it/7vgz2is3hrr61.png?width=2136&format=png&auto=webp&s=43eccea2ccf97c00ba3061f0f991b88e7c250c5b)](https://preview.redd.it/7vgz2is3hrr61.png?width=2136&format=png&auto=webp&s=43eccea2ccf97c00ba3061f0f991b88e7c250c5b)

Edit 6 10:20AM:

Nothing crazy in terms of options. 250k worth of 200 strike calls. They seem to have been sold on the bid.

[![r/Superstonk - Live Charting for 4/7/2021, predicting the day's price action in detail with Warden.](https://preview.redd.it/6wjf75h3grr61.png?width=2483&format=png&auto=webp&s=ab2ab74c6c0f24dae630079552d058f5ceddcd44)](https://preview.redd.it/6wjf75h3grr61.png?width=2483&format=png&auto=webp&s=ab2ab74c6c0f24dae630079552d058f5ceddcd44)

https://www.optionsonar.com/unusual-option-activity/GME/latest-trades

Edit 4 9:49AM:

The classic sideways arrow.

[![r/Superstonk - Live Charting for 4/7/2021, predicting the day's price action in detail with Warden.](https://preview.redd.it/cqf2cubjarr61.png?width=2126&format=png&auto=webp&s=417bf6e1a550f84c1016234af96d721f9b3383d7)](https://preview.redd.it/cqf2cubjarr61.png?width=2126&format=png&auto=webp&s=417bf6e1a550f84c1016234af96d721f9b3383d7)

Edit 3 9:42AM:

New support added at 180.5.

Edit 2 9:32AM:

First minute candle, around 250k volume in WeBull. It's shaping up to be a low volume day. Perhaps volume will kick back in during power hour.

Edit 1 9:28AM:

It's seriously trading like a penny stock, crazy low volume in premarket, sitting in the hundreds.

Begin reading here

[![r/Superstonk - Live Charting for 4/7/2021, predicting the day's price action in detail with Warden.](https://preview.redd.it/r1gd9eub6rr61.png?width=510&format=png&auto=webp&s=012cf555405e7c39f65e09f002df5ed0f13c7836)](https://preview.redd.it/r1gd9eub6rr61.png?width=510&format=png&auto=webp&s=012cf555405e7c39f65e09f002df5ed0f13c7836)

Gooooood morning my fellow apes!

It's certainly been very quiet yesterday. The lowest volume all week sitting at around 6 million. It's interesting to me that it's always on a Tuesday that we see some of the lowest volume trading days. On 2/24, a Wednesday, the stock exploded after a 7 million volume trading day.

Will we see some action today? Well let's find out.

I'll be streaming on <https://youtu.be/Vas9FymxdCk>.

Premarket analysis

No major gap up or down. We've just dropped to a lower support in the premarket. Broader market, S&P500, is also down in the premarket.

[![r/Superstonk - Live Charting for 4/7/2021, predicting the day's price action in detail with Warden.](https://preview.redd.it/ol6b25yd6rr61.png?width=2138&format=png&auto=webp&s=567a35bcb2f9af7ed3edd82b3ecfc3674e0df631)](https://preview.redd.it/ol6b25yd6rr61.png?width=2138&format=png&auto=webp&s=567a35bcb2f9af7ed3edd82b3ecfc3674e0df631)
