Writeup Summary on the Proposed SEC Rule Change for the NYSE
============================================================

| Author       | Source       | 
| :-------------: |:-------------:|
|  [u/Insertions_Coma](https://www.reddit.com/user/Insertions_Coma/) | [Reddit](https://www.reddit.com/r/Superstonk/comments/mlgasb/writeup_summary_on_the_proposed_sec_rule_change/) | 

---

[Serious DD 👨‍🔬🔬](https://www.reddit.com/r/Superstonk/search?q=flair_name%3A%22Serious%20DD%20%F0%9F%91%A8%E2%80%8D%F0%9F%94%AC%F0%9F%94%AC%22&restrict_sr=1)

I want to preface this by saying that I have 0 qualifications in any related field, so please take what I say with a grain of salt. I am just an ape who has been trying to figure out what's going on for the past 4 months. Please reply with any mistakes or misconceptions that I have so that I may amend my post. I do not wish to feed anyone false data based on my own misunderstandings. I take feedback as a chance to improve and better understand the situation. I will only be covering the [proposed rule changes to the NYSE](https://www.federalregister.gov/public-inspection/2021-07114/self-regulatory-organizations-proposed-rule-changes-new-york-stock-exchange-llc) as there are far too many propositions here to cover. This IS NOT all of the proposed rule changes listed.

Definition of an ISO: *Intermarket sweep orders (ISO) is a type of stock market order that sweeps several different market centers and scoop up as many shares as possible from them all.*

Below is the current rules on how an ISO affects best bid/ask.

Current rule:

[Intermarket Sweep Order Exception.](https://nyseguide.srorules.com/rules/document?treeNodeId=csh-da-filter!WKUS-TAL-DOCS-PHC-%7B4A07B716-0F73-46CC-BAC2-43EB20902159%7D--WKUS_TAL_19401%23teid-47)

1.  *The Exchange will accept ISO orders to be executed in the Exchange Book against orders at Exchange's best bid or best offer* *without regard to whether the execution would trade through another market's Protected Quotation.*

2.  *If an ISO is marked as "Immediate-or-Cancel," any portion of the order not executed upon arrival will be automatically cancelled. If an ISO is not marked as "Immediate-or-Cancel," any balance of the order will be displayed by the Exchange without regard to whether that display would lock or cross another market center if the member organization has complied with Rule 7.37(f)(3)(C).*

Sooooo... the way I read this is that as of right now, Away Market ISO orders will come into the DTC as bids and offers, and regardless of if it is canceled or unfilled, it still affects the way in which the DTC would calculate and send out the updated best bid/ask back to the Away Markets (based on there being no ruling stating otherwise). The new ruling seems to be addressing this (more later).

I have heard of this issue somewhere on an old thread on [r/GME](https://www.reddit.com/r/GME/) (link it if you can find it). And if I recall correctly, it allows Market Makers to abuse this by sending orders they know won't be fully filled in order to drive the current best bid/ask up or down that is being reported to all the Away Markets without having to fill those orders at all.

Section 1 of new rule proposal:

[Link to proposed rule changes.](https://public-inspection.federalregister.gov/2021-07114.pdf)

*As proposed, new paragraph (e)(1) of Rule 7.37 would provide: The Exchange may adjust its calculation of the PBBO based on information about orders it sends to Away Markets with protected quotations, execution reports received from those Away Markets, and certain orders received by the Exchange. This proposed rule text is consistent with the Exchange's disclosure in the Data Feed Filing and adds specificity that* *the Exchange may adjust its calculation of the PBBO based on execution reports received from Away Markets and certain orders received by the Exchange.*

This is the summary of the proposed rule change. By the language I've bolded above, it would seem as though they are attempting to change which types of orders end up affecting the best bid/ask calculation coming from the DTC to the Away Markets.

Section 2:

*MEMX has not disclosed circumstances when "certain orders received by the Exchange" would result in an adjustment to its calculation of the PBBO, but the Exchange believes that when MEMX receives an ISO with a Day time in force ("Day ISO"), it adjusts its calculation of the PBBO.* *The Exchange proposes that it would also adjust its calculation of the PBBO based on receipt of a Day ISO*, *which is consistent with how Nasdaq Stock Market LLC ("Nasdaq")8 and Cboe BZX Exchange, Inc. ("BZX")9 function. Specifically, the Exchange proposes that it would adjust its calculation of the PBBO upon receipt of a Day ISO Order that the Exchange displays. As described in Rule 7.37(f)(3)(C), a Day ISO is eligible for the exception to locking or crossing a protected quotation because the member organization simultaneously routes an ISO to execute against the full size of any locked or crossed protection quotations, i.e., the member organization routes ISOs to trade with contraside protected quotations on Away Markets that are priced equal to or better than the arriving Day ISO on the Exchange. Because receipt of a Day ISO informs the Exchange that the member organization has routed ISOs to trade with Away Market contra-side protected quotations priced equal to or better than the Day ISO, upon receipt and displaying of a Day ISO,* *the Exchange proposes to adjust its calculation of the PBBO to exclude any contra-side protected quotations that are priced equal to or better than the Day ISO.*

Based on what I've bolded above, It looks to me that if a Market Maker submits best offers/bids that are not in line with the current best bid/ask provided by the Day ISO from the DTC, then they will no longer affect the current Day ISO calculation which determines the overall markets best bid/ask.

Closing statement:

*The Exchange believes that the proposed amendments to Rule 7.37(e) would promote clarity and transparency in the Exchange's rules regarding circumstances when the Exchange may adjust its calculation of the PBBO. The Exchange does not believe this proposed rule change is novel. Rather, the Exchange believes that other equity exchanges that accept Day ISOs similarly adjust their calculation of the best protected bid and best protected offer for purposes of making execution, routing, and repricing determinations based on the receipt of Day ISOs, as described above.* *The Exchange anticipates that it will implement the technology change to how it calculates the PBBO in May 2021.*

*The Exchange believes that the proposal is consistent with Section 6(b) of the Act,12 in general, and furthers the objectives of Sections 6(b)(5) of the Act,13 in particular, because it is designed to prevent fraudulent and manipulative acts and practices, to promote just and equitable principles of trade, to foster cooperation and coordination with persons engaged in regulating, clearing, settling, processing information with respect to, and facilitating transactions in securities, to remove impediments to, and perfect the mechanisms of, a free and open market and a national market system and, in general, to protect investors and the public interest and because it is not designed to permit unfair discrimination between customers, issuers, brokers, or dealers.*

I've included the above section from the closing remarks. It is clear that the identified problem lies with Market Makers being able to change the best bid/ask.

TLDR:

-The proposed rule change would not allow Market Makers to affect the best bid/ask by simply submitting ISO orders that would not be fully filled or not filled at all.

-It seems clear that there is a problem with Market Makers being able to play the best offer/bid system in place by the DTC.

Speculation/Conclusion:

If I were an abusive Market Maker and I wanted to drive the price of a stock up or down, the traditional method is to do what's called "hitting the bid". Which as I understand it is basically when you start trickling in sell offers that are below the current best ask. This in turn starts moving the price down. Now if you really want to do this right and also not spend any of your own cash to drive the price down, you would put your ask in well below the current ask so far down that it isn't likely to even be filled. The current problem is that even though these don't get filled, they still change the way in which the best ask price is calculated by the DTC. This is an inherent flaw in the system as it totally breaks the common law of supply and demand. It would arbitrarily allow you to move the price of the stock based on orders that won't/arent likely, to fill. The proposed rule change sounds like it would be very beneficial and would ensure that only completed transactions affect the current best bid/ask sent to the exchanges.

My original comment and thread can be found [here.](https://www.reddit.com/r/Superstonk/comments/mlc4qn/the_dtcc_just_filed_7_new_rules_and_rule_changes/) Credit to [Squashua1982](https://www.reddit.com/user/Squashua1982/) for the links.

Edit 1: [Leaglese's reply from original comments.](https://www.reddit.com/r/Superstonk/comments/mlc4qn/the_dtcc_just_filed_7_new_rules_and_rule_changes/gtla04x?utm_source=share&utm_medium=web2x&context=3)
