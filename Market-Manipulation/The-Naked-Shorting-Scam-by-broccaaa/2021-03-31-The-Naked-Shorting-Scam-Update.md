The naked shorting scam update: selling nude like its 2021
==========================================================

| Author       | Source       | 
| :-------------: |:-------------:|
| [u/broccaaa](https://www.reddit.com/user/broccaaa/) | [Reddit](https://www.reddit.com/r/GME/comments/mh6lnz/the_naked_shorting_scam_update_selling_nude_like/) | 

---

[DD 📊](https://www.reddit.com/r/GME/search?q=flair_name%3A%22DD%20%F0%9F%93%8A%22&restrict_sr=1)

This post is an update to the one I posted yesterday on [r/GME](https://www.reddit.com/r/GME/) and [r/Wallstreetbetsnew](https://www.reddit.com/r/Wallstreetbetsnew/). I hope to address some of the minor criticisms that were raised and use updated references for interested apes to look into.

TLDR: This post updates the possibility of a naked shorting scam with massive hidden FTDs and short interest in 2021. By looking at SEC rules and academic papers I show that rule changes do not stop the potential abuses of naked short selling in a material way. Rather they slightly modify how it could be done and optimized. The changes also make the scheme less sustainable on the short side and over time pressure might "coil the spring" and lead to an [unprecedented FTD squeeze](https://iamnotafinancialadvisor.com/Current-DD/).

With current rules:

1.  Synthetic shares can still be sold to hedge funds as part of a married put trade (or reverse conversion)

2.  The borrowed privileges now only relate to the "bona-fide" market makers exemption from locate requirements

3.  Rather than being able to flood the market with synthetics and let them build up indefinitely, once a security is on the threshold list market makers are forced to cover (after a certain time period)

If mass naked shorting and married put trades were being carried out in GME this could explain:

-   the "BUG" bids as being part of "bone-fide" requirements to be "regularly and continuously placing quotations [..] on both the bid and ask side of the market"

-   short interest manipulation

-   how naked short selling has become so widespread

-   why borrow fees can still be so ridiculously low (low demand for located shares to borrow)

-   that the vast majority of options (both puts and calls) might be due to naked short selling

-   how short shares are 'washed' and able to be dumped on the market even during SSR

-   why such a large number of way out of the money calls have been seen recently (actually part of a naked short trick, not long whales or gamma ramps)

-   the vast number of trades in OTC / Dark Pools as part of married put trades

🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀

*Note: this is not financial advice. I am not a cat. I read some papers and made some interpretations. Any number of these could be flawed and wrong. Make your own mind up.*

Introduction

The [post I wrote yesterday](https://www.reddit.com/r/GME/comments/mgj0j1/the_naked_shorting_scam_revealed_lending_of/) was based on an economics paper looking at naked short practices that abused options market maker privileges. The paper was written in 2007 and took Overstock shares as an example of of a stock with massive short share fuckery. Here is a great [Rolling Stone article](https://www.rollingstone.com/politics/politics-news/accidentally-released-and-incredibly-embarrassing-documents-show-how-goldman-et-al-engaged-in-naked-short-selling-244035/) showing court documents confirming the illegal short seller activity in Overstock. Despite the clear similarities with GME in 2021certain SEC rules have changed since the paper was written.

*Which short selling rules have changed and could a modified version of the scam be happening in 2021?*

With some help from other apes in the comments and a little extra research I'd like to clarify this and provide some thoughts on what might be going on today.

SEC rules on short selling and the changes made up until 2006 ( amendments to Regulation SHO under the Securities Exchange Act of 1934 )

Regulation SHO, which became fully effective on January 3, 2005, set forth a regulatory framework governing short sales. One of the goals of this was to target potentially abusive "naked" short selling practices in certain equity securities. Additional regulation was put in place to limit the selling of securities without first finding a valid share to borrow. The 2005 implementation failed miserably.

A [fantastic letter](https://www.sec.gov/rules/proposed/s72303/sonecon010504.txt) was written in December 2003 by former Undersecretary of Commerce Robert Shapiro and forwarded to the SEC. In the letter Shapiro detailed findings from his own research and his doubts that the proposed changes in the SEC rules would have any material impact on the abusive practices:

> In my judgment, the proposed regulations would not significantly reduce short sale abuses. To have a genuine impact on the efficiency and competitiveness of the equity markets, the regulations should provide much stronger disincentives for naked short sales. The integrity of the capital markets demands much stricter regulation than those currently proposed, much greater industry compliance than has occurred of late, and much tighter enforcement than has been seen thus far.

The [SEC allowed for two exceptions in their ruling](https://www.sec.gov/rules/final/2008/34-58775.pdf), the second of which was highlighted as the source of abuse in my previous post:

> As adopted in August 2004, Rule 203(b)(3) of Regulation SHO included two exceptions to the mandatory close-out requirement. The first was the "grandfather" provision, which excepted fails to deliver established prior to a security becoming a threshold security. *The second was the "options market maker exception," which excepted any fail to deliver in a threshold security resulting from short sales effected by a registered options market maker to establish or maintain a hedge on options positions that were created before the underlying security became a threshold security.*

Note that Rule 203(b)(3) of Regulation SHO relates to the close out requirements when large FTDs pile up. The exception that was in place up until 2008 allowed option market makers to completely ignore the closing of their position even in the presence of huge FTDs!!

The Commission noted that it would look for evidence for whether the options market maker exception for closing FTDs was operating significantly differently from their original expectations. Just a few years later the SEC realized their rules we're still being abused and started updating them again (also from [here](https://www.sec.gov/rules/final/2008/34-58775.pdf)):

> To the extent that fails to deliver might be part of manipulative "naked" short selling, which could be used as a tool to drive down a company's stock price, such fails to deliver may undermine the confidence of investors. These investors, in turn, may be reluctant to commit capital to an issuer they believe to be subject to such manipulative conduct. In addition, issuers may believe that they have suffered unwarranted reputational damage due to investors' negative perceptions regarding fails to deliver in the issuer's security. Unwarranted reputational damage caused by fails to deliver might have an adverse impact on the security's price...
>
> ...With respect to the options market maker exception [...] we *reproposed amendments to eliminate the exception*. In addition, the Commission sought comment on two alternative proposals that would require options market maker fails to deliver to be closed out within specific time-frames...
>
> ...[to achieve] our goal of further reducing fails to deliver and addressing potentially abusive "naked" short selling, we believe that *we must eliminate Regulation SHO's options market maker exception*.

So after making new rules, then amending those rules, then looking at how well they worked, they realized the initial problem was not fixed.

Talk about taking your time to fix an issue that you acknowledge should be illegal and is highly detrimental to the market.

Updated SEC rules for short selling in 2008

A detailed and fairly easy to read description of the updated SEC rules in 2008 can be found [here](https://www.sec.gov/rules/final/2008/34-58775.pdf). It also has background info on previous rules.

Prior to updating the rules on options market maker FTD exceptions the SEC sought comment letters from interested parties:

> One commenter stated that it believes that the current options market maker exception "*harms investors and issuers, hinders the formation of capital, and is fatally flawed as written*" and that it should be eliminated. Another commenter stated that the options market maker exception "is a *well known tool of manipulators* *and must be removed to ensure a level playing field for public companies and their shareholders*." One commenter that supported the amendments noted that "*options market makers should factor the cost of borrowing stock and selling short into the price of the put options being sold*." Commenters also stated that 13 consecutive settlement days was more than sufficient to close out a fail to deliver relating to an options position.

On the other side of the debate:

> Commenters who opposed the proposed amendments generally criticized the impact of elimination on options market making risk, quote depths, spread widths, and market liquidity in threshold securities and securities that might become threshold securities. Among other things, they stated that the options market maker exception is integral to the options market maker's ability to make markets and manage risk and that, without the exception, making continuous markets would be very difficult, particularly in longer-dated options. One commenter suggested that "*withdrawing or greatly reducing the exception would cause varying losses of liquidity in over 20% of listed options and their underlying stocks*."

Of course it would decrease liquidity if your ABILITY TO PRINT SYNTHETIC STOCKS AT WILL WERE REDUCED!!!

The other comments basically say that market makers would have a hard time guaranteeing that they make guaranteed profits. There is a balance here as market making serves a purpose, but this topic is about the reduction of widespread strategic FTD short selling that endangers the market.

After considering comments and data on FTDs the SEC stated that:

> We believe that it is *appropriate to eliminate Regulation SHO's options market maker exception* because substantial levels of fails to deliver continue to persist in threshold securities and it appears that a significant number of these fails to deliver are as a result of the options market maker exception.

So the market maker exception for closing out FTDs was eliminated. Problem solved, right?

Rules changed, problem fixed. WRONG!

The elimination of the options market maker exception for closing out FTDs did help to reduce the number of FTDs in threshold securities (reference [here](https://www.sciencedirect.com/science/article/abs/pii/S1386418112000171)). However market makers have additional privileges when it comes to naked short selling...

The "bona-fide" market making exception of locating shares before you sell them!!!

> Rule 203(b)(1) provides that "[a] broker or dealer may not accept a short sale order in an equity security from another person, or effect a short sale in an equity security for its own account, unless the broker or dealer has: (i) Borrowed the security, or entered into a bona-fide arrangement to borrow the security; or (ii) Reasonable grounds to believe that the security can be borrowed so that it can be delivered on the date delivery is due; and (iii) Documented compliance with this paragraph (b)(1)." This is known as the "locate" requirement. *Rule 203(b)(2)(iii) excepts market makers engaged in bona-fide market making activities from the locate requirement*.

So "bona-fide" market makers are exempt from locating any shares before selling them. They don't even need to bother pretending they have a "*reasonable grounds to believe that the security can be borrowed*". They want to sell shares they don't have, no problem! As long as they're "bona-fide".

This means that "bona-fide" market makers can short sell stock with complete exception as part of their business. The privilege they lost in 2008 simply means that they cannot continue to hang onto the FTDs indefinitely with no intention of covering any more.

Furthermore we continue to have evidence of:

-   [Additional naked short selling when it suits funds around earnings calls (2016)](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=2867383),

-   [Continued short selling, fails-to-deliver, and abnormal returns (2016)](https://www.sciencedirect.com/science/article/abs/pii/S092753981630055X)

Did you really think they would give up the free money scheme *that* easily??

What is a "bona-fide" market maker

Seems like people don't really know. The SEC tried to clarify ([page 30](https://www.sec.gov/rules/final/2008/34-58775.pdf)) things as follows:

> The term "market maker" includes any specialist permitted to act as a dealer, any dealer acting in the capacity of a block positioner, and any dealer who, with respect to a security, holds itself out (by entering quotations in an inter-dealer quotation system or otherwise) as being willing to buy and sell such security for its own account on a regular or continuous basis.
>
> Moreover, as the Commission has stated previously, a market maker engaged in bona-fide market making is a "broker-dealer that deals on a regular basis with other broker-dealers, actively buying and selling the subject security as *well as regularly and continuously placing quotations in a quotation medium on both the bid and ask side of the market*."

Well that wasn't very fucking helpful. So they act as a dealer and deal with other dealers while actively buying and selling a security. Looks like a pretty low bar to be allowed to print synthetic shares outside of the normal rules.

Even [experts in the field](https://www.mmlawus.com/newsitem/pdf/joic-04-2017-0019_8757744610889.pdf) have a hard time understanding the definition:

> While there is still a lot of room for additional SEC guidance on what constitutes bona-fide market making, the SEC has provided some details on the specific type of trading that would not fall within the Regulation SHO exceptions applying to bona-fide market making activities. However, there is still a large gap between the type of activity that most likely falls within the exception and the concrete examples analyzed by the SEC.

WHY ARE ALL THE RULES AND DEFINITIONS SO UNCLEAR?!??

It must be by design. Who would think "reasonable grounds to believe that the security can be borrowed" provides clear guidance? Why is a "bona-fide" market maker so hard to describe yet they have exceptional privileges?

Some speculation. Let's look at the quote:

> as well as *regularly and continuously placing quotations* in a quotation medium *on both the bid and ask side* of the market

COULD THIS BE PART OF THE BUGS WE ARE SEEING WHERE THE BONE-FIDE PLAYERS NEED TO REVEAL THEIR POSITIONS?!?!

The naked shorting scam updated for 2021

We've seen that in the years since the method I described [yesterday](https://www.reddit.com/r/GME/comments/mgj0j1/the_naked_shorting_scam_revealed_lending_of/) was being used circa 2007 some rules have changed to reduce options market maker privileges. This is a summary of the changes:

-   As of 2008 market maker exception for closing out FTDs was eliminated

-   In 2021 "bona-fide" market makers are still exempt from locate requirements, allowing them to naked short sell their shares

How does this impact the scheme described previously?

1.  Synthetic shares can still be sold to hedge funds as part of a married put trade (or reverse conversion)

2.  The borrowed privileges now only relate to the "bona-fide" market makers exemption from locate requirements

3.  Rather than being able to flood the market with synthetics and let them build up indefinitely, once a security is on the threshold list market makers are forced to cover

So the new rules do not change the potential scheme in any material way. There is now more risk on the market makers but if they can manage their FTDs they can keep trying to roll them over as before. Does this sound [familiar](https://iamnotafinancialadvisor.com/discord/DD/og/GMEv13.pdf)?

[![r/GME - The naked shorting scam update: selling nude like its 2021](https://preview.redd.it/v5zkyg2x4dq61.png?width=1419&format=png&auto=webp&s=c0c48d441bb8cc46f497775a757dcb5e0c321c0c)](https://preview.redd.it/v5zkyg2x4dq61.png?width=1419&format=png&auto=webp&s=c0c48d441bb8cc46f497775a757dcb5e0c321c0c)

The FTD squeeze theory from https://iamnotafinancialadvisor.com/Current-DD/

If a market maker were to manage their FTD deliverables using the above method, or something similar, then in effect they have side stepped the new rules and can delay delivering shares as before.

The difference with GME is that they NEVER prepared for a situation with this much attention and so many hungry apes. I implore you to read the [full PDF thesis about the FTD squeeze](https://iamnotafinancialadvisor.com/discord/DD/og/GMEv13.pdf). Probably the best overview we have of GME and very much backs up how much rocket fuel is being pumped in as "the springs coil tighter".

Conclusion

Previous updates to SEC rules were shown to be insufficient at reducing unwarranted naked short selling. The rule updates in 2008 eliminated the exemption that allowed market makers to never close FTDs for securities with high FTDs. Today "bona-fide" market makers still have a key privilege that lets them sell synthetic shares without the locate requirement. Naked short selling.

These changes do not eliminate the potential for naked shorting schemes being run by "bona-fide" market makers or in coordination with short hedge funds using the married put options play. If these methods were being widely used it would help to explain:

-   how short interest has been manipulated in official reporting numbers

-   how naked short selling has become so widespread

-   why borrow fees can still be so ridiculously low (low demand for shorts that have been located)

-   that the vast majority of options (both puts and calls) might be due to naked short selling

-   how short shares are 'washed' and able to be dumped on the market even during SSR

-   why such a large number of way out of the money calls have been seen recently (actually part of a naked short trick, not long whales or gamma ramps)

-   the vast number of trades in OTC / Dark Pools as part of married put trades

-   the "BUG" bids as being part of "bone-fide" requirements to be "regularly and continuously placing quotations [..] on both the bid and ask side of the market"

This is one possible way in which the short interest is being hidden and the short shares being continuously sold, even when very hard to borrow on official channels. The rule changes do not prohibit such schemes, they would just need small modifications.

As the pressure builds it won't take much for the spring to sprung. Nothing has changed. I HODL!!

🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀

Some references and further reading:

-   [The 'Phantom Shares' Menace (2008)](https://web.archive.org/web/20190623164454/http://rgmcom.com/articles/PhantomShares.pdf)

-   [What is a Regulation SHO bona-fide market maker? (2017)](https://web.archive.org/web/20190623164454/http://rgmcom.com/articles/PhantomShares.pdf)

-   [(Naked) Short Selling Around Earnings Announcement (2016)](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=2867383)

-   [Three Essays on Naked Short Selling and Fails-to-Deliver (2013)](https://search.proquest.com/openview/b7759a0d7c621f67d82668197d99c379/1?pq-origsite=gscholar&cbl=18750&diss=y)
