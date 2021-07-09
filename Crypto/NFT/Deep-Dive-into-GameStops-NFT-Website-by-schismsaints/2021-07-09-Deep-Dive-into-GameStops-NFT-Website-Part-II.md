A Deep Dive into nft.gamestop.com - Part 2: Electric Boogaloo
=============================================================

| Author      | Source | 
|  :----:     |    :----:   |        
| [u/schismsaints](https://www.reddit.com/user/schismsaints/) | [Reddit](https://www.reddit.com/r/Superstonk/comments/oh0zfe/a_deep_dive_into_nftgamestopcom_part_2_electric/) |

---


[DD 👨‍🔬](https://www.reddit.com/r/Superstonk/search?q=flair_name%3A%22DD%20%F0%9F%91%A8%E2%80%8D%F0%9F%94%AC%22&restrict_sr=1)

[![r/Superstonk - A Deep Dive into nft.gamestop.com - Part 2: Electric Boogaloo](https://preview.redd.it/lzsb9ky2h7a71.png?width=225&format=png&auto=webp&s=8d709e3952f111fa21f696a57a2c7a0104475412)](https://preview.redd.it/lzsb9ky2h7a71.png?width=225&format=png&auto=webp&s=8d709e3952f111fa21f696a57a2c7a0104475412)

Hi, I'm Troy McClu...err, /u/schismsaints

You might remember me from my reddit hits such as "Why does AutoMod hate everything I do?", or [my most recent post from a couple of days ago](https://www.reddit.com/r/Superstonk/comments/of20ou/a_deep_dive_into_nftgamestopcom/).

I wanted to update my previous DD with some recent findings, clearing up a few points as well as expanding on the research I've done thus far. As before, you can find the current DD image in multiple formats here at my GitHub repo - <https://github.com/schismsaints/GME_NFT>

To start, if you aren't familiar with basic blockchain concepts, [my previous post](https://www.reddit.com/r/Superstonk/comments/of20ou/a_deep_dive_into_nftgamestopcom/) and [this one](https://www.reddit.com/r/Superstonk/comments/ofndb0/a_crypto_dive_with_the_jellyfish_10_things_about) from [/u/Dismal-Jellyfish](https://www.reddit.com/u/Dismal-Jellyfish/) (seriously, it's well worth a read) will help get you up to speed on the different token types, smart contracts, and other general blockchain concepts.

An Update on GME Tokens

-   [ERC-20 GameStop.finance scam token](https://etherscan.io/token/0x9eb6be354d88fd88795a04de899a57a77c545590) - Obvious scam is obvious, but finding this token gave me a link to be able to more conclusively debunk the 69,420,000 ERC-20 token

[![r/Superstonk - A Deep Dive into nft.gamestop.com - Part 2: Electric Boogaloo](https://preview.redd.it/tcf7cmqnr7a71.png?width=256&format=png&auto=webp&s=c4e2a7928d64cbbfc523ab59b7ade084dba3eef4)](https://preview.redd.it/tcf7cmqnr7a71.png?width=256&format=png&auto=webp&s=c4e2a7928d64cbbfc523ab59b7ade084dba3eef4)

[![r/Superstonk - A Deep Dive into nft.gamestop.com - Part 2: Electric Boogaloo](https://preview.redd.it/ami03a1ur7a71.png?width=249&format=png&auto=webp&s=72c594892dfb607b865f03f9ef8f28755837fe9d)](https://preview.redd.it/ami03a1ur7a71.png?width=249&format=png&auto=webp&s=72c594892dfb607b865f03f9ef8f28755837fe9d)

"The missing link"

-   [ERC-20 GME GameStop Token](https://etherscan.io/token/0x5b7d043ecb3a694069cc01e763159ea1bde0541d) - Thanks to several of the commenters on my last post(s), I went through a deeper dive into the ERC-20 GME ('fake 1337420' address) token and agree that it is likely a scam.

    -   The two most solid pieces of evidence identifying the scam are:

        -   [0xfoobar directly disputing its validity](https://twitter.com/0xfoobar/status/1409740353738096641?s=21)

        -   [More than one address holding the confirmed scam token as well as this one](https://etherscan.io/tokenholdings?a=0xfb5484a510c48c307fd0253ee4d0a0866950f9a3)

    -   [There is one address](https://etherscan.io/address/0x7f8c1877ed0da352f78be4fe4cda58bb804a30df) which has ties to some potentially relevant blockchain companies (Cudo primarily) that had me doubting early on whether it was a scam, but on further research I've found a lot of links to Nigeria, Dubai, etc which, while not red flags in and of themselves, certainly don't line up with GameStop corporate hiring their own domestic blockchain team.

[![r/Superstonk - A Deep Dive into nft.gamestop.com - Part 2: Electric Boogaloo](https://preview.redd.it/1wimkjrp48a71.png?width=738&format=png&auto=webp&s=313c9516cfef292f5a4570e971a292ddce3810f7)](https://preview.redd.it/1wimkjrp48a71.png?width=738&format=png&auto=webp&s=313c9516cfef292f5a4570e971a292ddce3810f7)

Largest single GME ERC-20 Token holder address

-   [ERC-20 GME Coin Token](https://etherscan.io/token/0xd4596454a0e145842d1319d6921399e8e1622ad7) - I have identified [an external account](https://etherscan.io/address/0x503828976d22510aad0201ac7ec88293211d23da) involved in funding the GME Coin address, but the trail went cold after that. I can't confirm or deny that it is legitimate at this point; in either event, whoever created it went through more effort to hide their tracks than the other tokens. It does not appear to have been sold/swapped anywhere as of yet.

-   [ERC-721 GME GameStop Token ("The One and Only")](https://etherscan.io/token/0x13374200c29C757FDCc72F15Da98fb94f286d71e) - I suspect this will be the only one of its kind minted, either as a teaser or POC token for further NFT work.

    -   One interesting possibility came to mind that - while not a crypto dividend per-se - could still have some interesting applications to securities exchanges or implications for the MOASS. Caution: Speculation/theorycrafting inbound

        -   Consider the scenario involved with shareholder voting, where each shareholder receives a control number on each brokerage where they hold shares. Each control number is associated with the number of shares held at a point in time snapshot.

        -   With ERC-721 or ERC-1155, a unique NFT could be minted for each shareholder/control number. The number of shares associated with each NFT could either be held in an external DB or as metadata (a field on the token itself).

        -   This would create a public record of the number of shares held by individual shareholders at a point in time and could be updated on an annual basis (or more frequently if desired) in line with shareholder voting standards.

        -   This also avoids the 'crypto dividend' hangups associated with Overstock as there isn't any money involved nor is there any way this method could prevent legitimate short selling - it's merely a public ledger of shares in circulation.

    -   Alternatively, if they do a crypto coin dividend instead of a crypto stock dividend like Overstock, presumably they wouldn't place the same restrictions on selling which was the main point of contention in the Overstock case as I understand it. See below for some reading on Overstock.

        -   <https://realmoney.thestreet.com/investing/stocks/overstock-is-paying-a-digital-dividend-and-it-gets-really-interesting-now-15037958>

        -   <https://www.irmagazine.com/technology-social-media/how-overstock-used-blockchain-distribute-its-digital-dividend>

[/u/No-Fox-1400](https://www.reddit.com/u/No-Fox-1400/) has a lot of the same thoughts I do in his posts here:

-   <https://www.reddit.com/r/Superstonk/comments/ofiev4/the_man_with_the_plan/>

    -   The timeline here including Overstock was an excellent read, but the part I really want to call out is this

[![r/Superstonk - A Deep Dive into nft.gamestop.com - Part 2: Electric Boogaloo](https://preview.redd.it/olsculkf38a71.png?width=678&format=png&auto=webp&s=dbdaefd50c398f333896a14a204bafaa79334fd2)](https://preview.redd.it/olsculkf38a71.png?width=678&format=png&auto=webp&s=dbdaefd50c398f333896a14a204bafaa79334fd2)

This is in line with my thoughts on timing - NFT platform launch on 7/14, announcement of dividend/crypto play on 7/14, and record date for a crypto based dividend on 7/24

-   And here: <https://www.reddit.com/r/Superstonk/comments/ocvqlp/the_rules_dont_matter/>

[![r/Superstonk - A Deep Dive into nft.gamestop.com - Part 2: Electric Boogaloo](https://preview.redd.it/89f8rnnw38a71.png?width=692&format=png&auto=webp&s=edc369dbfdb253baf183cdf837c9f725610a5a58)](https://preview.redd.it/89f8rnnw38a71.png?width=692&format=png&auto=webp&s=edc369dbfdb253baf183cdf837c9f725610a5a58)

Recent Activity

[/u/clawesome](https://www.reddit.com/u/clawesome/) and [/u/nuclear-falcon](https://www.reddit.com/u/nuclear-falcon/) noticed some recent activity on the original smart contract here

<https://www.reddit.com/r/Superstonk/comments/ogjbcy/one_of_the_addresses_associated_with_the_gamestop/>

I've drawn out these relations on the long format diagram, shown below

[![r/Superstonk - A Deep Dive into nft.gamestop.com - Part 2: Electric Boogaloo](https://preview.redd.it/507nrqd258a71.png?width=530&format=png&auto=webp&s=26992c61f9346de0a90cc46bea65c17011018810)](https://preview.redd.it/507nrqd258a71.png?width=530&format=png&auto=webp&s=26992c61f9346de0a90cc46bea65c17011018810)

Adding approving parties/other devs to the owner/approval list

Huge credit to [/u/HandyBananaMan](https://www.reddit.com/u/HandyBananaMan/) for being almost as obsessed with the transaction logs as me and pointing me toward several bread crumbs along the way.

TL:DR; Buy, Hold, Buckle Up. GME Blockchain team hard at work to bring us something mind blowing. I expect that *even if* a crypto dividend does not materialize, the [nft.gamestop.com](https://nft.gamestop.com/) project will be revolutionary and will function as a large catalyst for price movement regardless of a dividend play.

[![r/Superstonk - A Deep Dive into nft.gamestop.com - Part 2: Electric Boogaloo](https://preview.redd.it/i09xoc4e78a71.png?width=4808&format=png&auto=webp&s=03f646219e746517c83364692af14e96180906d6)](https://preview.redd.it/i09xoc4e78a71.png?width=4808&format=png&auto=webp&s=03f646219e746517c83364692af14e96180906d6)

This is the PNG format of the diagram here for convenience, but the current version is always on my GitHub repo.
