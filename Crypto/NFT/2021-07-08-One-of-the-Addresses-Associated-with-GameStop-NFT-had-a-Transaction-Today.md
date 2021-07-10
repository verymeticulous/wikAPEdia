One of the addresses associated with the GameStop NFT had a transaction today. Any wrinkle brains able to tell what it was used for?
====================================================================================================================================

| Author       | Source       | 
| :-------------: |:-------------:|
|  [u/clawesome](https://www.reddit.com/user/clawesome/) | [Reddit](https://www.reddit.com/r/Superstonk/comments/ogjbcy/one_of_the_addresses_associated_with_the_gamestop/) | 

---

[etherscan.io/addres...](https://etherscan.io/address/0x10B16eEDe03cF73CbF44e4BFFFa3e6BFf36F1Fad)

[Question ❓](https://www.reddit.com/r/Superstonk/search?q=flair_name%3A%22Question%20%E2%9D%93%22&restrict_sr=1)

---

## Relevant Comment/Answer by [u/nuclear-falcon](https://www.reddit.com/user/nuclear-falcon/)

---

**Official Gamestop NFT Contract "GME NFT":**

0x13374200c29C757FDCc72F15Da98fb94f286d71e

**Was created by "Creator":**

0x10b16eede03cf73cbf44e4bfffa3e6bff36f1fad

"Creator" is the account in question that OP linked.

*Creator is a contract itself!* If you go to the contract's [etherscan page](https://etherscan.io/address/0x10b16eede03cf73cbf44e4bfffa3e6bff36f1fad#readProxyContract) -> Contract -> "Read Contract as Proxy" you can get a little bit of information. The NAME field is "Gnosis Safe" which is a service in the form of a contract to force multiple people in a company to sign off on transactions before they happen, which is how you keep crypto at a company safe. [Here](https://help.gnosis-safe.io/en/articles/3876456-what-is-gnosis-safe) is a brief overview from their website.

If you go to the Creator address, you'll see a transaction from ~8 hours ago and then one that happened ~5 minutes ago (all from the time of writing). The "Events" tab on etherscan allows you to see which functions were executed.

Transaction from ~8 hours ago was to add "Add Owner" function execution. I think this means they added another person who can sign off on transactions.

Transaction from ~5 minutes ago executed 2 functions:

Remove Owner - to Remove a person/wallet from signing off on transactions

Add Owner - same as the one from ~8 hours ago that adds someone

**What I think this means:**

The NFTeam is adding new people who have rights to sign off on transactions with the official GameStop company crypto. This is a security measure that means no single person at the company can control/steal/send crypto to anyone else
