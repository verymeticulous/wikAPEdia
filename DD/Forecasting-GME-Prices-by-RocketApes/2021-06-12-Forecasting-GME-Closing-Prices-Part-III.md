GME price development decoded: A final update on GME price prediction
=====================================================================

| Author       | Source       | 
| :-------------: |:-------------:|
|  [u/RocketApes](https://www.reddit.com/user/RocketApes/) | [Reddit](https://www.reddit.com/r/DDintoGME/comments/nxyul2/gme_price_development_decoded_a_final_update_on/) | 

---

[𝘜𝘯𝘷𝘦𝘳𝘪𝘧𝘪𝘦𝘥 𝘋𝘋](https://www.reddit.com/r/DDintoGME/search?q=flair_name%3A%22%F0%9D%98%9C%F0%9D%98%AF%F0%9D%98%B7%F0%9D%98%A6%F0%9D%98%B3%F0%9D%98%AA%F0%9D%98%A7%F0%9D%98%AA%F0%9D%98%A6%F0%9D%98%A5%20%F0%9D%98%8B%F0%9D%98%8B%22&restrict_sr=1)

*edit2: You asked for pictures, I give you a picture:*

[![r/DDintoGME - GME price development decoded: A final update on GME price prediction](https://preview.redd.it/ygzikkivbv471.png?width=864&format=png&auto=webp&s=687ba1a0b09b08d5a6527e6e82248a2ac02ea1e6)](https://preview.redd.it/ygzikkivbv471.png?width=864&format=png&auto=webp&s=687ba1a0b09b08d5a6527e6e82248a2ac02ea1e6)

Variable influence. Bold area is 90% percentile. Variables not crossing the 0-line are significant, influence on GME price change in percent at x-axis. Example: VIXPD (Vix, previous day) has a positive and almost significant influence on GME price

*edit: Forgot to add, buy and hold. I am not a financial advisor or your mummy (say hello if you meet her!), but daytrading based on any of this stuff could be a very bad idea: Firstly, the model is not ALWAYS correct, secondly if only lasts for a day and who knows what is tomorrow. You could miss stuff like DFV returning or the MOASS. Just buy and hold, I'd say.*

tl;dr: I developed a very good model for GME price prediction (success rate > 90%) and found out by which factors the GME prices is moved. It is moved by FTD cylce, SI reporting, Beta values and MACD, maybe VIX, Options, Movie Theatres. It is NOT moved by cr*pto, longterm Beta, ETF FTD and the max pain price.

LAPEies and GAPElemen,

To complete the trilogy of GME price prediction posts which started [here](https://www.reddit.com/r/Superstonk/comments/noih5m/i_successfully_forecasted_gme_closing_prices_for/) and [here](https://www.reddit.com/r/Superstonk/comments/np9a0k/the_price_of_gme_since_february_is_completely/), I present the infamous third part: The final problem.

Didn't watch the first two movies and now getting on everyones nerves by asking what the story is about? Let me help you:

I developed a linear model to predict the price of GME after the first hour of premarket. I have been really successful with that. And now I improved it even further.

*Oh, and before you ask: No, I will not make predictions for each and every single day now. I will do something better: I will tell you which data you need to do it yourself and which theories on price influence are true - and which can mathematically be debunked.*

So, how good is your model, rocketGapes? Oh, glad you asked:

I could successfully predict the direction of movement in 97% of all cases in the extensive model (incl. FTD data until May) and 91% in the more up to date model until yesterday. The median error was about 3%.

R squared (where 1 is absolute perfect prediction and anything above roughly 0.4 is really good) is 0.65 for the up to date model and incredible 0.815 for the extensive model. So extremely good.

-   Question for the wrinkle brains: There were only two dates which none of the models could predict right: 2021/04/07 and 2021/04/16. Both should have been really good dates (strong upward movement) but the price moved down instead. *What happened on these dates?*

I will have a data section at the very bottom of the post where all the ANALysts can get extensive information on the models. The source code is available on my [github](https://github.com/rocketapes123/GMEmodel) and you can download the raw data [here](https://github.com/rocketapes123/GMEmodel/blob/main/LMGME_e.csv).

Alright, let us dig into the influential factors on GME price (important: These factors add up, they ALL need to be taken into consideration):

Factors of highest significance and importance

-   FTD-Cycle: Everyone talks about it and everyone is right: on the 21st day, statistically proven the shit hits the fan as hedgies try to kick the can down the road. But there is more:

    -   On day 2 and 3 as well as 12 and 13, the price declines quite often. Question for the wrinkle brains: Why could this be the case?

-   SI reporting: as the famous [/u/Criand](https://www.reddit.com/u/Criand/) found out [here](https://www.reddit.com/r/Superstonk/comments/nc1lny/ive_estimated_the_current_si_based_on_the_si/) and I could now prove, the price spikes up in the days previous to SI reporting days you can find [here](https://www.finra.org/filing-reporting/regulatory-filing-systems/short-interest). More specifically, the price explodes on one or both of the days prior to the SI reporting settlement days twice a month.

-   Movement in after hours and premarket: Not surprisingly, the direction of AH and first hour of PM is a big determinator of closing price

Factors of high significance and importance

-   Beta values: The beta values (how GME moves with the market) for various time periods (1W, 2W and 4W beta) have a big influence on the price as there seem to be cycles in which GME moves better or worse compared to the market in a predictable way (more wrinkle brains please interpret the numbers I provide below)

-   Previous Day movement of GME: Generally speaking, GME price movement uses to change direction quite often - the previous day price movement tends to inverse

-   First hour premarket volume: Interestingly, the volume of the first hour in PM has a big effect on the closing price: The higher the volume, the lower the closing price. Why? No idea :)

-   Earnings: Ok, I covered only two dated with earnings but the price decline on the after was so significant and unexplicable with other factors that this still shows up here

-   MACD: The value change of the daily MACD histogram (further explanation [here](https://www.investopedia.com/terms/m/macd.asp)) is another good price predictor. It has a positive sign, meaning: MACD moves up -> price tends to move up the next day. MACD moves down -> price tends to move down the next day

Factors which could very well play a role

-   Change of the Max Pain Price: The change of max pain price (call against put options) on the previous day has a positive correlation with the closing price of today: The price tends to reflect those changes, which only makes sense.

-   A certain theatre chain: The stock which may not be named not only has a big correlation to GME but also the closing prices of the previous day have a small, but interesting connection to today's GME price: It is negative, meaning: A::C moves up -> GME tends to move down the next day. Take it with a grain of salt, though.

-   VIX: Previous day VIX (measure of volatiliy in the market) correlates positively to today's GME closing prices: High VIX -> Better change of GME price rising

-   GME FTD: Failures to deliver of yesterday have a positive correlation to today's price: Many FTD's yesterdays -> Better change of GME price rising

-   RSI: RSI, a measure of whether a stock is over- or underbought, has a positive correlation to GME price

-   Ten year treasury yield: The change of yield of the 10Y treasury bond of the previous day, which is used as a significant indicator of stock market strength, has a negative correlation also to GME prices, so: Higher yield yesterday -> weaker GME price. Take it with a grain of salt though, the mathematical evidence is rather weak

Factors with little to no influence on GME price

-   Market movement (previous day): Yesterdays market movements almost have no influence on today's GME price

-   First hour movements of SPY and movie theater: Although there is some correlation between GME and movies / SPY, you cannot determine the development of today's price by looking at the first hour price movements of those two

-   Day of week: The day of the week has no real influence on prices. You could believe otherwise with weekly options and stuff, but no.

-   Difference of stock price to max pain price: This surprised me, but the difference of yesterdays stock price to the max pain price does not have an influence on the price (the direction of max pain movement price via options has, though). To me, this means that the theory, that the stock price always moves to the max pain price, is wrong. You might think so, because options are naturally playing around the current price but they dont determine it.

-   ETF FTDs: The failure to delivers of ETFs containing GME DONT have an influence on GME price.

-   B*C: As opposed to some of the theories here, the previous day B*C change does not have an influence on GME price. Maybe you find a relationship if you look at longer or shorter time periods, but I did not find indication that cr*pto currency sell offs lead to GME price spikes or anything.

-   What you know as beta: The longterm Beta which is calculated on weekly or monthly basis over more than a year and was hyped here because it was negative has no influence on GME price, sorry guys. GME generally moves with the market and if it doesn't, this has a reason.

Alright, this was long, sorry for that. But as a transparent community, I would like to have theories on price movement and influential factors proven. We see many theories around here, not all of them are true. Thanks for many smart apes, we can prove some and debunk others.

Model details

You find all the model details here: <https://github.com/rocketapes123/GMEmodel>

With a linear model, you can model a variable (in this case: GME price change to previous day in percent) as simple equation:

GME price change = Intercept + Estimate_a * Var_a + Estimate_b * Var_b.....

I have started with two models:

Model 1 including FTDs until mid of may:

```
ReturnGME~Sett+Volume1HPM+Return1H+FTD+Weekday+Beta.3M+Beta4W+Beta2W+Beta1W+B...C+MaxPain+RGME_PD+RA*C_PD+ReturnAMPD+TenYCPD+ReturnSPY+RSIPD+SP1H+A*C1H+MACDHISTPD+EarningsPD+VIXPD+mPlastPrice+GMEFTDPD+ETFFTDPD

```

Model 2 excluding FTDs until June 11:

```
ReturnGME~Sett+Volume1HPM+Return1H+FTD+Weekday+Beta.3M+Beta4W+Beta2W+Beta1W+B*C+MaxPain+RGME_PD+RA*C_PD+ReturnAMPD+TenYCPD+ReturnSPY+RSIPD+SP1H+A*C1H+MACDHISTPD+EarningsPD+VIXPD+mPlastPrice+GMEFTDPD+ETFFTDPD

```

With stepwise elimination of variables, I reduced the model to the relevant variables:

Model 1 compressed:

```
ReturnGME ~ Sett + Volume1HPM + Return1H + FTD +  Beta4W + Beta2W + Beta1W + MaxPain + RGME_PD + ReturnAMPD + A...C1H + MACDHISTPD + EarningsPD + VIXPD + GMEFTDPD

```

Model 2 compressed:

```
ReturnGME ~ Sett + Volume1HPM + Return1H + FTD + Beta4W + Beta2W + Beta1W + B*C + RGME_PD + RA...C_PD + ReturnAMPD + TenYCPD + RSIPD + MACDHISTPD + EarningsPD + VIXPD

```

Results of the models:

Model 1 compressed:

```
Call:
lm(formula = ReturnGME ~ Sett + Volume1HPM + Return1H + FTD +
    Beta4W + Beta2W + Beta1W + MaxPain + RGME_PD + ReturnAMPD +
    A*C1H + MACDHISTPD + EarningsPD + VIXPD + GMEFTDPD, data = data)

Residuals:
    Min      1Q  Median      3Q     Max
-13.064  -3.617   0.000   3.296  14.404

Coefficients:
              Estimate Std. Error t value Pr(>|t|)
(Intercept) -1.089e+01  1.191e+01  -0.914 0.367437
Sett1        3.641e+01  5.779e+00   6.301 4.55e-07 ***
Volume1HPM  -6.383e-05  3.034e-05  -2.104 0.043350 *
Return1H     2.631e+00  4.183e-01   6.290 4.70e-07 ***
FTD2        -5.024e+01  1.064e+01  -4.721 4.46e-05 ***
FTD3        -4.474e+01  1.114e+01  -4.015 0.000335 ***
FTD4        -1.962e+01  8.175e+00  -2.400 0.022407 *
FTD5        -1.564e+01  8.444e+00  -1.853 0.073182 .
FTD6        -1.196e+01  8.441e+00  -1.417 0.166289
FTD7        -9.609e+00  8.527e+00  -1.127 0.268163
FTD8        -1.017e+01  8.360e+00  -1.217 0.232590
FTD9        -1.074e+01  8.348e+00  -1.287 0.207281
FTD10       -2.731e+01  8.155e+00  -3.350 0.002085 **
FTD11       -1.871e+01  9.679e+00  -1.933 0.062089 .
FTD12       -4.335e+01  1.045e+01  -4.148 0.000231 ***
FTD13       -4.216e+01  9.586e+00  -4.398 0.000113 ***
FTD14       -1.123e+01  7.802e+00  -1.440 0.159666
FTD15       -7.598e+00  8.420e+00  -0.902 0.373609
FTD16       -1.371e+01  8.580e+00  -1.598 0.119820
FTD17       -1.423e+01  8.278e+00  -1.719 0.095223 .
FTD18       -1.588e+01  8.637e+00  -1.838 0.075329 .
FTD19       -1.373e+01  8.509e+00  -1.613 0.116579
FTD20       -9.808e+00  8.535e+00  -1.149 0.259011
FTD21        1.911e+01  9.799e+00   1.950 0.059921 .
Beta4W      -3.992e-01  1.729e-01  -2.310 0.027517 *
Beta2W       5.655e-01  2.330e-01   2.427 0.021019 *
Beta1W      -3.329e-01  1.616e-01  -2.060 0.047609 *
MaxPain      2.792e-01  1.635e-01   1.707 0.097437 .
RGME_PD     -5.448e-01  1.530e-01  -3.561 0.001181 **
ReturnAMPD   1.397e+00  3.667e-01   3.810 0.000595 ***
A*C1H       -7.257e-01  4.269e-01  -1.700 0.098876 .
MACDHISTPD   2.140e+00  6.889e-01   3.107 0.003948 **
EarningsPD  -2.731e+01  1.160e+01  -2.355 0.024824 *
VIXPD        9.884e-01  5.047e-01   1.958 0.058947 .
GMEFTDPD     6.550e-05  3.731e-05   1.756 0.088738 .
---
Signif. codes:  0 '***' 0.001 '**' 0.01 '*' 0.05 '.' 0.1 ' ' 1

Residual standard error: 7.413 on 32 degrees of freedom
Multiple R-squared:  0.9103,	Adjusted R-squared:  0.8149
F-statistic: 9.548 on 34 and 32 DF,  p-value: 2.596e-09

```

Model 2 compressed:

```
Call:
lm(formula = ReturnGME ~ Sett + Volume1HPM + Return1H + FTD +
    Beta4W + Beta2W + Beta1W + B*C + RGME_PD + RA*C_PD + ReturnAMPD +
    TenYCPD + RSIPD + MACDHISTPD + EarningsPD + VIXPD, data = data)

Residuals:
     Min       1Q   Median       3Q      Max
-16.6535  -4.4684  -0.6397   4.4523  25.7623

Coefficients:
              Estimate Std. Error t value Pr(>|t|)
(Intercept) -4.074e+01  1.598e+01  -2.549 0.013989 *
Sett1        1.565e+01  5.028e+00   3.113 0.003088 **
Volume1HPM  -8.234e-05  3.577e-05  -2.302 0.025637 *
Return1H     2.007e+00  5.069e-01   3.959 0.000243 ***
FTD2        -5.185e+00  1.013e+01  -0.512 0.611216
FTD3        -1.211e+01  8.966e+00  -1.350 0.183168
FTD4         5.329e+00  8.798e+00   0.606 0.547468
FTD5        -1.206e+00  8.464e+00  -0.142 0.887296
FTD6         1.198e+00  8.737e+00   0.137 0.891454
FTD7         8.505e-02  9.220e+00   0.009 0.992677
FTD8         1.327e+01  8.470e+00   1.566 0.123737
FTD9         7.258e+00  8.522e+00   0.852 0.398582
FTD10       -1.385e+01  8.327e+00  -1.663 0.102749
FTD11       -1.024e-14  9.909e+00   0.000 1.000000
FTD12       -7.953e+00  9.406e+00  -0.845 0.401959
FTD13       -5.410e+00  9.009e+00  -0.600 0.550974
FTD14        9.777e-15  8.865e+00   0.000 1.000000
FTD15        1.063e+01  8.958e+00   1.187 0.240998
FTD16        2.623e+00  8.929e+00   0.294 0.770202
FTD17       -7.713e+00  8.858e+00  -0.871 0.388130
FTD18       -1.733e+00  9.249e+00  -0.187 0.852146
FTD19        2.827e+00  8.567e+00   0.330 0.742814
FTD20       -1.729e-14  9.230e+00   0.000 1.000000
FTD21        1.948e+01  9.232e+00   2.110 0.039948 *
Beta4W      -1.007e-01  2.195e-01  -0.459 0.648532
Beta2W       2.997e-01  2.478e-01   1.210 0.232146
Beta1W      -1.873e-01  1.625e-01  -1.153 0.254594
B*C         -1.793e-01  2.701e-01  -0.664 0.509813
RGME_PD     -1.556e-01  1.817e-01  -0.856 0.395913
RA*C_PD     -1.865e-01  1.094e-01  -1.705 0.094556 .
ReturnAMPD   1.772e+00  4.559e-01   3.887 0.000305 ***
TenYCPD     -5.988e-01  3.491e-01  -1.715 0.092623 .
RSIPD        3.419e-01  1.802e-01   1.897 0.063783 .
MACDHISTPD   1.959e+00  8.426e-01   2.325 0.024262 *
EarningsPD  -1.611e+01  9.099e+00  -1.770 0.082947 .
VIXPD        1.049e+00  6.372e-01   1.646 0.106149
---
Signif. codes:  0 '***' 0.001 '**' 0.01 '*' 0.05 '.' 0.1 ' ' 1

Residual standard error: 9.569 on 49 degrees of freedom
Multiple R-squared:  0.7932,	Adjusted R-squared:  0.6455
F-statistic:  5.37 on 35 and 49 DF,  p-value: 5.649e-08
```
