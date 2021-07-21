6/6/2021 Gamma Update - Review of Gamma Maximums
================================================

| Author       | Source       | 
| :-------------: |:-------------:|
|  [u/yelyah2](https://www.reddit.com/user/yelyah2/) | [Reddit](https://www.reddit.com/r/Superstonk/comments/ntw1h1/662021_gamma_update_review_of_gamma_maximums/) | 

---

[Education 👨‍🏫 | Data 🔢](https://www.reddit.com/r/Superstonk/search?q=flair_name%3A%22Education%20%F0%9F%91%A8%E2%80%8D%F0%9F%8F%AB%20%7C%20Data%20%F0%9F%94%A2%22&restrict_sr=1)

TLDR: Potential new indicator - Gamma Maximum prices could identify potential ceilings for an underlying price, and a threshold to catapult the stock upwards if it can break through.

Few Quick Words

As my posts have recently gained some attention, thought I'd like say a few quick things before digging in:

-   I use raw options data from [historicaloptiondata.com](https://historicaloptiondata.com/), write my own algos, and these are just Excel graphs I made.

-   I have a few motivations for sharing this information:

    -   Give back to this community. It's awesome, and has given me so much knowledge already.

    -   Get feedback and suggestions. I do this as a hobby. I'm not a professional, and this is a pool of very intelligent people who have a lot of good ideas. This post is dedicated to one suggestion I received this last week, and was excited to dig into. I appreciate all your comments and suggestions.

        -   Just be kind if you see something you don't agree with. I'd love an honest discourse!

-   I try to read/reply to all your comments, messages and chats. If I don't respond and you wanted a chat, just bug me again. Like everyone, I have a lot going on in life, but this is important to me.

-   I'm giving away a lot of my sauce, but I choose to keep some of my sauce secret. Hoping you can understand if I don't give away all secrets of what I do with trading this model.

Recap

My work is built on the idea that the market is largely unpredictable, but one particular kind of behavior is certain - hedgies like to hedge. It's written into their algorithms. Specifically, they like to delta hedge and gamma hedge. This work tries to profit on this one particular type of buying/selling behavior. I have a little data dictionary at the bottom if you need a refresher on terminology.

Usual Graph Update

Here's the graph you're used to seeing, and it includes the Close Price (green), delta neutral (blue), gamma neutral (orange) and max pain (blue).

[![r/Superstonk - 6/6/2021 Gamma Update - Review of Gamma Maximums](https://preview.redd.it/4lrpvevj5p371.png?width=910&format=png&auto=webp&s=7d8a66d7133074756b822614a74b5389553390e3)](https://preview.redd.it/4lrpvevj5p371.png?width=910&format=png&auto=webp&s=7d8a66d7133074756b822614a74b5389553390e3)

GME 12/3/2020 - 6/4/2021

And on a log-based 10 scale:

[![r/Superstonk - 6/6/2021 Gamma Update - Review of Gamma Maximums](https://preview.redd.it/w8hji3wc5p371.png?width=910&format=png&auto=webp&s=e6f2d7ff15bb04826059d30df5e473bef9998ff7)](https://preview.redd.it/w8hji3wc5p371.png?width=910&format=png&auto=webp&s=e6f2d7ff15bb04826059d30df5e473bef9998ff7)

GME 12/3/2020 - 6/4/2021 - Log Base 10 Scale

Some people are expecting another drop as the GME price climbs up. The Delta Neutral was at $164 on Friday, and I am projecting that it will climb to $168 by tomorrow, so if the price does dump, don't panic!

Gamma Maximum

As I said, I try to read/reply to all your comments and appreciate all feedback/ideas. For this post, I want to highlight one idea by [u/pennyether](https://www.reddit.com/u/pennyether/):

*"I have a hunch that the price point that has "peak gamma" is more predictive than the point that has "zero gamma". I would be very interested to "peak gamma price point" plotted with the other values.*

*I think "zero gamma" is overall just indicative of call/put ratio, and how far out they are. It's more of a measurement of "how much are people gambling?".*

*"Peak Gamma" acts more like magnet in some respects. It's easier to move the price around through price points of high gamma (since each buy or sell is magnified by delta hedging). So if you're just below the peak, buying will push you up slightly more than selling will push you down.*

Before I show you GME, I wanted to show you the Amazon graph with the "Max Gamma", in a nice red crayon color, and represents underlying price that would achieve the maximum total gamma for the day. I picked Amazon because it's a stock that behaves really well, it has some of the highest underlying equity and options volume on the stock market.

[![r/Superstonk - 6/6/2021 Gamma Update - Review of Gamma Maximums](https://preview.redd.it/rtcns36a7p371.png?width=910&format=png&auto=webp&s=43fa5f0686002248a5e11f018a4eaf02c096ae87)](https://preview.redd.it/rtcns36a7p371.png?width=910&format=png&auto=webp&s=43fa5f0686002248a5e11f018a4eaf02c096ae87)

AMZN 12/1/2020 - 6/4/2021

A couple quick comments:

-   For Amazon, it does seem like the gamma maximum could be acting like a magnet, as [u/pennyether](https://www.reddit.com/u/pennyether/) suggested.

-   It also seems to act like a ceiling for Amazon on a couple points

So with that here's the GME graph, in all its madness:

[![r/Superstonk - 6/6/2021 Gamma Update - Review of Gamma Maximums](https://preview.redd.it/tamz8rn28p371.png?width=910&format=png&auto=webp&s=ead72bace85cb8bc461acf3292186c10ee5c5274)](https://preview.redd.it/tamz8rn28p371.png?width=910&format=png&auto=webp&s=ead72bace85cb8bc461acf3292186c10ee5c5274)

GME 12/3/2020 - 6/4/2021

I also zoomed in so you could see the run-up to the January squeeze:

[![r/Superstonk - 6/6/2021 Gamma Update - Review of Gamma Maximums](https://preview.redd.it/3a3gy4kb8p371.png?width=910&format=png&auto=webp&s=78f250da0d58caa3a196a6e75f48ad2f9f31604b)](https://preview.redd.it/3a3gy4kb8p371.png?width=910&format=png&auto=webp&s=78f250da0d58caa3a196a6e75f48ad2f9f31604b)

GME 12/3/2020 - 1/24/2021

I'm really interested to hear about what you see here, and what you think the maximum gamma could represent. I have a few thoughts/observations:

-   It does seem like the gamma max could act like a ceiling, as I showed with Amazon

-   but if the price breaks through the gamma maximum barrier, then it seems like it gives it the power to accelerate the underlying price upwards

-   If so, does that mean the ceiling tomorrow is ~$280 that we have to break through to get to the next level? Maybe? It definitely seems like the latest battles have been centered around $280. Here's hoping we can break through it!

Just for fun, here's a logarithmic scale showing the maximum gamma from the January squeeze. As you can see, the gamma maximum would have been $12,270,857,810,209,300,000,000,000,000,000 on 1/28/2021.

[![r/Superstonk - 6/6/2021 Gamma Update - Review of Gamma Maximums](https://preview.redd.it/kxbmw9gq5l371.png?width=910&format=png&auto=webp&s=4b2f236f63e054d5cb07ccd5d7901929ca008c31)](https://preview.redd.it/kxbmw9gq5l371.png?width=910&format=png&auto=webp&s=4b2f236f63e054d5cb07ccd5d7901929ca008c31)

Do I think that was really the ceiling? No.... not really... but I have a feeling some will say it's the new "floor" :) I'm guessing it's an infinite glitch as the optimizer tries to find a solution (I know you love that "g" word...).

Ok that's it for today, see you out there tomorrow! Keep your ideas coming! I love looking at this stuff!!

*Data Dictionary*

-   Delta Neutral: price that creates a total market delta of 0 across all GME options (all expiration dates) for a given date. General observation is it acts like a theoretical floor (although the price can go lower, as seen in February). My theory is that as the underlying approaches the delta neutral, call options go on sale. As people buy call options, MM have to buy the stocks which increases the price. Most stocks like to hang out above the delta neutral, some dip below and create pressure that can shoot them back over the delta neutral (like what happened in February), and some like to hang out below (like the VIX).

-   Gamma Neutral: price that creates a total market gamma of 0 across all GME options (all expiration dates) for a given date. General observation is it acts like support/resistance between the delta neutral and the underlying, and typically bounces around between the two prices for most plan (like we have seen with GME since April). It also goes crazy in periods of high volatility (as you can see by the infinite spikes).

-   Max Pain: price that creates largest loss for option buyers and largest gain for option sellers. This is a controversial topic because underlying prices can drift towards this point. There are typically large areas around the max pain that doesn't make a lot of difference to the profits for option buyer/sellers. It can be used to help gauge where the equilibrium of the options data is, but there is often a wide range around this price point that does not meaningfully affect MM profits.

Disclaimer: I'm just a person that likes to play with options data and builds models to trade for a hobby. I have no experience trading professionally or offering any advice to anyone. Nothing is certain in trading. It's all probabilities and what increases/decreases your chance at a profit. This is just one indicator for one type of price movement, and there are many other indicators that can help you make investment decisions.
