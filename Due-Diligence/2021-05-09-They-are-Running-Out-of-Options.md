They're Running Out of Options - Estimating potentially hidden FTDs using public options data
=============================================================================================

| Author       | Source       | 
| :-------------: |:-------------:|
|  [u/SuperstonkBot](https://www.reddit.com/user/SuperstonkBot/) | [Reddit](https://www.reddit.com/r/Superstonk/comments/n8gflf/theyre_running_out_of_options_estimating/) | 

---


[🤖 SuperstonkBot](https://www.reddit.com/r/Superstonk/search?q=flair_name%3A%22%F0%9F%A4%96%20SuperstonkBot%22&restrict_sr=1)

Hello you sexy silverbacks, I'm one of the many silent holders and I'm really hoping at least one ape *tries* to read this shit. It's taken me some time to go through everything and type this up, so go find somebody with a nice deep reading voice baby I MEAN I'M JACKED,

IM JACKED TO THE TITS\
I've seen scattered posts on a lot of this stuff, but I'm trying fit the pieces into a more linear argument. I do my best to present data and let it tell it's story.

That said, I wrote I a lot of shit down there, so I wrote most of it in a way that hopefully won't make your mom's boyfriend fall asleep while to reading to you.

I think I linked everything I used so ..

Please let me know where I'm off!!\
( [This important post](https://web.archive.org/web/20210504013036/https://www.reddit.com/r/Superstonk/comments/mtmqf3/critical_thinking_from_a_psychology_academic/?utm_source=share&utm_medium=ios_app&utm_name=iossmf) by [u/Makataui](https://web.archive.org/web/20210504013036/https://www.reddit.com/u/Makataui/) - a Psychology professor who's made a living on his ability to logically discern shit- goes over the importance of critical thinking, especially in our dopamine bath of confirmation bias and group polarization !! Save it for later, at the very least. )

Also this isn't advice, some of it will be wrong - it's my interpretationspeculation of data.

It's blind ape's description of an elephant.

TLDR:\
If you don't like foreplay you can skip to the numbers warning. If you don't wanna read any of it I guess just hodl until Jan 21, or at least wait for a bankruptcy or two. Basically there are so many ways to indefinitely roll FTDs into the future, the number of actual fails in GME, and maybe the whole system Idk, is pretty much a measure of Wall Street's integrity.

//

Okay, so

1\. Options Options\
I've been digging through [GME options data](https://web.archive.org/web/20210504013036/https://www.barchart.com/stocks/quotes/GME/options?expiration=2021-04-30-w&moneyness=allRows) for a while, and I found some, uh, colorful numbers. I'm hoping someone less autistic than I am can tell me why they smell like horse shit.

Most of GME's expiry dates, EXCLUDING 7/16/21 and 1/21/22, are pretty boring. Not only are there low volume and open interest, there are far fewer strikes with interest, *especially* at sub $50 strikes. But for July 16 and Jan 21, strikes climb in $0.50 increments up to $5.50. Most other dates begin $5, usually moving in $5 or $10 increments.

Alright I'm losing you already so I'll back up and explain as I go along. If you know this shit already skip to - (???????? ????????)

Each option contract (call or put) represents a non-obligational right to buy (call) or sell (put) x number (usually 100) of shares for an agreed upon price (strike price) per share, by an agreed upon expiration date. These are contracts, not shares - owning the right to buy/sell has an opposing obligation to deliver/purchase. This means that options traders are not required to buy contracts before selling them. Typically the trader will instead buy 100 shares of the underlying security to "cover the call".

This is one reason why looking at open interest data is useful. Open interest is the number of contracts yet to be settled at some expiration date, and the options data I linked above shows the interest of individual strike prices within that date.

Contracts can be settled (and thus OI decreased) in 3 ways: 1) they can be exercised (buyer exercises his right to buy/sell), 2) they can expire worthless, 3) the seller can purchase the option back from the market

Btw notice how I said "market" and not "buyer" - that's because when a contract's seller buys to close, the market (the OCC) fills his buy order (bid) with a random seller, even if one of his original buyers has a sell order (ask).

