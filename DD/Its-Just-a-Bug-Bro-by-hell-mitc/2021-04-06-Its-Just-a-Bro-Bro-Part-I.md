It's Just a Bug Bro
===================

| Author       | Source       | 
| :-------------: |:-------------:|
|  [u/hell-mitc](https://www.reddit.com/user/hell-mitc/) | [Reddit](reddit.com/r/Superstonk/comments/mlqedv/its_just_a_bug_bro/) | 

---


[Serious DD 👨‍🔬🔬](https://www.reddit.com/r/Superstonk/search?q=flair_name%3A%22Serious%20DD%20%F0%9F%91%A8%E2%80%8D%F0%9F%94%AC%F0%9F%94%AC%22&restrict_sr=1)

Ok everyone here's the DD on how the market data actually gets to our ape boxes and hopefully will help trigger some more research on this shit because I am almost tapped. Me, I solve problems for a living. Basically people who don't think it's worth their time come to me as an IT/Technical professional and pay me to figure it out. Im pretty good at it actually, so if this literally goes tits up, oh well. Im not sure how much more time I can invest before my wife actually ends up with a boyfriend (hopefully after this goes moon because it'll be easier to get over crying into my wads of cash).

[![r/Superstonk - It's Just a Bug Bro](https://preview.redd.it/f6k9p55hfnr61.jpg?width=1085&format=pjpg&auto=webp&s=2799b87aa6f16150642f6449728c9e5787240f5a)](https://preview.redd.it/f6k9p55hfnr61.jpg?width=1085&format=pjpg&auto=webp&s=2799b87aa6f16150642f6449728c9e5787240f5a)

To start, I think it's imperative we really understand how the market data and ticker prices came to be. Initially, prices of shares of companies were updated by messengers, mail, etc., updated in a ledger by hand and made available to the public (New York). We're talking 1700's style don't shoot the messenger type shit. Then a bro came along and was like hey we can do this easier because everyone should have access to the information up to the minute, because... well, you know, free market or laziness, or because by the time some dude rode in on a horse or fucking train (were there trains in 1700s? Fuck it I'm too lazy to google) that info was already old news. 1867 out comes the telegraph ticker. This would have someone type on a keyboard the info (amount sold, last price, open/close, etc.) into the transmitter. In the 1900's, we get to personal tickers, computerized market and data, etc. It starts getting a bit muddy here because like anything, a market needs competition to live. So there were more than 1 different ticker style, and we can see with discrepancies that have been popping up that this is probably far more true than ever.

So, back to our anomalies we keep seeing. Back in Feb/March, I made a pretty quick post in GME about the After Hours spikes we were seeing. A few of the "ohhh it's just a bug" bros popped up and like anyone, I got a little discouraged and thought it might be a bug. But then it was "nahhh some idiot just fat fingered the keyboard." I mean I seriously doubt any of this is some experienced trader on an AH platform fat fingering to $400. Outrageous. I hypothesized that this was legit a spread with some smaller shorts covering and a few big players forcing the prices to be whatever they wanted (I mean seriously, I actually couldn't even tell you how to trade in AH). Now, I believe since then, we have seen $1300 spike, sell and buy data at crazy amount, and now we are seeing volumes WAY beyond what is any reasonable (1T, 600M, just ridiculous numbers that anyone would be like "ya fuck it it's a bug"). Shortly after this, I got banned from GME for... Well I don't actually know why, they cited "Violence". But whatever back to the data.

Now, yesterday I noticed that the NYSE and Yahoo/Nasdaq closed AH at some different prices. What's weird to me is that Yahoo pulls data at the minute (with a 15 min delay notice) pretty accurately I think. Nasdaq actually seems to be almost on par with Yahoo, but with a 15 min delay and updates the trade volume better. The NYSE seems to be ONLY at a 15 minute delay, and has the worst way to follow what is going on (which is weird for a company that touts being the most advanced data whore -- but more on that later and if you're good at something, never do it for free, right?).

So here's how far I am and if anyone wants to put on a tinfoil hat and hop down the rabbit hole, please do.

Why (and how) would Yahoo, Nasdaq and the NYSE all have a different price showing when you would think that they would at least pull the data from a similar, consolidated spot?

[![r/Superstonk - It's Just a Bug Bro](https://preview.redd.it/tjkwovlpdnr61.png?width=348&format=png&auto=webp&s=9b9d3a705d02072621851258c143e39a89f2a449)](https://preview.redd.it/tjkwovlpdnr61.png?width=348&format=png&auto=webp&s=9b9d3a705d02072621851258c143e39a89f2a449)

Yahoo

[![r/Superstonk - It's Just a Bug Bro](https://preview.redd.it/ovz17q9sdnr61.png?width=527&format=png&auto=webp&s=60716acabdfabbbeb269ce95ff665720a73c8807)](https://preview.redd.it/ovz17q9sdnr61.png?width=527&format=png&auto=webp&s=60716acabdfabbbeb269ce95ff665720a73c8807)

NYSE

[![r/Superstonk - It's Just a Bug Bro](https://preview.redd.it/iifu46dvdnr61.png?width=479&format=png&auto=webp&s=889caef4eb1352375086e5886692b9f788ffd88e)](https://preview.redd.it/iifu46dvdnr61.png?width=479&format=png&auto=webp&s=889caef4eb1352375086e5886692b9f788ffd88e)

Nasdaq

Sorry for the NYSE one, it stayed the same at and past 19:59:57 and was even different on their graph, but like I said in my post - I felt a little like I was actually just going crazy and didn't post this immediately.

I will say, I am not a software engineer but I know how to inspect code and where it comes from. And as to what it is doing, well, lurk moar.

Yahoo Finance

Uses what seems to be raw binary data through something called SharedArrayBuffer. It seems to pull data from all over the map and consolidate it on their site. Direct quote from Github on how this works is:

"A SharedArrayBuffer is like an ArrayBuffer, apart from its memory being shared, and the memory is accessed in the same way as an ArrayBuffer's memory is: by creating views on the buffer, and then accessing the memory via the view using standard array access syntax. The same view types can be applied to SharedArrayBuffer as to ArrayBuffer, from Int8Array to Float64Array."

Now, Yahoo, when I sell or buy shares, personally seems to be the most accurate on the platform that I use. Maybe because when I sell my shares, they are pulling it from the same place the clearing houses are. We need to remember that Yahoo had the opportunity to buy google (only the most powerful data company in the world now) originally. We can only assume that it was because Yahoo is a data powerhouse... And they are still around so obviously they were aligned but didn't go through with it.

My hypothesis in this is that this is the raw binary data pooled by NSCC and the DTCC that is pulled and presented.

Nasdaq

I am having a hell of a time figuring out where the Nasdaq pulls its info from. As far as I can tell, it is open source? This could be completely wrong and I am not willing to throw a guys name out who is promoting OSS and is designing nodes. If I know anything about business (and I should hope I do), it would seem plausible that a main entity has raw binary data and leases the access to it to whoever wants to pay. No offence kid, it's just business.

Now lets get to the main entity that is delayed, has our stock listed, and is owned by its own data company. Haha, yes. Really.

NYSE

The NYSE seems to gather its data from someone called Intercontinental Exchange (ICE). Now, funny thing is, ICE is completely automated (as per their own website) and OWNS THE NYSE. No conflict of interest there, right? RIGHT!?

I was going to post this last night so I am not sure who wants to look at the data still, but it is posted as of AH on April 5, 2021.

The NYSEs graph for GME shows a little closer, at $188.57. Odd that it isn't tied directly to the Close price up top (Last Trade Time: 04/05/2021 19:59:57 Price=$186.95).

Now, when I dig into ICE a bit more, there isn't a ton of info. A lot is veiled in secrecy around how this company operates for 6 clearing houses and 11 exchanges (internationally). Constantly completing M&As and becoming the go-to for data.

Maybe they are attempting to change the way the data is processed to create a more transparent market, but I can't help but feel this nagging issue with 1 company controlling all the data surrounding the market information we all use to diagnose issues. And it would be in their best interest to make people think that Yahoo and everyone else is "just a bug bro". With saying that, if they are operating as the up to the date info for international exchanges, they would have to meet all compliance requirements laid out in any trade agreements. This creates another nightmare, but we can just keep that in a little box for now and hope it isn't anything.

On to the reason I cant see this being a glitch or bug: Risk and Compliance. Ive read some DD over the span of being banned on GME that would make a lot of sense. If you know anything about risk and compliance people (lawyers, underwriters, adjudicators, any of them), they don't like to fuck around. We are talking Tesla self driving fuck around where we need to figure out if the computer should run over the baby carriage or the old lady. What do you think they think when the team of these people sit around and try to figure out how their liability is going to be extended? Who is going to sue who and how do we get out of this for the cheapest way possible? Liability is everything in these worlds, and when we are talking about physical (digital really) money being passed around at billions (trillions?) per day, you better fucking believe the risk and compliance guys wont fuck around with "bugs" and "glitches".

In my opinion, if we are seeing these numbers and people popping up saying "nah fuck it its just a bug or a glitch", we are on to something. There are no "glitches" in the finance world. This isn't fucking cyberpunk2077. They don't release a new patch to solve "where'd my money go" glitch. If you can imagine legacy on legacy programing, they have tested this shit inside and out before it even came to be. They worked out every possible bug. If we are seeing massive numbers on Yahoo, I am under the assumption that they are actually pooling the data they need to in order to get a real number (someone is anyway), and that number is being presented behind closed doors, to whoever is monitoring this at this point (ummm... uhhh... what?).

Now I am not a software engineer, but infer from this what you want. We keep seeing random shit pop up, and I haven't noticed this with any other superstonk. If anyone can provide an example of another stock, I will update this. But until then, go go gadget tinfoil hat. See you on the moon, or the asylum I am not sure at this point.

Not financial or software or programming advice. Just research and hypothetical situations.

[![r/Superstonk - It's Just a Bug Bro](https://preview.redd.it/7jdagqqjfnr61.jpg?width=640&format=pjpg&auto=webp&s=793ead25d80554da47bcefcdd189e480598150f5)](https://preview.redd.it/7jdagqqjfnr61.jpg?width=640&format=pjpg&auto=webp&s=793ead25d80554da47bcefcdd189e480598150f5)

PS I stole these memes so if theyre yours - Thanks for the laugh.

Edit: For me this means someone is looking at the real numbers and there's no way to pull them without sourcing them collectively in binary data. If you ask the citadel et al. legal teams for this info, you think they'll hand it over? There's a reason why these private corps are continuing this, and there's a reason why someone is trying to access the collective data. They are trying to see just how deep the rabbit hole goes. The only way to do that in a live setting from a private entity is to source it how its supposed to be submitted. The same way it's being hidden, it's being viewed. That's my only opinion on it.
