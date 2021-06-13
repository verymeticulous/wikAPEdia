I successfully forecasted GME closing prices for the last two weeks based on your DD (proof included). Can therefore prove FTD and SI DD and that Hediges haven't started covering big time. Want me to share the model?
========================================================================================================================================================================================================================

| Author       | Source       | 
| :-------------: |:-------------:|
|  [u/RocketApes](https://www.reddit.com/user/RocketApes/) | [Reddit](https://www.reddit.com/r/Superstonk/comments/noih5m/i_successfully_forecasted_gme_closing_prices_for/) | 

---

[Education 👨‍🏫 | Data 🔢](https://www.reddit.com/r/Superstonk/search?q=flair_name%3A%22Education%20%F0%9F%91%A8%E2%80%8D%F0%9F%8F%AB%20%7C%20Data%20%F0%9F%94%A2%22&restrict_sr=1)

*edit2: Fixed broken links.*

*edit1: Formatting. Proof for successful predictions now better visible.*

Hi to all the apes out there,

I do data stuff for a living and since I basically spend my work hours staring at green and red GME dildos since January I thought:

*"Why not try to predict GME movement for today?"*

So I did. And it worked, I predicted the general movement of the last two weeks including last weeks crazy price action pretty accurately. That is why I am accused of witchcraft in the German Sub where I published my forecasts ;)

Don't believe me? Neither would I. But I will deliver proof.

*Before I start: I am a data scientist, but not financial expert or advisor. Don't base investments on anything you see here, a model can always fail. If you really want, I can be your wifes boyfriend, though.*

That is how it looks:

[![r/Superstonk - I successfully forecasted GME closing prices for the last two weeks based on your DD (proof included). Can therefore prove FTD and SI DD and that Hediges haven't started covering big time. Want me to share the model?](https://preview.redd.it/3ce2pe9p6b271.png?width=913&format=png&auto=webp&s=562b5bccbd0ed527e0f87aebab74f61eccd747fa)](https://preview.redd.it/3ce2pe9p6b271.png?width=913&format=png&auto=webp&s=562b5bccbd0ed527e0f87aebab74f61eccd747fa)

GME price vs. my forecast

Want proof? Alright, the forecasts where announced in the German *Unter* [r/spielstopp](https://www.reddit.com/r/spielstopp/) in the following posts or comments (model was improved over time, old descriptions are not up to date):

| Date | Forecast | Link / Proof |
| --- | --- | --- |
| 2020-05-17 | 5 to 7.5% | [Here](https://www.reddit.com/r/Spielstopp/comments/ne9vhn/neues_kursmodell_zur_vorhersage_f%C3%BCr_euch_zum/) |
| 2020-05-18 | -6 to -9% | [Here](https://www.reddit.com/r/Spielstopp/comments/nf4mgo/kursmodell_20_und_offenlegung_von_daten_und_modell/) |
| 2020-05-19 | -5 to -8% | [Here](https://www.reddit.com/r/Spielstopp/comments/nfz5x7/ich_habe_euch_entt%C3%A4uscht_gebt_mir_noch_ne_chance/) |
| 2020-05-20 | 0 to 2.5% (Model 1) | [Here](https://www.reddit.com/r/Spielstopp/comments/ngoyj4/t%C3%A4glicher_spielstopp_sammelfaden_20052021/gysw3ug?utm_source=share&utm_medium=web2x&context=3) |
| 2020-05-21 | 2.5 to 5% (Model 2) | [Here](https://www.reddit.com/r/Spielstopp/comments/nhihrz/t%C3%A4glicher_spielstopp_sammelfaden_21052021/gyx9xad?utm_source=share&utm_medium=web2x&context=3) |
| 2020-05-24 to 2020-05-28 (whole week because I was on vacation) | Longterm forecast (NOT up to date) | [Here](https://www.reddit.com/r/Spielstopp/comments/ngyrai/langfristige_kursvorhersage_von_spielstopp/) |

*Alright, what did I do? (You can skip this part if you like)*

I developed a relatively simple linear regression model and optimized it with a little Monte-Carlo-Simulation to improve the forecast. R² is 0.62, overfitting was hopefully countered by stepwise reduction of variables.

I am sure there are smart apes out there who could improve the model by adding non-linear regression terms, time series analysis and so on, but I had no time for that yet ;) If I chose to share my model, I would be happy to assist with improvements.

*Why should I care? I am just an ape who buy and holds? (DONT skip this part!)*

I will tell you why! Because I can proof some DDs floating around here right.And, most importantly, the fact that GME price movements especially in this week were predictable, shows that we are still in the "Hedgie manipulated area", no covering of shorts or crazy staff has yet happened!

What variables did I include in my model (bold ones are of greater significance)?

1.  Volume und Price movements of afterhours previous day and first hour of the premarket (prediction for the day is therefore available at 5am EST or 10am my time ;))

2.  FTD cycle. Hell yeah, this one IS important, we saw that last week. Hank and all the other's theories seem to be right

3.  Day of week (NOT that important, also no special movements on fridays (options) or tuesday (option hedging) to be seen)

4.  SPY movement (previous day)

5.  Price movement of 10Y US treasuries

6.  Price movement B...Coin (previous day)

7.  Price movement of a certain Cinema (previous day). Not that important as a predictor but of course still correlated to GME!

8.  Change in max pain price (not that important either)

9.  Did RC tweet (previous day)? For the lulz, also not that important

10. RSI (Relative strength index) at the end of previous day

11. 3 month, 4 week, 2 week and 1 week beta. VERY relevant and, to be clear, betas are POSITIVE most of the time

12. SI settlement dates as described in [this](https://www.reddit.com/r/Superstonk/comments/nc1lny/ive_estimated_the_current_si_based_on_the_si/) DD are extremely relevant

(So why did the price go up this week? in simple terms: FTD+21 plus SI settlement dates plus a little FOMO)

You can find more explanation at my github: <https://github.com/rocketapes123/GMEmodel> or in a little pastebin: <https://controlc.com/9e895bdb>

I set the project to private temporarily, though. Why? Read on.

*Ok, now to the most important question? Should I publish the model and / or forecasts? To be clear, I don't want to farm karma, I am not going to monetize, stream, ask for funding or similar bullshit. I just want to share my findings.*

Whats stops me from doing it? What are my doubts?

1.  Hedgies can read this, too. My model shows that DD here is on spot. (Counter argument: They not it anyways)

2.  A model is a model. It can be wrong, there can be new factors, fuckery or FOMO it can not predict. If people rely on it too much, a wrong prediction could spread doubt.

3.  Danger of "self-fulfilling prophecy": If I, lets say, predict that price is going to drop 5% tomorrow, some people may sell their shares and accelerate a decline

What do you say? Mods and wrinkly apes, I need your input:

[u/rensole](https://www.reddit.com/u/rensole/)**,** [u/redchessqueen99](https://www.reddit.com/u/redchessqueen99/)**,** [u/dlauer](https://www.reddit.com/u/dlauer/)**,** [u/atobitt](https://www.reddit.com/u/atobitt/)
