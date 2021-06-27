Calculating potential Short Interest from Married Put remnants and Share Rehypothecation

========================================================================================

| Author       | Source       | 
| :-------------: |:-------------:|
|  [u/AlexanderHood](https://www.reddit.com/user/AlexanderHood/) | [Reddit](https://www.reddit.com/r/Superstonk/comments/mtnohj/calculating_potential_short_interest_from_married/) | 

---

[DD 👨‍🔬](https://www.reddit.com/r/Superstonk/search?q=flair_name%3A%22DD%20%F0%9F%91%A8%E2%80%8D%F0%9F%94%AC%22&restrict_sr=1)

There have been a lot of posts floating around the subs postulating the real short interest.

I wanted to take a stab at it using what we know for sure about the mechanism for how the FTD's are hidden, the latest put option open interest and why the new DTC rule about double-borrow shares was implemented.

Assumptions

1\.  Citadel and friends are using the Married Put method of hiding FTD's.

2\.  Any Put for a strike of $20 or less for the rest of the year is an irrational option play no sane person would make.

3\.  These apprently irrational puts are in fact part of a rational mechanism for hiding a FTD.

4\.  The current outstanding number of irrational puts is correlated to the number of FTD's resulting from naked shorts.

5\.  Basically all available shares to legally borrow have been legally borrowed.

Shares in cash accounts should not be made available to borrow. (Note the use of the S-word) With much of retail on RH or other brokers who may not be able to resist the temptation to make free money, I'm going to assume the borrow is 100%. (See disc below. If you disagree, swap in your own number and recalculate.) Due to re-hypothecation where a share sold short can be borrowed again and sold short again, the shares borrow number *could* exceed 100%. The daily available shares available to borrow often taps the zero shares mark before magically finding more shares the next day.

Let's math

GME Shares outstanding: 70.03M

GME Float: 45.99M

Irrational Puts from now until Jan 2023:

Apr 16 7,067

Apr 30 6,124

May 7 577

May 14 135

May 21 3,648

May 28 150

Jul 16 299,922

Oct 15 14,736

Nov 19 22,760

Jan 22 220,355

Jan 23 43,984

Total puts: 619,458

Shares equivaluent: 61,945,800

Shares borrowed & rehypothecated for shorting: 45.99M (100% of the float)

Shares failed to deliver: 61.95M (From Married Put remnants)

Estaimted Short Interest: 107.94M total shares

Estimated Short Interest: 234% using the proper industry-standard technique for calculating it

Estimated Short Interest: 70% using the dumb new method S3 Partners invented of calculating it

Discussion

Through the magic of re-borrowing a share sold short, there could be an infinite number of shares rehypothecated but in practice if we assume all shares purchased and placed in a cash account by and honorable broker, only X% of shares could be borrowed back so we have a case of diminishing returns. No idea what X% is here, but if you are reading this post please please move your shares to a cash account or take some action to prevent them from being borrowed. *Small changes to this X percentage have a dramatic effect on the ability to do this type of re-borrowing.*

Conjecture

Personally, I think X% here is 50%, which after maximum re-borrowing works out to be equal to the entire float. i.e. Half the shares are not available to borrow but the ones that are have been re-borrowed. (0.5 + 0.25 + 0.125 + 0.0625 + 0.03125 ... = 0.99) This is why I made the assumption above that shares equal to 100% of the float have been borrowed.

DTC Borrow Rule

Yes, the new DTC rules would prohibit this type of re-borrowing because you cannot borrow a share that has alredy been borrowed. All the shares borrowed more than once would have to be covered, which is half the outstanding float if you subscribe to my 50% estimate.

Very Conjectural

From the latest Bloomberg dump, the Institutions own 122% of the float and from my math we own about 105%. This is actually the reason I did this specific calculation, because I wanted to know if retail owned enough shares to force a moass even if all the Institutions were ordered to paper-hand by the PTB. If Institutions paper-hand in exchange for a seat at the asset auction for Citadels corpse, the moass hits Millions per shares rather than Trillions per share.

And at a minimum, 61.6M shares must be covered just to get back to a (legal) 100% Short Interest on the stock.

Sources

[What DFV knows](https://www.reddit.com/r/Superstonk/comments/mtftsq/i_think_i_figured_out_what_dfv_knows_and_its/)

[Original Post on Married Puts](https://www.reddit.com/r/GME/comments/mgj0j1/the_naked_shorting_scam_revealed_lending_of/)

[Finra](https://finra-markets.morningstar.com/MarketData/EquityOptions/detail.jsp?query=126%3A0P000002CH&sdkVersion=2.59.0)

[Yahoo Finance](https://finance.yahoo.com/quote/GME/key-statistics?p=GME) [Stonk Tracker](https://gme.crazyawesomecompany.com/)

---

**Relevant Comment by [u/Soulsauce042689](https://www.reddit.com/user/Soulsauce042689/)**

Just a quick couple of notes, on some common misunderstandings that DO NOT contradict OP's points, but do shore up some things:

Real shares can not be double borrowed DTC has been tracking lent shares since 2008 if not longer. [Relevant filing: DTC-2021-05]

"if that's the case, how does the SI% reach 226% then?" Best possible answer I can come with is naked shorting - illegal if entity is not a bonafide market maker.

* * * * *

Rehypothection is a lender (broker in this case) using collateralized assets as collateral to borrow from another lender. An example - your home is collateral for your mortgage, your mortgage lender may use your home to gain borrow from their lender.

Relevant note on margin accounts - In margin accounts up to 140% of your equity can be used in rehypothection to borrow capital from another lender.

* * * * *

One big piece to watch this week (22/04) is if brokers have lent more shares than they have the ability to cover. I'm going to be keeping a close eye on borrowable shares and borrow rate. If a significant portion or brokers are over extended on lent shares we can see a massive recall resulting in shorts being (hopefully) forced to cover.
