Delta/Gamma Update & The Role of a Critic
=========================================

| Author       | Source       | 
| :-------------: |:-------------:|
|  [u/yelyah2](https://www.reddit.com/user/yelyah2/) | [Reddit](https://www.reddit.com/r/Superstonk/comments/nzyji4/deltagamma_update_the_role_of_a_critic/) | 

---

[Education 👨‍🏫 | Data 🔢](https://www.reddit.com/r/Superstonk/search?q=flair_name%3A%22Education%20%F0%9F%91%A8%E2%80%8D%F0%9F%8F%AB%20%7C%20Data%20%F0%9F%94%A2%22&restrict_sr=1)

*Graph Update*

Here's the graph you're used to seeing, and it includes the Close Price (green), delta neutral (blue), gamma neutral (orange), and max pain (light blue) .

[![r/Superstonk - Delta/Gamma Update & The Role of a Critic](https://preview.redd.it/97mi0v0sxa571.png?width=910&format=png&auto=webp&s=c3ca835309cae2a0f9c3a22534de8d98f3f94cec)](https://preview.redd.it/97mi0v0sxa571.png?width=910&format=png&auto=webp&s=c3ca835309cae2a0f9c3a22534de8d98f3f94cec)

GME 1/4/2021 - 6/14/2021 - Log Base 10 Scale

I'm really excited to share that I bought a massive options database, with all optionable stocks going back to 2007! I'm in the process of transitioning my code over to this new vendor, making some enhancements to the model I've been wanting to do, and running the algo. I'm Excited to see how my indicators work on prior short squeezes (like the VW squeeze). I look forward to sharing my research!

My work is built on the idea that the market is largely unpredictable, but one particular kind of behavior is certain - hedgies gonna hedge. It's written into their algorithms. Specifically, they like to delta hedge and gamma hedge. This work tries to profit on this one particular type of buying/selling behavior. I have a little data dictionary at the bottom if you need a refresher on terminology.

There isn't a lot to note today for these specific indicators, but wanted to give you an updated. Instead, I just have something to say to support my amazing, fellow DD/TA friends that are putting out incredible new ideas.

*Quick Chat*

I think like we may need to have a little chat. I say it at the bottom of each post, but these indicators just help give help identifying if the probability of a certain event occurring has increased. None of my fellow DD/TA'ers are giving you prophecies. There are too many variables to incorporate, and the human element, which makes it impossible to tell you any price movement is 100% certain.

Similarly, sports analysts put a lot of work incorporating all kinds of factors into the chance a certain team winning a game, and incorporate all kinds of factors (weather, injuries, home field advantage, etc.). However, any team can win on Any Given Sunday.

For example, every analyst predicted the 7-9 Seahawks would lose to the 11-5 Saints in the 2010 NFC Wild Card Game, but none of them realized the secret was that Marshawn Lynch ate his special skittles, and resulted in Beast Quake (best running touch down ever).

[![r/Superstonk - Delta/Gamma Update & The Role of a Critic](https://preview.redd.it/akg7mts0za571.png?width=1000&format=png&auto=webp&s=c3ea9c4b163e260867e450596d9b99786124aa78)](https://preview.redd.it/akg7mts0za571.png?width=1000&format=png&auto=webp&s=c3ea9c4b163e260867e450596d9b99786124aa78)

2010 Beast Quake

Now I could start predicting with some certainty that when Marshawn Lynch ate his special skittles, the Seahawks would win. That would work with some certainty, and my success rate in using that indicator was higher than with other factors (or maybe in addition to those other factors).

Now say that I knew Marshawn Lynch had extra special Skittles before Super Bowl XLIX, so I knew the chances were much higher that the Seahawks would win, and Marshawn Lynch was ready to run in the game winning touchdown.

HOWEVER, no one could have expected that fricking PETE CARROL WOULD DECIDE TO PASS IT INSTEAD OF GIVING IT TO SKITTLE-MUCHING-MARSHAWN AT THE ENDZONE FOR THE GAME-WINNING PLAY.

[![r/Superstonk - Delta/Gamma Update & The Role of a Critic](https://preview.redd.it/ueou8kpa0b571.png?width=1024&format=png&auto=webp&s=c3036caf38c54c56a7c45690aade6a312773e624)](https://preview.redd.it/ueou8kpa0b571.png?width=1024&format=png&auto=webp&s=c3036caf38c54c56a7c45690aade6a312773e624)

Super Bowl XLIX - Heartbreak

So does that mean I was wrong about using special Skittles as a helpful indicator for a Seahawks win? No! Because the human-element (i.e. stupid Seahawks coaches) adds unpredictability. I won't ditch that indicator, but will work to refine that indicator or use it in conjunction with others.

We're all working to improve and become more accurate, so be kind if you think a DD/TA wasn't perfect for the day. Ape no fight Ape. I support every one of my incredibly smart, new, GME friends that are putting out new ideas.

So I will just leave you with some Ratatouille to think on as you read through posts this evening:

[![r/Superstonk - Delta/Gamma Update & The Role of a Critic](https://preview.redd.it/cwb4c7fb1b571.png?width=530&format=png&auto=webp&s=d028013629530a4e1ed0f585bb56677e600cfae1)](https://preview.redd.it/cwb4c7fb1b571.png?width=530&format=png&auto=webp&s=d028013629530a4e1ed0f585bb56677e600cfae1)

Ratatouille - The Role of a Critic

*Data Dictionary*

-   Delta Neutral: price that creates a total market delta of 0 across all GME options (all expiration dates) for a given date. General observation is it acts like a theoretical floor (although the price can go lower, as seen in February). My theory is that as the underlying approaches the delta neutral, call options go on sale. As people buy call options, MM have to buy the stocks which increases the price. Most stocks like to hang out above the delta neutral, some dip below and create pressure that can shoot them back over the delta neutral (like what happened in February), and some like to hang out below (like the VIX).

-   Gamma Neutral: price that creates a total market gamma of 0 across all GME options (all expiration dates) for a given date. General observation is it acts like support/resistance between the delta neutral and the underlying, and typically bounces around between the two prices for most plan (like we have seen with GME since April). It also goes crazy in periods of high volatility (as you can see by the infinite spikes).

-   Max Pain: price that creates largest loss for option buyers and largest gain for option sellers. This is a controversial topic because underlying prices can drift towards this point. There are typically large areas around the max pain that doesn't make a lot of difference to the profits for option buyer/sellers. It can be used to help gauge where the equilibrium of the options data is, but there is often a wide range around this price point that does not meaningfully affect MM profits.

Disclaimer: I'm just a person that likes to play with options data and builds models to trade for a hobby. I have no experience trading professionally or offering any advice to anyone. Nothing is certain in trading. It's all probabilities and what increases/decreases your chance at a profit. This is just one indicator for one type of price movement, and there are many other indicators that can help you make investment decisions.
