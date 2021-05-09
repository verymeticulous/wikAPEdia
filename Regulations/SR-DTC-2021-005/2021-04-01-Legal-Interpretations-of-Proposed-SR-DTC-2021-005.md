Legal Interpretation of the Proposed SR-DTC-2021-005
====================================================

| Author       | Source       | 
| :-------------: |:-------------:|
|  [u/BigBrainBets](https://www.reddit.com/user/BigBrainBets/) | [Reddit](https://www.reddit.com/r/GME/comments/mi8mo9/legal_interpretation_of_the_proposed_srdtc2021005/) | 

---

[DD 📊](https://www.reddit.com/r/GME/search?q=flair_name%3A%22DD%20%F0%9F%93%8A%22&restrict_sr=1)

Let me preface this post by saying there are a number of effects arising out of the proposed changes SR-DTC-2021-005, primarily because a Pledgor and Pledgee can be a mix-match of parties depending on the transaction being scrutinized. Think of it like playing Mariokart, sometimes Kenny G plays as Bowser, and sometimes he plays as Wario. To be blunt, the same party can be a Pledgor in some cases, and a Pledgee in others. Same goes for other market participants. Thus, there are are a variety of implications from these changes.

That being said, I will leave you with my main takeaway after a brief overview of the proposed language:

In my opinion, some of the [proposed] language in SR-DTC-2021-005 is designed to limit the ability of market makers and hedge funds working together to reset FTD transactions and/or conceal short positions through nefarious options trading.

In case you are not well versed on the nefarious options trading process by now, here is a quick breakdown. I will subsequently refer to this process as Steps A-F, respectively.

A. If short sellers [Pledgor] are facing a squeeze because shares are hard to buy, or scrutiny for holding an illegal short position, they can create an appearance of having closed their short position through the use of deceptive options trades, called a reset transaction.

B. A hedge fund [Pledgor] that is short a stock can write call options on a stock --- meaning they are now "short" the call options, having sold the call options to someone else (typically a market maker) [Pledgee] --- and simultaneously buy shares against the call options.

C. The shares bought against the call options could be "synthetic" longs --- meaning they are not part of the original share float of the stock --- as sold to the hedge fund [Pledgor] by the market maker [Pledgee] that takes the other side of the options trade.

D. This works because, if a market maker [Pledgee] buys options from an options writer, the market maker [Pledgee] has legal privileges to do a version of "naked shorting" as part of their hedging function. This is necessary, under the current rules and the current system, for market makers [Pledgee] to protect themselves when facilitating options trades. In theory, this privilege allows market makers [Pledgee] to provide liquidity in the options market when a trade order lacks a buyer/seller on the opposite side.

E. As a result of the above transaction, the hedge fund [Pledgor] that sold short calls was able to buy synthetic long shares against the calls. (A synthetic share is one that has a long on one side and a short on the other but wasn't part of the original float.) The synthetic long shares are the other side of the naked shorts, legally initiated by the market maker [Pledgee], so the market maker [Pledgee] can hedge their position to remain a net-neutral party.

F. The hedge fund [Pledgor] that bought the shares can now report that they have "bought back" their short position via buying long shares---except they actually haven't. The synthetic shares they bought are canceled out against the short call positions they initiated, a necessity of the maneuver by way of the market maker's [Pledgee] hedging of the call position they bought from the hedge fund.

The Pledgor/Pledgee role could be reversed, depending on the circumstances. So just roll with me for now.

Lets get to it.

When reading the excerpts from the proposed rule, remember the following:

Bold text indicates additions;

~~Bold strike-through text~~ indicates deletions

Settlement Transactions (p.41)

> There are three main types of transactions processed through the Settlement system.
>
> ***
>
> 3\. Collateral loans: The collateral loan service allows a Participant (the pledgor) to pledge securities as collateral for a loan or for other purposes and also request the release of pledged securities. This service allows such pledges and pledge releases to be made free, meaning that the money component of the transaction is settled outside of the depository, or valued, meaning that the money component of the transaction is settled through DTC as a debit/credit to the pledgor's and pledgee's DTC money settlement account. When pledging securities to a pledgee, the pledgor's position ~~is moved from the pledgor's~~ ~~general free account to the pledgee's account~~ continues to be credited to the pledgor's account, however with a system notation showing the status of the position as pledged by the pledgor to the pledgee. This status systemically ~~which~~ prevents the pledged position from being used to complete other transactions. Likewise, the release of a pledged position would move the pledged position back to the results in the removal of notation of the pledge status of the position and the position would become pledgor's ~~general free account where it would then be~~ available to the pledgor to complete other transactions.

Collateral Loan Program (p. 42)

> The Collateral Loan Program allows you to pledge securities ~~from~~ held in your general free account as collateral for a loan or for other purposes (such as Letters of Credit) to a pledgee participating in the program. You can also request the pledgee to release pledge securities ~~back to your general free account~~~~.~~ These pledges and releases can be free (when money proceeds are handled outside DTC) or valued (when money proceeds are applied as debits and credits to the pledgee's and pledgor's money settlement accounts). A Pledgee may, but need not be, a Participant. Only a Pledgee which is a Participant may receive valued pledges.

My interpretation of the DTCC perspective:

(See Step B above).

"From" is way too ambiguous; any lawyer with half a brain can manipulate this in any which way (For example, I could argue that I have "credited GME shares in my account from an incomplete or pending transaction" therefore, I should be able to use those shares as collateral because they are "From" my account, even though I don't actually own them yet, OR never plan to....).

By changing this to "Held in" tells me that the DTCC wants to place more emphasis on the Pledgor [short seller] actually being obligated to hold the shares, or position, they are planning to trade (I.e., not being able to rely on pending transactions]. To be clear, the DTCC is only worried about their own liability and covering their own ass here, not necessarily punishing the wrongdoings of bad actors. This is explicitly confirmed in the section above titled "3. Collateral Loans" and becomes more clear when read in conjunction with the following language:

> "These pledges and releases can be *free* (when money proceeds are handled outside DTC)"

(I.e. if Citadel and Melvin want to hold hands in the backyard that's fine, just not at the dinner table). BUT, if Citadel is transacting as a DTCC participant (I.e. at the dinner table) then the transaction must be *"valued"* as opposed to *free.*

> "*valued* (meaning when money proceeds are applied as debits and credits to the pledgee's and pledgor's money settlement accounts)."

In other words, the DTCC is saying do as you wish as long as we are not involved, but if the DTCC is acting as an intermediary for the exchange of securities, then "SHOW ME THE MARGIN" *Jerry Maguire voice*. Someone mentioned in another post this morning that Citadel opened a new office location in Austin, Texas on the same street as several other financial institutions. I'm sure they have offices all over the world, but it goes without saying that conducting "offline" trades and option swaps with other institutions, or "*free*" collateral loan programming as the DTCC calls it, seems much easier if you are in close proximity to your trade partners. Regardless, this is pretty irrelevant for the purpose of this post, so I'll leave that for someone else to discuss; like the Citadel Has No Clothes stud, I forgot his username, but his posts are golden.

Moving on...

Settlement Transactions (p.41)

> When pledging securities to a pledgee, the pledgor's position ~~is moved from the pledgor's~~ ~~general free account to the pledgee's account~~ continues to be credited to the pledgor's account, however with a system notation showing the status of the position as pledged by the pledgor to the pledgee. This status systemically ~~which~~ prevents the pledged position from being used to complete other transactions

My interpretation of the DTCC perspective:

If the market maker and hedge fund are transacting through the DTCC, the DTCC will now be monitoring the Pledgor's [hedge fund] position in order to ensure the validity of the pending transaction. This seems consistent with the previous rules we have seen come through the portal lately. The DTCC is ramping up their oversight and overhauling their rulebook to be consistent across the board.

(See Step F above).

To put it in simpler terms, let's look at it from the eyes of the DTCC:

Okay Melvin, I see you own enough shares to pledge that trade you submitted to Ken. However, now that you have pledged those shares to Ken, they are locked, and you are not allowed to use them to enter a new transaction with Jim. In addition, we also see you have a ginormous short position. We just want to make sure that you are not offering the same shares to multiple people at one time. That sounds pretty risky if they all come looking for those shares at the same time, dontcha think? Cool, this new account status provision will stop you from blowing your ass off by promising transactions to new Pledgees with shares that are already pledged to someone else in a pending transaction. We can call this the "no double dipping" provision.

Pledges to the Options Clearing Corporation (p. 42)

> A Participant writing an option on any options exchange may fully collateralize that option by pledging the underlying securities by book-entry through DTC to the Options Clearing Corporation (OCC). If the option is called (exercised), the securities may be released and delivered to the holder of the call. If the option contract is not exercised, OCC validates a release of the pledged securities**~~,~~ ~~which are then returned to the Participant's general free account~~********~~.~~**

Release of Deposits with Options Clearing Corporation on Expired Options (p.42)

> OCC automatically releases securities deposited with it to cover margin requirements on an option contract when the option contract expires. ~~The securities are then allocated~~ ~~to your general free account.~~ Notification of the released securities is received via the\
> Collateral Loan Services functionality in the Settlement User Interface or automated output.

My interpretation of the DTCC perspective:

(See Step D above).

Hedge those calls as you need to, Ken. We have no problem with that, and we appreciate you providing liquidity to the market. Although we enjoy you bringing the liquidity to the market, we aren't sure about what you're doing with all those [synthetic] shares you are buying when you hedge these call options. So we are making a change:

(See Step E above).

Instead of allowing you to hold on to these synthetic shares (and probably short the fuck outta GME with them at your own discretion, or give them to Melvin to conceal his shitty short position), they'll just be returned to the public float if the option contract is not exercised on your mischievous reset transaction. In other words, because the MM's have the ability to create synthetic shares they were previously allowed to hold onto those shares if the call options were never exercised.

To be clear, the new language does not explicitly state what procedure is going to happen if calls are not exercised. Thus, I am making a hypothesis that the shares will be returned to the float because it seems like the only logical explanation to me if they DTCC is no longer going to return t hem to the general participant account.

TLDR: Overall, the proposed changes seem to be consistent with the other rules we have seen submitted over the past few weeks. The DTCC is revamping their entire rulebook to make these changes consistent across the board.

In addition, the [proposed] language in SR-DTC-2021-005 is designed in a way that may hinder the ability of market makers and hedge funds who work together to reset FTD transactions and/or conceal short positions through nefarious options trading.

Edit: Apologies for the shitty quote formatting, I was copy and pasting from the PDF and I guess reddit's text box wasn't fucking with the pdf coding. Will try to fix when I get home.