This is largely for two reasons: 1) So a trader on Citadel's trading floor can close his position without waiting for individual RobinHood buyers to sell their calls, and 2) to prevent a trader from just buying calls from Phil down the hall (this will come up later, surprise lmao ofc he still can)

Options chains are usually organized by strike prices at different expiration dates, and every buyer has a seller, so even if a trader buys to close, the overall OI on $60 calls will only decrease if he manages to buy back calls he originally wrote, otherwise that interest is just shifted to Credit Suisse or whoever sold.

This means that, even if a trader's initial option position is closed, the option will still have interest until all buyers decide to sell.

Note: Options are typically organized by strike and expiration, but that does not mean all traders trade at single strikes. A trader can fill my 250k order at $60, or he can tell me to fuck off and write 50 calls at every strike from $40-$60, adding more room to hedge and possibly making liquidity easier.

So remember how I said there were options on 7/16 and 1/21 in 50 cent increments up to $5.50...

(????????????????)

2\. ETFs, FTDs, WTF\
This is probably where you may want to break out the tinfoil...

By looking at an [option's price history](https://web.archive.org/web/20210504013036/https://www.barchart.com/stocks/quotes/GME%7C20210716%7C0.50P/price-history/historical) you can see when that option began trading, hinting at when the option was originally written, and almost every option within those weird 50 cent increments began trading just after the 2020 dip in March, with some going back further into 2019 at very low activity until March 2020. Note GameStop was trading around $3.50 before the March 2020 drop. These March dates aren't regular, either. Most other options were not traded until November, 2020.

** *cue speculative cutscene* **

Now, if I'm Phil the Hedge Fund Manager in March, 2020, looking at brick-and-mortar GameStop, a company I've been short for years on that's now trending into the dirt BEFORE a global pandemic --- and I'm watching all my friend's brick-and-mortar short positions furiously shitting Benjamins, what better way to print free money than just sell bunch of calls and wait for the iNeViTabLe bankruptcy? Mother Nature just broke into the ICU and stuck a knife in GameStop, says Phil, so if any of the calls are executed I'll just borrow the shares to cover them for a measly $350 per contract and maybe I'll borrow some more to deliver the first batch I borrowed. What? FTD? Is that like FYE?? Ehh who cares GME will be in retail heaven with Blockbuster and Toys Were Us by January. Flu season in a pandemic?? I'll see you in Barbados boyzzzz

MAYBE Phil, with Ponzi-the-money-printer, earns his firm, Edgar Capital, [60 PERCENT RETURNS IN 6 MONTHS](https://web.archive.org/web/20210504013036/https://fintel.io/ip/melvin-capital-management-lp) and now his bosses who earned 10% last year are literally asking him to fuck their wives. And their daughters. In Barbados.

Maybe things start to get [a little tense](https://web.archive.org/web/20210504013036/https://images.fintel.io/us-gme-fails-to-deliver.png) toward the end of September. Just a month ago Phil thought FTD was an STI and now people are calling him Margin Capital online :(

Now seems like a good time to talk about what exactly happens when a trade fails. If your trades fail all the time already, skip to -

(????????????????????)

It might be helpful to think of any given hedge fund or capital group as.. less like a chess grandmaster and more like the guy who sells hotdogs downtown at 2 am. He picks the street, maybe he makes the chili, but unless he's selling to a restaurant, he's kinda fucked unless people stumble up to him. He's got some wieners in stock, but if there are more buyers than wieners, he might take their money and tell them to come back tomorrow for their hotdogs.

Now picture millions of these bastards huddled inside their Broker-Dealer Cafeteria's, all stuffed inside Market Maker Superdome selling and promising food all day to orders coming in - add a few more superdomes and replace hotdogs with stocks, ETFs, options, blah blah that's basically the stock market.

To set the scene, it's late August, 2020, and Grandma buys a share of Monster and at the end of the day, Phil has no Monster. Usually Phil's BD will lend Phil its shares (or just create them..) for a day or two, and if he doesn't find Grandma's Monster by then then, he must declare a fail-to-deliver. Well Phil has amnesia and after two days he just declares fail-to-deliver. Phil now has 3 days to find the Monster or Phil's Market Maker (who clears the BD's trade), on the fifth day, will force the BD to buy one with his money.

*Unless* that BD vouches that Phil's a kind, forgetful guy, in which case Phil gets to tack on another 3 days.

[This SEC document](https://web.archive.org/web/20210504013036/https://www.sec.gov/investor/pubs/regsho.htm) goes over these guidelines btw I'm not just spitballing

*In a shocking twist of events* - Apple buys Monster and now Phil's fucked. There are no shares to borrow and Monster is too expensive to buy.

Let's say the BD's Market Maker is Phil's wife's boyfriend's brother - and honestly the MM has so many shares he wipes his ass every day with them every day, so - if there's an ETF (basically a veggie burger of shares) containing Monster, he can use his MM authority to throw some Monster into a 50,000 share burger called a creation unit, then sell it to BD as a new share of the ETF. BD trades the ETF to Phil, who's been holding the BD's share so he doesn't fail to deliver, then Phil plucks a Monster seed from the burger and *voila* Monster is on the books - Phil shows the BD the MM's shares, winks, and the FTD is settled. On paper.

The DTCC is the final clearing destination for most US trades. They allow 35 calendar days for MM's to settle, so Phil rented the MM's extension and the MM is trusting Phil to find Grandma's Monster in 35 days. When he does, he can sell the newly minted ETF share back to the MM, the MM puts the shares back in their places and it's all roses and ????????

Oh btw, to tie in the hotdog guy analogy, you probably won't be surprised to know that the Superdome owns a lot of the Cafeterias inside. Many Market Makers *are* Broker-Dealers. This reduces internal regulation, and, because these trades are often beneficial for everyone except Grandma, they can potentially be abused.

Okay to keep things realistic, let say Monster's only ETF is the Wedbush Addictive 50 ($WADD) and holy shit, Apple is in there too. Just before the ETF-burger move, the MM is out of Monster and and Phil's fuckedfucked

In this situation, Phil can simply offer his wife to his MM, in which the MM can build the WADD as a creation unit of IOU's, called an [ETN](https://web.archive.org/web/20210504013036/https://www.investopedia.com/investing/etfs-vs-etns/), from which Phil can pluck the Monster IOU, and *voila* - Phil's has a happy Grandma and a happier wife

(????????????????????)

MMs generating ETFs and ETNs as a means of lending less-liquid securities inside, is well covered in [this presentation](https://web.archive.org/web/20210504013036/https://youtu.be/ncq35zrFCAg). This is one way to conceal fails, but they're not *entirely* hidden - the fails may still show up within the ETFs.

As I understand it, if this were the case with GME, or any security, you would expect repeated spikes in ETF fails, ~6-8 days after the security fails.

Of course this would smell like bull shit from a mile away, so there are a few other ways fails can be kicked down the road. They're not my secrets lol both of my great grandparents are still alive - the SEC warned about them in 2103:

//

Side note on ETN's:

ETN's are, by definition "unsecured debt obligations" - and they have legitimate benefits. As debt obligations they also have risks, as [this presentation from 2019](https://web.archive.org/web/20210504013036/https://youtu.be/ncq35zrFCAg) discusses.

I have a concern I really hope someone can ease for me. A short position is a debt obligation, so wouldn't borrowing to cover a short create a collateralized debt obligation? And if ETN's are basically virtual, unsecured debt obligations, wouldn't repeatedly using ETN's to cover short positions create a synthetic collateralized debt obligation?

Yes I'm unashamedly using 2008 hot words, and maybe I shouldn't, but considering the (albeit extreme) example at 28:00 in the video I linked above, when XRT (ETF containing GME) reported 78m ownership of 11m outstanding shares -

That's a security-stew of 11m veggie burger bits floating in a broth of 67m promises. Priced by the pound.

I genuinely hope this FTD shuffling tactic isn't accidentally (or otherwise) creating synthetic CDO's. Remember the Asian dude Michael Scott's alter ego almost strangled in a restaurant over how completely autistic derivatives of synthetic CDO's were? Wouldn't that just translate to all options contracts and other derivatives involving ETF's??

//

3\. It Often Rhymes\
If you don't read another word of this post, please please save [this SEC risk alert from 2013](https://web.archive.org/web/20210504013036/https://www.sec.gov/about/offices/ocie/options-trading-risk-alert.pdf) to read for later.

That document reviews the FTD settlement guidelines that I went through earlier and discusses two other known methods of concealing fails: married puts and buy-write transactions.

Reminder that this is all in relation to GME's first big FTD spike in September and the July/Jan share price), essentially replacing the short position (shares are needed to exercise)

In either case, as with ETF/ETN schemes, the trader who was short is essentially paying the MM for access to the 35 day settlement exception.

(??????????????)

4\. What You Know For Sure\
Back to September. Hedge funds and Market Makers have been turning retail short sales into Ferraris and Ivy League athletic scholarships for the past 6 years. They successfully [strangled multiple businesses into bankruptcy](https://web.archive.org/web/20210504013036/https://stockhouse.com/news/newswire/2016/01/19/how-short-sellers-are-killing-companies-and-market). multiple businesses into bankruptcy and now flu-season was approaching amid not only a global pandemic, but a global microchip shortage that completely halted distribution of GameStop's single biggest sales driver: gaming consoles.

Its important to note that the market is a dynamic system that is intentionally confusing. There are hundreds of multi-million dollar firms placing thousands of bets, and generating liquidity through short selling is a genuine part of a MM's job.

That said, through BD/MM affiliation that benefits both parties, even if caught and fined - the potential for 1 or 2 disingenuous traders to begin contagion is a legitimate threat. [This video originally from 2003](https://web.archive.org/web/20210504013036/https://youtu.be/I0WXg5T3cBE) describes this in more detail.

This is highly speculative and I should probably leave it out but fuck it

In my opinion, given ample opportunity, deep fucking incentive, sound rationalization, and chicken shit regulation - it is seems possible that, on a market wide scale, 100+ million shares that should have failed-to-deliver are quickly, and sometimes fraudulently, shuffled --- via married puts, buy-writes, ETF manipulation including ETF/ETN creation units from a Market Maker, and writing naked calls --- to maintain the virtual appearance of buying/borrowing shares to settle the FTD.

The fuck was I saying

Oh yeah September

Back in August, [short interest reached $426 million](https://web.archive.org/web/20210504013036/https://www.marketbeat.com/stocks/NYSE/GME/short-interest/). Correct me if I'm wrong, but at ~$4.70 share price, that's over 90 million shares sold short. If that's accurate, that's uhh.. a little aggressive there, chief

So by September, fails start rolling in. Phil is seeing FTD tags in his nightmares - *Fuck, how many calls did I sell? How many shares do I have? Are those shares borrowed? What the fuck is a DTC??*

At this point, Phil has to decide between:

a) cutting his possibly massive losses and unwinding one of the biggest cash cows beneath the [64+ billion dollars](https://web.archive.org/web/20210504013036/https://www.google.com/amp/s/mobile.reuters.com/article/amp/idUSKBN29U00R) hedge funds made in 2020, or

b) paying a small fee and risking another small fee to double down and stay short

Oh, let's not forget that cold/flu season is approaching amid, not only a global pandemic, but a *global microchip shortage* that will probably slow distribution of GameStop's single biggest sales driver: gaming consoles.

Maybe Phil was smart and got out. Obviously his friends didn't. 4.2 million shares failed in 2 days, October 13-14, and the 30m share Niagara Fails of December and January suggests some quadrupled down in October.

5\. Everything in the World is Magic...\
Here's a puzzle:

Assume someone wanted to use some of the the neat and totally legalish tactics I so concisely described to indefinitely roll FTDs into the future ---

Using public data, estimate just how heinous GME's actual rolling FTD number *could* be.

I'll shoot for a realistic degree of atrocity

(my limited understanding of) The Rules:

-Roughly, ( beneficial ownership ) --- ( shares outstanding ) = ( total shares owed )

-   Broker-Dealers have 2 trading days after a client is short to cover. Otherwise they report a fail and have 6 trading days after the fail to cover - which can be done btw by buying *or borrowing* shares

-   *BUT* with a little Market Makipulation, BDs can temporarily report short on the 5th day after failure, wait 2 trading days before reporting a fail, then have 35 calendar days after the fail to settle

-   Evidence of this process should include FTD spikes in one or more ETF's containing GME ~6-8 days after a large number of GME fails

( edit: [This post](https://web.archive.org/web/20210504013036/https://www.reddit.com/r/Superstonk/comments/n4axra/95_gme_etfs_3_months_of_ftds_visualized/?utm_source=share&utm_medium=ios_app&utm_name=iossmf) by [u/Leenixus](https://web.archive.org/web/20210504013036/https://www.reddit.com/u/Leenixus/) overlays FTDs in GME and its ETFs and compares to other securities. )

-   Accurately accounting for FTDs concealed with synthetic options positions and ETF's is impossible, but I'll do my best to explain my estimates. I'll start by identifying FTD spikes, usually in groups of 3 or 6 days (because of the T+3 and T+6 settlement requirements).

-   Oh btw, Citadel, the BD/MM in question here, [clears 99% of all options trades](https://web.archive.org/web/20210504013036/https://www.citadelsecurities.com/products/equities-and-options/), so if there's open interest in a contract, statistically there's a 99% chance Citadel is liable to settle it. I'll bump that to 100% for kicks

Warning\
??????

Numbers Ahead\
//

This entire post is built on using data to speculate.

The following argument, however logical or likely it may or may not be, is, obviously, speculative.

The puzzle is complex. The answer is likely more complex.

Apes just hodl that's not so hard.

//

GameStop Corp\
[Fintel data](https://web.archive.org/web/20210504013036/https://fintel.io/ss/us/gme) (note: Month markers on the FTD graph mark the *middle* of the month) shows:

~4.1 million GME shares failing from September 2-9 (6 trading days)

~5.8m shares failed September 21-25 (5 days)

~4.2m shares failed October 14-15 (2 days)

~5.6m shares failing December 2-8 (5 days)

~4.2m shares failing December 17-24 (6 days)

~3.3m shares falling from January 5-11 (5 days)

~6m shares failing January 13-21 (6 days)

~5.1m shares failing January 26-28 (3 days)

XRT\
[XRT](https://web.archive.org/web/20210504013036/https://fintel.io/ss/us/xrt), GameStop's most liquid ETF, had:

~3m shares failing September 28 to October 6 (7 days)

~2m shares failing December 15-17 (3 days)

~5.7m shares failing January 28 - February 3 (5 days)

You can roughly see how XRT's FTD spikes fit between GameStop's. The 2 most other liquid ETF's had spikes of ~100k or so.

Based on the FTD data, let's say, ohhh Idk - 4 million FTDs are rolling into January, using the ETF/ETN tactic to alternate between GME and XRT.

Citadel claims to clear virtually all options trades, and based on [GME option data](https://web.archive.org/web/20210504013036/https://www.barchart.com/stocks/quotes/GME/options?expiration=2021-05-07-w&moneyness=allRows&view=stacked_ohl) call total OI is 104,221 on 7/16 and 1/21 alone. Total call OI from the other 10 expiration dates is ~105k for a grand total of ~210k interest.

um\
If [Citadel is clearing 99%of all options order flow](https://web.archive.org/web/20210504013036/https://www.citadelsecurities.com/products/equities-and-options/), and they're constantly [delta-gamma hedging](https://web.archive.org/web/20210504013036/https://www.investopedia.com/terms/d/deltagamma-hedging.asp), what better way to roll a FTD than to:

1.  Make long calls a little cheaper and gobble up the bids.

2.  Collect all 210k premium payments and now, as a MM, they have to [delta-gamma hedge](https://web.archive.org/web/20210504013036/https://www.investopedia.com/terms/d/deltagamma-hedging.asp) those calls to claim a riskless position.

3.  Use all those "for hedging" shares to satisfyextend the FTD requirement, then strategically dump the shares hedging all the calls *you think* will expire OTM, since no hedge is ultimately needed for a call never exercised.

4.  EZ game, now Citadel gets to collect premiums for resetting some FTDs and driving the price down

Delta hedging would typically require somewhere between 9-99 shares per call, with more shares needed for deeper ITM calls.

Taking the 210k (and counting) call OI as a whole, of which Citadel claims to clear 99%, if 50 shares are delta-hedged on average, that grants Citadel access to 10.5m shares for allocating to failed trades.

Of course not all of them would allocated, but the allocation process would essentially be the same as that time Phil lost Grandma's Monster. This would mean that some portion, maybe a large portion, of GME's daily trading is Citadel allocating and eventually repurchasing shares from its clients with high FTD's.

And maybe if there aren't selling enough calls, the resort to [Buy-Writes](https://web.archive.org/web/20210504013036/https://www.reddit.com/r/GME/comments/lylvrb/update_35_1625_million_of_deep_itm_gme_calls_have/)...

6\. Eventually, Trust Fails\
What in the depressing fuck kind of title is that

Anyway remember when Phil's MM made a WADD and Phil traded his wife for it?

[XRT's Options data](https://web.archive.org/web/20210504013036/https://www.barchart.com/etfs-funds/quotes/XRT/options?expiration=2021-05-07-w&moneyness=inTheMoney) reveals ~51k call OI over 11 dates, 45k of which are concentrated in only 3 dates: 5/21, 6/18, and 9/17. Notice how those dates fit nicely between 7/16 and 1/21, the two dates housing half of GMEs call OI.

*tinfoil time*

Ken sells calls and hedges and juggles FTD's and Ken plans to pretty much do it until he retires. Well when those $69,420 calls expire, he should still have the one share he had to buy as a hedge. If he gave that share to Phil to cover both their asse(t)s he needs to either buy his share back or find another one. Well Kenny's no rookie - he's been doing slight-of-shares with ETF's since, like, 2006 - so he buys or whips up or promises to whip up an XRT burger and everything's ???? and ????????.

Yeah that's not gonna make sense if you skipped the foreplay, sorry.

Well the only thing better than XRT is free XRT, so Ken can just sell cheap XRT calls, forcing delta hedges on XRT, then crack open the XRT and allocate the GameStop.

But even if all 50k XRT calls were hedged with 100 shares, GME is only 7% of XRT. So 5m XRT shares equates to 350k GME shares...

*Allow me to introduce:* [IWM](https://web.archive.org/web/20210504013036/https://fintel.io/so/us/gme/ishares-trust-ishares-russell-2000-etf)

IWM is the iShares Russel 2000, and they announced a 15% increase in GME on 2/25/21. Funny, I didn't hear much about it.

IWM holds GME at a humble 0.35%. Take a guess at what [IWMs options chain](https://web.archive.org/web/20210504013036/https://www.barchart.com/etfs-funds/quotes/IWM/options) looks like...

You *may* not guess a call OI of 1.56 million over the 15 expiry dates from now until 1/21/22. Hedging those at an average of 50 shares/call represents 78m shares. At 0.35%, thats 2.7m GME shares.

By the way, if an extra 2.7 million shares available to extend shorts, purely in call hedges, doesn't shake you, remember GameStop is in over 60 different ETFs.

Oh and it gets better

I've been talking about calls for a while but *puts* exist too. If you somehow managed to read through this whole post you'll remember what the SEC said about married puts...

The put OI for IWM, up to 1/21, is 3.7 million. ~750k of those puts are at-the-money. With GME at .35% of IWM, that potentially represents 2.6 million GME shares capable of floating FTD's via married puts in IWM.

Married puts *should* have ATM puts to maintain the short position, but they don't need to be ATM to settle a FTD - one reason MPs are used over just re-borrowing (and the reason they're illegal) is they function by claiming one asset as collateral in two transactions. There are 100 shares married to the put (risk-less position to skirt regulation) and the same 100 shares are used to close the FTD.

The MP provides the paperwork loophole but it's not necessary for the short position. Phil can just borrow shares ( [IWM shortvol% was apparently 74% on 4/30](https://web.archive.org/web/20210504013036/http://shortvolumes.com/?t=iwm) ), buy a worthless put to marry and instantly divorce, and now you did the paper magic and are still short. Maybe they call it a one night stand Idk

The total put OI of all strikes with over 10k OI is over 2.5 million.. there are puts at dozens of strikes trading for $1. If ONE THIRD of those were used for disposable MP's, that's another 2.6 GME shares.

Which is interesting, considering GME has [329k put OI at the LOWEST 2 STRIKES on 7/16 and 1/21](https://web.archive.org/web/20210504013036/https://www.barchart.com/stocks/quotes/GME/options?expiration=2022-01-21-m&moneyness=allRows&view=stacked_ohl). Even more interesting about those 329k puts - when they were being gobbled up in late January, ~200k of them, they averaged their highest prices of all time.

50 cent puts... While GameStop was soaring. Went from $4 in December to $15 on Jan. 28. Right.

Guess I could take a shot at that puzzle now.

Total potential-shares-for-allocation estimate:

-Citadel delta hedging call order flow: 10.5m

-[The suspected Buy-Write trades](https://web.archive.org/web/20210504013036/https://www.reddit.com/r/GME/comments/lylvrb/update_35_1625_million_of_deep_itm_gme_calls_have/): 14,500 calls = 1.4m shares

-Citadel delta hedging IWM calls: 2.7m

-Married puts in IWM: ~2.6m

-Married puts in GME: up to 32m.. but I'll leave these out

Total: 17.2m GME shares

If half of these were actually used to roll fails, 8.6m + the 4-5m already rolling in the FTD data + 11m reported short volume = ~26 million shares sold short

Including the GME puts and everything else - it'd be ~64 million.

And *excluding* married puts, Citadel has access to over 13m GME shares, solely from delta hedging GME and IWM calls, to potentially distribute among shorts about to fail.

Do not forget that I don't know what the fuck I'm talking about. I'm not an expert in this stuff, I just had surgery two months ago and it pisses me off when shit doesn't make sense.

These people have been playing this game for years and I'm sure there are dozens of other ways reversals can be achieved, they get fined like 100k for this shit and without it.. well if it's bad enough they'll go bankrupt.

//

My point here is - where there's smoke there's fire, and there's so much smoke in these numbers I can't taste the purple in my lunch.

Obviously none of that was advice or conclusive I can't even spell conclusive

//

All this shit is meant to be be confusing. The internet revolutionized trading, especially options. In fact they started becoming popular in the 90's, right around when ETF's came along. The SEC talked about two ways options could be used to hide FTD data - and I liked a presentation talking about how ETF's can be used to do the same thing. The AMA last week mentioned it, too.

All of these loopholes serve to provide Citadel, who claims to clear 99% of options order flow, with enough shares *merely in hedges* to juggle 13 million fails. Add to that buy-write transactions, married puts, naked calls, ETNs, and all the other autistic things possible in a system so complex, who tf knows how many shares they might be juggling on paper.

The options, to me, look like a smoking gun. Fails in GME's ETFs repeatedly fall between fails in GME, suggesting some number of fails are being rolled with ETFs. The number of ETFs with institutional ownership over 100% 6 months ago suggests many of those shares used to cover came from ETNs.

The fact that the bulk of call OI in IWM and XRT falls neatly between the call OI in GME suggests these options are, in some capacity, related to rolling fails into the future.

THAT SAID -

Regulation changes increasing margin requirements or decreasing settlement times, would begin to unwind these positions. And-

A share recall would bring the buying pressure of every IOU floating around because of this horseshit.

A bet on GME is a bet again Wall Street's integrity.

But - don't just trust me on this stuff, seriously, use the links, find some bullshit that looks weird and ask yourself why it's weird. I promise, there's lots of weird shit. Start with the 1500 $1.50 calls someone bought / Citadel sold for 1/21.

And the 100k 50 cent puts that *weren't* bought in January probably traded for under $5 so I'm sure plenty of that is legit. On the other hand, I do remember a post saying put OI in early March was obscenely high but I can't find it anymore.

If you just scrolled on down here and read the "my point is" part, no worries. The post was just some bullshit anyway - 11m reported shorts is an infinite short/float % because there is no float.

Oh and if really read this whole fucking thing, message me and I'll fly you to dinner next year.

* * * * *

*This is not financial advice!*\
*This post was **anonymously** submitted via *[*www.superstonk.net*](https://www.superstonk.net/)* and reviewed by our team. Submitted posts are unedited and published as long as they follow *[r/Superstonk](https://www.reddit.com/r/Superstonk/)* rules.*
