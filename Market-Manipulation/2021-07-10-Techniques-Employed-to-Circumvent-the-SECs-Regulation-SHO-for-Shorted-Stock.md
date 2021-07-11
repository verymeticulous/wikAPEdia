Illegal Naked Shorting - Techniques Employed to Circumvent the SEC's Regulation SHO for Shorted Stock, FTDs, Borrow Lists, Threshold Securities through Continuous Net Settlement System and Stock Borrowing Programs
=====================================================================================================================================================================================================================

| Author       | Source       | 
| :-------------: |:-------------:|
|  [u/apegoneinsane](https://www.reddit.com/user/apegoneinsane/) | [Reddit](https://www.reddit.com/r/Superstonk/comments/ohivio/illegal_naked_shorting_techniques_employed_to/) | 

---


[DD 👨‍🔬](https://www.reddit.com/r/Superstonk/search?q=flair_name%3A%22DD%20%F0%9F%91%A8%E2%80%8D%F0%9F%94%AC%22&restrict_sr=1)

Reference: Full credit to Larry Smith that covered this back in 2019.

I will summarise the key points from my research into this.

Introduction

As we know the DTCC was set-up to take advantage of a paper free, electronic system. This has raised issues of transparency as the system is a closed loop, enabling an environment where manipulation can occur through naked shorting.

Regulation SHO was supposed to tackle naked shorting in the electronic clearing and settlement environment. However it has many loopholes that render it ineffective and the SEC themselves remain either intentionally or recklessly unconcerned about these loopholes.

Regulation SHO defines locate and settlement requirements for any borrowed stock that was used to execute short sales. There are also trading limits on threshold securities that have significant FTDs.

Normal participants must locate the stock before shorting it. Market makers are exempt from this and can do this without location. This type of naked shorting is aligned with the rules of Reg SHO and bizarrely 'legal'. It's only when the rules are not followed to the T, that it becomes illegal.

Any naked short should be located in a 2 day period before settlement. If it can't be, it creates a FTD. In this situation, a broker is supposed to close out the position in the open market. Market makers can maintain this for a longer 6 day period.

In reality, these rules are circumvented and we end up with synthetic shares that DTCC treats as real shares. You could create an infinite number of synthetic shares and overwhelm the stock market to drive down price. The SEC lacks the resources and seems disinterested in actively policing FTDs. Market Maker "A" may be able to just ignore the FTD without penalty.

Location

As above, broker-dealers are treated differently and allowed to do a short sale without having the stock.

Rule 203 (a) states that if broker dealers have *reasonable* grounds to believe that the security can be borrowed and delivered on or before the date that delivery is due, they can naked short.

There are 2 types of lists for borrowing:

1.  Easy to borrow - lists of securities that are generated and policed by prime brokers.

2.  Hard to borrow lists - intended to prevent naked shorting in stocks that appear on this list.

So a broker dealer can short stocks appearing on the easy to borrow list without first locating the shares to be delivered at settlement. If they do not, it is a FTD. The SEC maintains that repeated FTDs are grounds for removal of the stock from the easy to borrow list. Stocks on the hard to borrow "should" not be shorted before the stock is located.

As you can see, there is a lot of a ambiguity in the SEC's rules - particularly 203(a) and the "reasonable grounds" definition. As well as this, both lists are maintained by brokers and not the SEC. This makes the rules around them subjective and open to interpretation that can lead to manipulation.

There is an additional list which is the DTCC's stock borrow program - this will be covered in another post.

The SEC seems more concerned with maintaining liquidity than tackling naked shorting. The exemption that Reg SHO provides market makers is due to the belief that it is necessary to help with retail orders and maintain liquidity.

It has become increasingly hard to differentiate between market makers and hedge funds. Some operate as both, which is a strategic business model that can take advantage of the exemption above.

Close-out Requirement.

Rule 204 covers FTDs. If a failure occurs, this requires action by brokers and deals from whom the stock was borrowed by requiring them to buy and close out the stock on the market. Settlements will occurs on a T+2 basis.

There are even more exemptions to this rule. If a MM has a FTD but can show that this came from well intentioned market activities, the close out can be extended to T+5. If it is still not closed out, the MM can not perform more shorts until they have closed. Obviously, there are ways around this, which will be discussed.

Threshold Securities

Rule 203(B) outlines the creation and operation of threshold securities lists. These are securities that have large and persistent Fail to Delivers that are a hallmark of illegal naked shorting. These are defined as stocks that have an accumulated FTD position totaling 10,000 shares or more for five consecutive settlement days and is equal to at least 0.5% of the issuer's total shares outstanding. These are openly published by exchanges.

A stock on this list activates provisions in Reg SHO which are designed to eliminate FTDs. If the security is on the list for T+14, it must be closed out by purchasing the shares. The partidopant cannot perform more short sales without first locating or entering into an agreement. Market makers are not exempt from this.

*In practice, this is fucking bananas. Most stocks remain on the threshold list for months. The FTDs are rolled over from one broker to another. After T+13, even though they are required to close out, the market maker can transfer the position to another market maker or broker and the thirteen-day countdown to a mandatory buy-in starts all over.*

*This is frequently used to allows FTDs for months or years.*

Techniques Used to Circumvent Reg SHO

Given the SEC is content with the DTCC self-regulating its participants, there are frequently employed techniques to circumvent these requirements.

1.  Allowing "important" hedge fund clients to ignore the locate requirement

2.  Creating easy to borrow lists that inappropriately include threshold and hard-to-borrow stocks

3.  Hiding FTDs through washed and matched trades, i.e. rolling over an FTD to another broker

4.  Illegal stock sales in dark pools off the primary markets to avoid NYSE oversight and to maintain anonymity

5.  No supervision that the locate requirement was satisfied for short sales

6.  Fradulently marking short sales as long to hide naked positions.

7.  Fradulently saying they possessed the borrowed securities or had located them.

8.  Not making any effort to locate shares prior to short selling,

9.  Entering into a made up option contract to hide naked shorting

10. Using the DTCC stock borrowing program mentioned above as a means to conceal naked short sales,

11. Putting through fake short interest and other reports to regulators - as we see with Ortex.

12. Hiding activity by falsely reporting synthetic shares as real shares in broker statements

13. Hiding the activity by issuing voting material to shareholders with nonexistent assets who have no corporate rights including the right to vote shares,

14. Not complying with requirements to investigate and report suspicious transactions to regulatory authorities.

Elimination of the Uptick Rule

A big change in the governance of shorting was also the elimination of the uptick rule that required an increase in the stock price before allowing a short sale.

Bernie Madoff helped eliminate the uptick rule in 2007. Madoff had a MM and HF firm, which routinely participated in illegal naked shorting, as well as his ongong Ponzi Scheme.

The SEC defended this by saying the uptick rule reduced liquidity. Another example of the SEC prioritising liquidity over tackling predatory techniques and protecting investors. The SEC endorsed and defended the decision stating that the uptick rule reduced liquidity.

The Role of the DTCC

DTCC- US clearing and settlement services and a central securities depository.

DTC: a subsidiary and depository for almost all US securities and keeps records of transfers through electronic record-keeping of securities balances.

NSCC - a DTCC subsidiary that provides clearing and settlement for almost all securities transactions in the US two days after a transaction (T+2). It also guarantees completion of certain broker-to-broker securities transactions.

As we know the DTCC is owned by Prime Brokers. Prime brokers have hedge fund support which makes up a significant portion of their net income.

DTCC Performs a Critical Function but also Facilitates Illegal Naked Shorting

There are significant loopholes that facilitate an illegal enterprise. The subsidiaries use Continuous Net Settlement (CNS) and the Stock Borrowing Program to facilitate efficient liquid markets in securities. These have loopholes.

Market Makers can exploit these loopholes to create synthetic shares. Hedge funds can be involved in this but have plausible deniability as they don't execute the trades themselves.

The amount of synthetic shares and FTDs are staggering but the data is locked deep inside the DTCC, which allows it to circumvent regulatory oversight and reporting. This gives it an effective monopoly which can work to the benefit of Prime Brokers and as a fuck you to everyone else.

The process of creating synthetic shares is complex and understanding all aspects usually requires a team of highly skilled lawyers specialising in securities law, clearing and settlement procedures.

1.  Physical Transfer of Stock Certificates Has Been Replaced by Electronic Data Entries. Stock certificates are now stored in a central vault in the DTC. When an investor buys a security through a broker, the investor's name does not appear on the stock certificate. They are categorised by the broker dealers, called a "street name".

2.  The actual custody, physical control and even the official ownership of stocks (and other securities) is done through Cede and Company, which processes on behalf of DTC. This is another private company in partnership with the DTCC so technically Cede own all listed shares in the US and all investors have are contractual rights.

This has some advantages - rapid settlements. But this is also non-transparent. It is a mind fuck that the SEC has been happy waiving control of clearing, settlements and custody to a private company. In theory, number of street name shares = registered shares in Cede's vault. In reality, Wall Street creates massive numbers of synthetic shares. Once created, the DTCC does not differentiate between synthetic and real street name shares.

It also means that "*while you may think you are buying registered stock, you are actually buying a financial derivative. Effectively, you are buying a financial derivative from brokers of a financial derivative they hold from Cede that is just a digital entry in your DTC account."*

You own fungible derivatives and untraceable commodities.

> Operating in this black hole of important information they use loopholes in the clearing and settlement system administered by DTCC and loopholes in the ineffective SHO regulations to create counterfeit shares at will. They can and do expand the supply of street name securities through creating counterfeit shares to overwhelm demand and drive down the stock price.
>
> You can see this scheme at work almost on an almost daily basis. All too often, when a Company reports approval of an important new product, the stock trades up slightly and then trades down to a lower price than before the announcement  to the amazement of investors who are long the stock. The same thing can happen with achievement of a meaningful, clinical, regulatory or financial milestone. Why? Because there are hedge funds who have been shorting the stock and have huge outstanding short positions who stand to suffer huge losses if the stock price increases. In self-defense, they launch a short attack spearheaded by creating counterfeit shares arising from illegal naked shorting. The clear intent is to make good or great news appear to be badly received. Jim Cramer was a long time hedge fund manager before becoming a commentator on CNBC. In this famous [interview](https://www.youtube.com/watch?v=gMShFx5rThI),  he fills us in on how he and other hedge funds routinely manipulated stocks.
>
> God forbid, if a company you are invested in reaches a point that it becomes apparent that it has to raise equity. The hedge fund gang jumps in and start shorting in anticipation of an offering. The hedge funds have had great success in persuading other investors that equity offerings are bad for investors because it dilutes their shares. In most cases, this argument is total nonsense because companies are raising money to enable the completion of projects that will enable them to become successful, i.e. executing an important clinical trial, building infrastructure, etc. Raising equity to enable companies to grow is the cornerstone for our successful economic system. Claiming that equity raises are dilutive and harmful is something that Vladimir Lenin might have said.
>
> In the vast majority of cases, the stock slides sharply when the deal is announced. For small emerging companies, the offering is then priced by Wall Street investment bankers at a 10% discount to the already distressed price and often warrants must be attached in order to attract buyers who all too often the hedge funds who have shorted the stock. Yes, I know this is illegal, but hedge fund A buys stock on an offering to cover for hedge fund B who has been shorting and they switch positions to cover the short and split the profits. This is a routine practice. In the end, this does lead to enormous share dilution, which causes untold harm to investors and emerging companies who are so important to economic growth. The winners are Wall Street and hedge fund employees and real estate brokers in the Hamptons.

Continuous Net Settlement System Used by the NSCC

In the old days, if you bought a stock from another investor, you would own the stock certificate. Given the sheer size and complexity of electronic transactions that is here in the modern age, the solution by the NSCC was to not handle each trade individually but to use a system called Continuous Net Settlement (CNS). This centralised and automated the accounting of settlements.

In the CNS system, Prime Brokers have an account with the DTC along with market makers, hedge funds etc. Everything is electronic and in real time so you can immediately see the status of specific investments in accounts.

The clearance and settlement system of the NSCC functions through a system called multilateral netting.

You have a customer order. Broker A buys 10 shares of GameStop from Broker B. Then later Broker A sells 10 shares of GameStop to Broker B. In the new approach, these 2 trades are netted so there is no movement in the electronic certification. In the real world, there would be complex trading with multiple buy/sell with multiple participants for GameStop stock.

NSCC settlement T+2. At this time, all NSCCs member are netted for the stock in question. They are further netted against any previous trades in which there were failed to deliver securities. If the Prime Broker has sold more shares than it has bought (net short), it owes shares to the NSCC. The inventory of XYZ in the broker's account at the DTC is checked to see if there are available shares that can be transferred to cover the short obligation. In the case of net long positions, they are automatically credited to the member's DTC account. Also, daily money settlements are debited or credited to the member's account.

Example: During the day Broker A might handle multiple transactions in a stock for its customers as follows:

1.  Sells 500 shares to Broker B

2.  Buys 1000 shares from Broker C

3.  Sells 2000 shares to Broker D

4.  Has 500 shares of XYZ on deposit at its DTC account

Broker A at settlement (T+2) is net short 1000 shares of XYZ (-500+1000-2000+500) and turns to the Stock Borrowing Program.

NSCC's Stock Borrow Program

When a broker is net short, it has T+2 to locate and deliver. But as above, there could be a situation where a broker is net short of XYZ on settlement day and does not have enough shares of XYZ in inventory to cover. I

Under CNS, the NSCC guarantees the trade so that even if the seller of the stock fails to deliver, the transaction goes through. This can be used to create counterfeit share.s

The DTC knows every member's position. If a member is net short, the DTC reviews the number of net shorts of the shares of the XYZ to determine if the DTC itself holds enough to settle. If there are enough, the DTC offsets the net short and the shares are sent to the account of members who loaned them.

If the member does not have enough to cover, the NSCC will borrow through their Stock Borrow Program.

This allows members with net long positions to lend out shares to members who are net short. So Broker A who is net long on GameStop can put it in the program and Broker B can loan it as it has a net short position and needs to cover. The program is continuously updated by members stating how many shares they are OK lending. Once this is established and covered, this cures the failures to deliver at settlement.

Creating Counterfeit Shares through the Stock Borrow Program

This is of course abused through loopholes.

Example:

> Let's assume that the parties in a hypothetical example are Hedge Fund A, Broker A, Investor B, Broker B, a market maker and the DTC and NSCC. Let's look at a highly simplified example in which Hedge Fund A asks broker A to short 2,000 shares of XYZ at $10.00 per share.
>
> 1.  Broker A transmits Hedge Fund A's short sell order to a Market Maker in XYZ stock (this could be either the broker itself or another market maker.)
>
>
> 2.  The Market Maker confirms immediately to Broker A that the trade is complete without first locating the shares; he is naked short the stock. Under Regulation SHO this is legal.
>
>
> 3.  Investor B through Broker B buys the 2,000 shares offered by the Market Maker at $10.00 even though the market maker has not located 2,000 shares to borrow.
>
>
> 4.  If at T+2, the Market Maker still hasn't found a locate, he is in a fail to deliver situation. In the system of the 1960s, the trade would have been broken and $20,000 would be returned to Investor B's account, but because the NSCC guarantees all transactions, the stock borrowing program comes into play and the settlement proceeds with the NSCC borrowing stock from other member firms.
>
>
> 5.  The DTC identifies Broker C having a net long position of 2,000 shares which it is willing to lend to NSCC.
>
>
> 6.  At settlement (T+2), Hedge Fund A's account at the DTC is credited with cash of $20,000 (2,000 shares at $10.00). Investor B's account at the DTC is now credited with owning 2,000 shares of XYZ at $10.00 even though the market maker failed to borrow the shares. Broker C is credited to receive interest on $20,000, the value of the stock it has loaned.
>
>
> 7.  Broker C loaned 2,000 shares of XYZ, which it took from its customer accounts, to the NSCC. However, the NSCC accounting credits customers of Broker C with still owning 2,000 shares of XYZ.
>
>
> 8.  This is the critical point at which counterfeit shares have been created. The NSCC shows customers of Broker C as still owning the 2,000 shares of XYZ. However, Investor B is credited as owning the same 2,000 shares. Presto, there are 2,000 new counterfeit shares outstanding that were never issued by the Company.
>
>
> 9.  Under Reg SHO, the Market maker has until T+6 to locate stock and close out the 2,000 shares of XYZ it has borrowed through the stock borrow program from Broker C. Under Regulation SHO, if a locate has still not been found at T+6, the Market Maker must purchase 2,000 shares in the open market and return them to Broker C. However, Wall Street has a bag of tricks to get around this requirement. One of which is simply to ignore it. Another is to roll the position to another broker-dealer. Oftentimes, fails to deliver can last for months or years. The SEC seems strangely unwilling or unable to enforce this provision of Regulation SHO.

If the FTD is not addressed, the NSCC system does not differentiate between synthetic and real shares. Both the 2,000 legitimate shares that were originally in the customer accounts at Broker C and the 2,000 new unauthorized (counterfeit) shares given to Investor B can both be loaned to cover other net short, fail to deliver positions. This process can be repeated ad infinitum to flood the market with counterfeit shares.

There are many ways that this process directly benefits Wall Street at the expense of retail shareholders. Shares loaned by Broker C to make good on the Market Maker's delivery obligation actually do not belong to Broker C. They come from customer's margin accounts who do not know their shares are being loaned. Meanwhile, the Broker is receiving interest on the cash value even though they have no ownership. The customers receive no economic value. The interest of the Broker is to see the price rise. Loaning to short sellers who want the stock to go down is against their interest. With the stock borrowing program, brokers put their own economic interest before their customers.

Why Do It?

Shorting is extremely popular amongst Hedge Funds. Firms benefit from lending through the collection of interest and associated fees. Estimates are that 20% of net income for large investment banks comes from shorting selling.

Issues:

1.  Liability is unlimited - if you buy a stock, your lose is capped at your investment. If you short a stock, there is no limit to your liability.

2.  Kalo Bios was about to go bankrupt and trading at $0.25 per share. An investor shorted 4000 shares, thinking they could could $1000. Martin Shkreli came in and initiated short squeeze that drove the stock to $40. 00 per share. The investor ended up with a loss of about $160,000 based on a $1,000 investment.

3.  Short sellers have ongoing costs via interest on a loan. If the stock price increase,s more collateral and cash is required and the interest increases. This creates a sense of urgency when shorting.

4.  You have to have incredible timing. If you buy and hold, there is no cost for you. If you short, there is an ongoing cost. The short seller has to have precise timing .

5.  Over the long term, buying is a winning result and shorting is a losing result.

6.  Shorting is anti-social - you are selling something you don't own to drive down the price of a company so that everybody loses (the investors, the employees, the business, the customers)

The Implications of FTDs

> Here is what happens when an FTD is rolled over, no buy-in occurs or is simply ignored. Let's use an example when Market Maker "A" receives an order to short 10,000 shares of XYZ at say $20.00, but can not immediately locate shares to borrow:
>
> 1.  A hedge fund delivers an order to short 10,000 share of XYZ to Market Maker "A"
>
>
> 2.  Market Maker "A" immediately shorts 10,000 shares without locating shares to borrow.
>
>
> 3.  Some customer(s) of Broker "X" buys the shares.
>
>
> 4.  The hedge fund receives $200,000 in cash from the customer(s) of Broker "X" at T+2.
>
>
> 5.  However, at T+2. Market Maker "A" has not located shares to borrow and deliver to the customers of Broker "X".
>
>
> 6.  NSCC steps in to guarantee the settlement of the trade. It borrows 10,000 shares from a customer(s) of Broker "Y".
>
>
> 7.  These 10,000 shares of XYZ are credited to the customer(s) of Broker "X". They now show 10,000 shares of XYZ in their accounts.
>
>
> 8.  The problem is that the NSCC borrowed 10,000 shares of XYZ from customers of Broker "Y" and they are also credited with owning 10,000 share of XYZ.
>
>
> 9.  The customers of Brokers "X" and "Y" own the same 10,000 shares. This is how counterfeit shares are created.
>
>
> 10. Because of continuous net settlement used by member firms of the DTCC, these shares are commingled in the inventory of the Brokers "X" and "Y" and can't be traced to individual accounts.
>
>
> 11. Customers of Broker "X" now own 10,000 counterfeit shares of XYZ, but they can't be distinguished from legal street name shares.
>
>
> 12. These 10,000 counterfeit shares can be loaned out to other short sellers.
>
>
> 13. Market makers and hedge funds working in concert can create a virtually unlimited number of counterfeit shares.

Acknowledgements - [https://smithonstocks.com](https://smithonstocks.com/comp/)
