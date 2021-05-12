Hoping some research that I put a lot of time and effort into can make it through the drama. I've spent the past couple weeks collecting and analyzing data on off-exchange short volume, and wanted to share a write-up on my findings.
========================================================================================================================================================================================================================================

| Author       | Source       | 
| :-------------: |:-------------:|
|  [u/pdwp90](https://www.reddit.com/user/pdwp90/) | [Reddit](https://www.reddit.com/r/GME/comments/mkq470/hoping_some_research_that_i_put_a_lot_of_time_and/) | 

---


OC[DD 📊](https://www.reddit.com/r/GME/search?q=flair_name%3A%22DD%20%F0%9F%93%8A%22&restrict_sr=1)

This write-up relies heavily upon data used in [this dashboard](https://www.quiverquant.com/offexchange/gme) I've been building that visualizes daily data from this FINRA, and tracks cumulative off-exchange short sales over the last 5 years. If you're more of a crayon learner than a word learner, I'd start there.

Introduction

In the wake of the Financial Crisis in the late 2000s, many financial regulation disclosures were adopted in an effort to make financial institutions more transparent. One notable new publication was FINRA's daily Short Sale Volume Report, which was first shared with the public in 2009 following an SEC request. Unfortunately, the contents of these reports is so misconstrued by individuals that FINRA has had to issue [several notices](https://i2.t.hubspotemail.net/e2t/tc/VVPKbm4vwXt-N3m0wnGrFLB3W1RGk9h4q1lGqN3ypqFD3lGn5V1-WJV7CgJsxW50y38W4Zz9jKW3x2B_b89P5f5W4Z77yG7q8RCkW2vDf1f4TvlMLW18z82F7FmrKXW52_hxB5KpQ3cW4KK3D38xrpxPW1t5r-H2LD6gXW2xqgZy224NdlW5yP3612bdxtBW6N1z6K2_N4FZW9bT4j61dk0F2W88ccnP6KBZWlW17GNzS6Mh7_QW5CB7cL5b-YMXW6bCnxm1M1WP5W281Lyl1ZvDwzW564mPG8Q03HnW345gfw4GwdVMW6CwDBx1SzxZZVHdYHz1r56-ZW6kGK1x70PsP7W8Qy2sf7PRFGQW5ZbSGg67hTDP32Rt1) clarifying the data. 

Motivated by this, I'm going to explain why the data is misunderstood, and how to accurately interpret the data to help guide investment decisions.

[![r/GME - Hoping some research that I put a lot of time and effort into can make it through the drama. I've spent the past couple weeks collecting and analyzing data on off-exchange short volume, and wanted to share a write-up on my findings.](https://preview.redd.it/efvand30wdr61.png?width=1401&format=png&auto=webp&s=d8b8fd41f4618e5fcbf3babfc1af396e3e018614)](https://preview.redd.it/efvand30wdr61.png?width=1401&format=png&auto=webp&s=d8b8fd41f4618e5fcbf3babfc1af396e3e018614)

Off-Exchange Short Volume Activity - 04/01/2021

Daily Short Volume Vs. Bi-Monthly Short Interest

One area of confusion is the distinction between FINRA's daily short volume data and the bi-monthly short interest data they require companies to report. Let's start by clarifying the difference between FINRA's reports using their own definitions: 

-   Short Sale Volume Report: The Daily Short Sale Volume Files provide aggregated volume by security for all short sale trades executed and reported to the ADF during normal market hours. (Finra.org. 2021)

-   Short Interest Report: FINRA requires firms to report short interest positions in all customer and proprietary accounts in all equity securities twice a month. This data reflects all outstanding short positions held by market participants at a specific moment in time on two discrete days each month (Finra.org. 2021)

High transaction volume in the daily reports will not necessarily equate to a large outstanding short position. For example, if a firm sells short 1,000 shares of security ABCD, then purchases 1,000 shares of ABCD later the same day, the short sale volume in the Daily Report will include the 1,000 shares that were sold short. Because the firm sold short and purchased an equivalent number of shares that day, it did not establish or accumulate a short position in ABCD; thus, its short sale has no impact on the reported short interest in ABCD.

Here are two more things to note when interpreting the number from the daily report:

1.  The Daily Report only accounts for OTC exchange transactions or "Off-Exchanges" which is 30% of total market activity, resulting in lower share numbers than the total volume for a given ticker. 

2.  Off-exchange transactions are predominantly used by Market Makers (MM) to fill orders. Let's consider for instance that you place an order to buy one share of ABC stock for $10. To facilitate the transaction, a MM sells you the stock for $10 which it doesn't have.  As a result, the MM sells the share short and passes the share to you. Then the order goes through as a 'Short' on record. Conversely, if you were to sell your share of ABC stock, it would be reported as a 'Long'.

Market Makers make a profit from the spread between the bid and ask prices, typically covering the short sale immediately after the transaction. This results in a "short sale" which can be misleading to investors, because it's actually indicative of buying activity. These reported short sales are typically not the result of long-term speculative bets being taken against a given company.

DPI Ratio

Finally, the DPI ratio is used to determine the relative buying and selling activity for stocks on the Daily Report. Here's an example:

```
Shares Short = 70,000
Total OTC Volume = 100,000
DPI = 70,000/100,000 = .7

```

Remembering that 'Shares Short' is often the number of shares bought by non-MMs, and based on the example above, we can assume that a company with a DPI of 0.70 equates to high non-MM buying interest in the given company.

Armed with this new information: Does off-exchange activity have predictive power on future price movements? 

Study & Findings

To answer this question, I gathered 400,000+ data points pertaining to 5,041 stocks listed on the NYSE, honing in on the DPI and intraday performance averaged weekly for 2021 (YTD).

For the initial analysis, I segmented the 5,041 stocks into 3: The S&P500 to account for DPI effect on large-cap stocks, the top trending stocks on WallStreetBets in 2021 to gauge the forums relationship with DPI, and lastly the remaining stocks on the NYSE excluding companies in the two aforementioned groups. Subsequently, I divided them further based on the DPI ratio being less or >.50, to determine if there is a correlation between the DPI ratio and performance, with the results accounted below:

[![r/GME - Hoping some research that I put a lot of time and effort into can make it through the drama. I've spent the past couple weeks collecting and analyzing data on off-exchange short volume, and wanted to share a write-up on my findings.](https://preview.redd.it/knlkunc24er61.png?width=678&format=png&auto=webp&s=edf7e6987ca5afcef4ac5e90c167cb6f022e89e2)](https://preview.redd.it/knlkunc24er61.png?width=678&format=png&auto=webp&s=edf7e6987ca5afcef4ac5e90c167cb6f022e89e2)

DPI vs. Next-Week Return

The initial findings suggest that DPI ratio has a correlation with stock performance the following week, as the stocks with a higher DPI achieved superior performance on average than their lower DPI peers.

The histogram graph below depicts columns based on DPI divided into hundredths, whereas color highlights the number of instances that occurred, giving us a clearer picture of average performance in different DPI cohorts: 

[![r/GME - Hoping some research that I put a lot of time and effort into can make it through the drama. I've spent the past couple weeks collecting and analyzing data on off-exchange short volume, and wanted to share a write-up on my findings.](https://preview.redd.it/n03wp432xdr61.png?width=700&format=png&auto=webp&s=862830ce43f63e5b8c191ea24d5eb02a6291ac51)](https://preview.redd.it/n03wp432xdr61.png?width=700&format=png&auto=webp&s=862830ce43f63e5b8c191ea24d5eb02a6291ac51)

DPI vs. Return: NYSE

Overall, stocks with a DPI of 0.4-0.5 returned an average of 1.08% the following week, whereas the most favorable DPI cohort was 0.5-0.6, averaging 1.41%.

These findings are supported by Squeeze Metrics, [Short is Long](https://i2.t.hubspotemail.net/e2t/tc/VVPKbm4vwXt-N3m0wnGrFLB3W1RGk9h4q1lGqN3ypqFD3lGn5V1-WJV7CgR4TN4c2zmcRJYzJN35bqcWYZy-5W1ZLs561xJ3rmW1cMcN76N0ljlW4fbQ2x4LnsG-Vck8kZ74qj5bV5FtZ12SGJx0W2frnRq7_Sr4TW8BbDf17SfPwZV340-J5RVBS8W5sJb_23xP-x2W6ZlJCJ6k6_t7W2Vgtc_2TS16rW7yxpdK6JSvHkW484W9R2G8HzrW4yygtQ8jbTXDW6fWGg72DkqtZW6XXNfr3h9gYPW2DsyGL9lxVvDW3ZjgnC6m_WsHW2LxKff2ZPdK7W25Vfc83RFVwqW6j_88m6ZSRGcW36CjWN5LLhTb3h3z1), a study in which they assessed Daily Short Volume data for 11,254 securities, between 2010 and 2018. They found  "Very high relative percentages (≥45%) of dollar-weighted short volume are associated with mean 60-market-day returns of 5.3%, as compared to a mean of 2.8% across the whole dataset." (Squeeze Metrics, 2018)

In addition to showing DPI on my new dashboard, I also provide information on the cumulative number of OTC shares sold short for different tickers going back as far as 2010. This will allow investors to see how stocks' off-exchange short interest has accumulated and deteriorated over time, as shown with $GME in the example below:

[![r/GME - Hoping some research that I put a lot of time and effort into can make it through the drama. I've spent the past couple weeks collecting and analyzing data on off-exchange short volume, and wanted to share a write-up on my findings.](https://preview.redd.it/ykgrw58dxdr61.png?width=1530&format=png&auto=webp&s=79b3984a5faf562e33ed1900b41810f55bf6fe80)](https://preview.redd.it/ykgrw58dxdr61.png?width=1530&format=png&auto=webp&s=79b3984a5faf562e33ed1900b41810f55bf6fe80)

Cumulative OTC short vs. $GME

While the Daily Report data sourced by FINRA is publicly available and holds tangible value, it still remains opaque and convoluted compared to what it could potentially be. This is likely intentional, as a 2014 report by the SEC claimed that **"more precise and timely information about short interest could... discourage liquidity supply, fundamental analysis vital to price efficiency, and hedging"**and that "short sellers are often in the best position to report their own transactions" (SEC DERA, Short Sale Position and Transaction Reporting, 2014).

Conclusion

My newly introduced [Off-Exchange Dashboard](https://i2.t.hubspotemail.net/e2t/tc/VVPKbm4vwXt-N3m0wnGrFLB3W1RGk9h4q1lGqN3ypqF13lGmwV1-WJV7CgLNYW8Qy2xS8SdZFbW6vyYMF5Qlbn6VZ1LYg3F3Bj_W46nHPF68g33DW25w3wf9f5qFpW2yTqLR4mlglyW1gF2z-1SgMMmW2BxK4v5P4_5MW6g_Zxw7vdTM3W8RxJVB1ZFHnWW8nSH-k4SZdzLW7P3HWZ7tB6LtV3qZdp8CMxbXW1nnHwW3WjV4kN5tpTdN79bPZMSks1mhbjzdW88pBhh5rgP5SW9kTjsn90L5KBW4wmz9M8BFbt8W6WX1m03JXppw3dv_1) allows users to view the prior trading days off-exchange market activity, with the ability to filter by ticker, the total number of shares short, total numbers of shares traded, and DPI ratio.

I believe that this data can be a valuable tool for tracking market movements, and that the ratio of off-exchange short interest to total volume holds some predictive power for future price movements.
