---
title: Mozilla's failures and a path to profitability
linkTitle: Mozilla's failures and a path to profitability
author: Andrew Gioia
slug: mozilla
date: 2020-08-14
publishdate: 2020-08-14
banner: https://media.gioia.cloud/blog/posts/mozilla/post-cover.png
images:
    - https://media.gioia.cloud/blog/posts/mozilla/post-cover.png
description: I love Mozilla, I love its mission, and I love its core product, Firefox. It absolutely sucks as a business though, and its current trajectory is insolvency. Mozilla needs to focus on Firefox and core technologies, sell privacy-first software as a service, and bring back technical leadership if it truly wants to execute on its mission.
tags: 
    - Mozilla
    - Firefox
    - Internet
    - Nonprofits
    - Business
---

<p class="big">I love Mozilla, I love its mission, and I love its core product, Firefox. It absolutely sucks as a business though.</p>

I suspected this for many years, re-realizing it every time [Hacker News](https://news.ycombinator.com/item?id=24120336) or some other story reminded me of its umbilica cord to Google. Relying on one contract to provide over 80% of its revenue[^1] every year is bad enough. Forcing itself onto a tightrope walk&mdash;privacy as a business model on one side, reliance on your _chief competitor_ (an _ad company_ no less!) to make payroll on the other&mdash;is critically negligent. 

<!--more-->

Despite Firefox Quantum's significant improvements over the past three years, I've felt for a while that Mozilla has been on a self-inflicted downward spiral and that the number of its eggs in one basket was symptomatic of some yet-unidentified-to-me structural issues. Its [recent blog post by CEO Mitchell Baker](https://blog.mozilla.org/blog/2020/08/11/changing-world-changing-mozilla/) and corresponding [internal memo laying off _25% of its worforce_](https://blog.mozilla.org/wp-content/uploads/2020/08/Message-to-Employees-Change-in-Difficult-Times.pdf) were so resoundingly misguided, though, that **I feared for the first time the organization is all but dead**.

It's unclear to me how a message designed to rally the troops and its userbase in a time of crisis could create so much confusion. It appears to be perfectly emblematic, however, of Mozilla's poor leadership over the last decade, repeated failures at _the business side_ of software development, loss of identity, and inability to innovate while staying [true to its mission](https://www.mozilla.org/en-US/mission/). 

I use Firefox all day and recommend it. I pay for their limited VPN offering to encourage its development. **I want Mozilla to succeed so badly and deliver on its mission, which is why it's so painful to feel this way about them.** These are also very hard things to do and as the champion of the "free and open Internet" Mozilla is admittedly held to a very high standard. Its repeated own goals are frustrating and inexcusable, though, and a company of its size and with its brand and trust could succeed with a better direction.

## Mozilla is bad at business {#business}

<p class="big">After over 2 decades as one of the founding Internet companies, Mozilla has shipped essentially one profitable product: Firefox.</p>

In that time it also [lost about 80% of Firefox's browser market share](https://en.wikipedia.org/wiki/Usage_share_of_web_browsers)[^2] and abandoned its only two other potentially profitable ones, Thunderbird[^3] and Firefox OS.

While it is certainly not required for nonprofits and purpose-driven organizations to sell, they do need to focus on their bottom line if they hope to continue existing. At [$14MM in 2018](https://assets.mozilla.net/annualreport/2018/mozilla-fdn-2018-short-form-final-0926.pdf), Mozilla's donations barely scratchd the surface of its $444MM expenses that year. 

Without a fundraising machine, it's foolish to think Mozilla can continue to develop interesting open source software without any attempts at monetizing it or other endeavors. **It's also misguided to think that monetizing software means Mozilla has given up on its mission.** Selling software and services is its only path forward and is indeed what it wants to be doing as a mature open source software organization today.

Unfortunately, instead of realizing this and leveraging its early advantage and market share in a software space _where the product is used every day all day by every human being_, Mozilla hired consistently bad leaders who set a bad direction, got lazy, and focused on the wrong things.

### Mozilla sat on Firefox's lead, allowing it to get slow and bloated {#slow}

I was _excited_ to switch away from Firefox in 2009 when Google Chrome became a bit more established. At that point Firefox was much, much better than Internet Explorer 7 and I took advantage of its deep extension ecosystem, but browsing still was slow, the app was very resource intensive, and like all browsers, one tab crashing nuked the whole window. Chrome came out of nowhere and completely reset the expectation on browser speed and footprint. Indeed, it reset the idea of what a good browser even is.

* **It was very light and fresh**, and its minimalistic interface helped make it _feel_ faster. Tabs moving to the title bar and the removal of anything extra helped the browser get out of the way as much as possible so that I could do what I wanted to do online.

* **The omnibox made search faster.** Combining the dedicated search box and URL bar created huge and unexpected performance gains for me. There was one place to do things&mdash;the universal address bar&mdash;and I didn't need to make a decision between URL and search. Firefox did help autocomplete URLs from browsing history, but it still had a dedicated search input. The omnibox removed a big step.

* **Each tab had its own process.** Not only did this prevent the entire browser from crashing when one tab had a problem, it helped speed up browsing even more as there wasn't one big process for everything. 

* **Incognito Mode was very useful.** Safari had apparently had this for years but I wasn't on a Mac then and Safari wasn't popular for a lot of other reasons on Windows. While very basic, Incognito windows were my first foray into Internet privacy and became an easy way to load a fresh copy of a website. 

{{< picture 
    source="https://media.gioia.cloud/blog/posts/mozilla/firefox-chrome-2009@light.png"
    dark="https://media.gioia.cloud/blog/posts/mozilla/firefox-chrome-2009@dark.png" 
    alt="Firefox and Chrome in 2009" 
    title="Firefox 3 and Google Chrome 0.2.149 on Windows XP in late 2008."
    caption="Firefox 3 and Google Chrome 0.2.149 on Windows XP in late 2008." >}}

Firefox was without question the best browser through the early 2000s and it pushed the web forward in countless ways, often in stark contrast to Microsoft. [Firefox 3 earlier in the year was incredible](https://www.cnet.com/reviews/firefox-3-review/) and set single day download records, but the browser experience was slow and updates felt incremental and not "revolutionary." 

After Chrome launched, Mozilla started playing catchup and soon began releasing updates to match or mirror its new rival, like moving its tabs up to the title bar and releasing "Private Browsing." [A review of Firefox 3.5](https://www.technologizer.com/2009/06/30/firefox-3-5-review/2/) captures the beginning of a sentiment that would swell over the next years, emphasis mine:

> **Today’s most interesting browser isn’t Firefox&mdash;it’s Chrome**, with its spare user interface and total focus on making Web apps run seamlessly. The most feature-rich browser continues to be Opera&mdash;and with the new Unite server technology, Opera is being daring in a way that Mozilla isn’t.

While Firefox 3.5 was still often recommended as "the most well-rounded browser overall," users begain saying things like "3.5’s enhancements _get Firefox back in the game_ in several areas where other browsers had jumped ahead." Speed became the number one factor and Firefox lagged, and as Chrome launched its own extensions the delta began retracting. 

As Mozilla fell behind on speed and footprint, its inability to match Google's heavy advertising of Chrome sealed its fate. This is perhaps unfair as Google was able to plaster "Download Chrome!" ads on its trillions of pageviews daily, but if Mozilla had stayed hungry and leveraged its position, it could have anticipated the latent demand for a more minimal, faster, and lighter browser. It didn't and began conceding marketshare with every Chrome release, importantly to many of the IT and tech enthusiasts who recommend and install browsers.

While I've been back and loving Firefox since Quantum came out in 2017 and will not install Google Chrome on any machine my family touches, a lot of damage was done in this time period.

### Somewhere Mozilla lost its focus and has failed to innovate where it matters {#focus}

**It cannot be overstated how positive a force Mozilla has been** for open source software and Internet freedom. Their contributions over the past two decades are too numerous to list in full, but to highlight a few: recent technologies like [Rust](https://www.rust-lang.org/), [Web Assembly](https://webassembly.org/), and [Servo](https://servo.org/) are really innovative and promising web foundations; its contributions to JavaScript, WebGL, and open codecs like AV1 have been critical; even the MDN web docs are an absolutely wonderful resource.

Over the past decade, though, a lot of its innovation on core products and services was uninspired at best while some, like Thunderbird, were left to rot. The only _relevant_ innovations I can even think of off the top of my head have been Firefox OS, its promising but failed mobile operating system, and multi-account containers, an actual gamechanger in browsing but really the only homerun there. 

Mozilla bet heavily on Firefox OS and under proper management it could have been _the_ community-driven, open source mobile OS with open standards and APIs and a competing app store. The dream. It _still_ could be a phone I'd be happy to switch to, just as I was eager to at the time, had a proper handset shipped. [It lasted less than 4 years](https://www.cnet.com/news/why-the-death-of-the-firefox-phone-matters/), due in no small part to [their new CEO misunderstanding it](https://medium.com/@bfrancis/the-story-of-firefox-os-cb5bf796e8fb), among other issues.

There have been a lot of distractions during this time as well that have peeled resources away from their foundational product: strange partnerships that send data to third parties (even Google Analytics), social advocacy on issues that have nothing to do with the Internet, and bets on trendy technologies that have gone nowhere.

Why has Mozilla been investing so heavily into virtual reality? Hubs, a service to launch private virtual rooms together, and Firefox Reality, a VR browser, have gone nowhere and do nothing to "ensure the Internet is a global public resource, open and accessible to all." Mozilla's acquisition of Pocket was also strange&mdash;its forced Firefox integration as a default super-extension angered much of its core userbase for most likely very, very little in return. It also competes directly with Firefox's native bookmarks/library, a feature that's been core to the browser experience since inception and could be held back by this competing service.

While these trendier areas siphoned resources, Mozilla began playing catchup on its one core product. One look at [some of the longest](https://bugzilla.mozilla.org/show_bug.cgi?id=288704) [and more fundamental outstanding bugs](https://bugzilla.mozilla.org/show_bug.cgi?id=69687) is just a very small revelation into some larger issues as to where the company invests resources and what it focuses on. Chrome may not have even existed had Mozilla been more aware of what its chief product and userbase needed, or welcomed initial attempts by Google to help propel Firefox further, faster.

### The company has a phobia for monetization {#phobia}

Selling valuable software and services does not at all necessitate Mozilla compromising on its mission or values. It's a perfectly respectable (and welcome!) path for any nonprofit or FOSS organization and there's been a growing trend with for-profit open source organizations selling support or other addons, normalizing this even more. 

For some reason Mozilla has only recently dipped its toes into a booming SaaS world. These are the only products I can currently give Mozilla money for:

* **Mozilla VPN**, a whitelabeled Mullvad for $5/month. I've been paying for this for 5 months since I got off the waitlist and there is still no Mac and Linux support. (Up until this month this was called Firefox VPN).

* **Pocket**, a bookmarking service for $5/month. With premium I get permanent archiving of anything I save (excluding embedded media and PDFs) and full-text search. This actually isn't bad for the price, but it seems to be primarily for reading and not notetaking or bookmarking how I use them. There's a lot of opportunity here for a service that doesn't appear to have had any updates in years.

That's it. I could donate to the Mozilla Foundation and pray it goes towards product development or to hire back the [Servo](https://twitter.com/directhex/status/1293352458308198401) and [MDN teams](https://twitter.com/MozDevNet/status/1293647529268006912) that just got eliminated. Most likely it will fund one of the social causes I don't think they should be spending time and energy on, so I don't donate.

* **Lockwise** could be a true competitor to Bitwarden, which I love, or one of the other premium password management apps like 1Password or LastPass. There's a clear market for this, [1Password raised $200MM last year](https://techcrunch.com/2019/11/14/fourteen-years-after-launching-1password-takes-first-funding-a-200m-series-a/) on it and we pay Bitwarden hundreds per year right now for our team of 15. 

* **Monitor** is just a thin wrapper over Have I Been Pwned; where is the development there or more enhanced monitoring they could try to innovate on and roll out?

* **Send** is currently down and has been down for quite some time. It's a great idea and one I've also been _trying_ to spend money on the business side, it's just not available.

### Mozilla's leadership has been the root of its problems and is still actively harming it {#leadership}

Perhaps the true root cause of Mozilla's business failures has been it's management and the culture that developed it, particularly since Brendan Eich was fired.

I won't pretend to be an expert on the internal politics at Mozilla or a lot of the explanations as to their poor leadership changes and decisions, but two public examples offered all of the support needed for Mozilla's cultural and operational problems.

#### Mozilla has a massive cultural problem if its CEO thinks it's okay to defame a deceased coworker. {#baker}

My first real inclination that Mozilla has problems was when its CEO, Mitchell Baker, wrote a [blog post in memory of Mozilla's first intern, Gervase Markham](https://blog.lizardwrangler.com/2018/08/07/in-memoriam-gervase-markham/). Baker wrote things that are strange to even think about a recently deceased coworker, let alone say quietly to close friends, let alone _publish online for everyone to read_.

For a CEO to defame someone in the organization who lost his battle with cancer&mdash;particularly one as consequential as their very first intern!&mdash;speaks volumes about the company culture and workplace toxicity that would create an environment where this is normal. 

> Eventually Gerv felt called to live his faith by publicly judging others in politely stated but damning terms. His contributions to expanding the Mozilla community would eventually become shadowed by behaviors that made it more difficult for people to participate....
>
> Gerv's default approach was to see things in binary terms — yes or no, black or white, on or off, one or zero. Over the years I worked with him to moderate this trait so that he could better appreciate nuance and the many “gray” areas on complex topics....
>
> Gerv's faith did not have ambiguity at least none that I ever saw. Gerv was crisp. He had very precise views about marriage, sex, gender and related topics. He was adamant that his interpretation was correct, and that his interpretation should be encoded into law. These views made their way into the Mozilla environment. They have been traumatic and damaging, both to individuals and to Mozilla overall....

Why feel the need to highlight "the damage and trauma he caused"? Why must we remember "all of Gerv — the full person, good and bad" in his public obituary? Why feel compelled to highlight how _you_ were the only person moderating his judgmental mindset?

It's completely unprofessional and while at least politely written, was [exceedingly mean-spirited and perhaps greatly upsetting to his surviving family and friends](https://lwn.net/Articles/762345/). This is their leader.

#### The way Mozilla handled Brendan Eich's forced resignation was shockingly immature and harmful. {#eich}

Brendan Eich was one of the [co-founders of the original Mozilla](https://en.wikipedia.org/wiki/Brendan_Eich) and then the foundation, going on to serve as the corporation side's CTO and later CEO in 2014. Eich invented JavaScript and was critical to the creation and early success of Firefox. In 2008 he donated about $3,000 to a California effort seeking to ban same-sex marriage in the state. This was the same year [Barack Obama said "marriage is between a man and a woman"](https://en.wikipedia.org/wiki/Social_policy_of_the_Barack_Obama_administration#Same-sex_marriage).

[Mozilla was assuredly aware of this](https://news.ycombinator.com/item?id=3793012) yet did not have the foresight or experience to anticipate it. [He resigned 11 days later](https://blog.mozilla.org/blog/2014/04/03/brendan-eich-steps-down-as-mozilla-ceo/), choosing to leave instead of finding a new role, later founding a competeing browser, [Brave](https://brave.com).

Eich felt he could not "be an effective leader" of Mozilla given a personal belief unrelated to Mozilla's mission, products, or business. Mozilla not only allowed, but presumably compelled to leave one of the smartest minds and biggest contributors to open source software and Internet freedom. Mozilla could not balance personal and professional spheres, and it did not have the organizational integrity to support such a leader despite his views that some people find very objectionable.

Mozilla won nothing and institutionalized a social litmus test, no doubt turning away many potential highly qualified leaders and developers.

[The comment on Hacker News by will4274](https://news.ycombinator.com/item?id=24123409) that prompted me to think and write about Mozilla captures many other aspects of Mozilla's leadership problems much better than I could know or articulate (emphasis mine):

> Mozilla, like Debian, has many technical users with loud opinions and struggles to reach consensus.... But, Mozilla has the worst result&mdash;"logjam breaker" executives come in, and, rather than pushing the technical leadership to make a reasonable technical decision based on the weighed factors, they break the logjam by encouraging the technical leaders to blindly imitate the competition. This problem is intractable&mdash;giving in to the Debianers means being mired in debate forever and making no or extremely slow progress; giving in to the suits means failing to innovate, becoming a clone of your competition, and eventually being forgotten. **A true solution requires real technical leadership, something that's sorely lacking at Mozilla,** or a different user base, which is not a possibility at Mozilla.
>
> Second, ... [n]on-technical leadership comes to dominate decisions about how to [spend] incoming donations from successful technical projects. Such leadership is often interested in [hopping] from the board of one non-profit to another.... The results [are] a slew of failed and cancelled projects while the core project languishes.
>
> Finally, ... [m]ost companies right now are on a social justice kick and for the last few years. That's good; racism is bad, and tech could be a bit more welcoming. However, most companies understand where the lines are drawn. For example, Google executives don't release statements after employees die trashing the employee because of an underlying difference in personality and/or political views. Google also doesn't fire executives because of their political views or previous donations, when held privately, particularly when those political views are relatively common. **Such actions have a chilling effect on recruitment** and leads to technical talent [who] might otherwise have been interested in Mozilla (like myself) to permanently write it off.

Mozilla has chosen social advocacy over technical leadership and has reduced itself to maintaining Firefox rather than navigate an innovative path forward.

## A (proven) path forward: Mozilla as a privacy-focused SaaS company that sells well-designed software in exchange for dollars {#solution}

<p class="big">There's a shockingly simple solution to all of the non-leadership problems Mozilla has: make Firefox the best browser in the world and sell privacy-first, open source software-as-a-service that respects our integrity.</p>

### Mozilla should first focus on its core product: Firefox {#firefox}

The primary all-hands-on-deck imperative should be to decouple Firefox from Mother Google. Mozilla's chief competitor and an ad company toxic to the web&mdash;one that needs user data to build tracking profiles for Mozilla's users&mdash;is diametrically opposed to its mission and ethos. And for some reason _that's_ totally fine but Eich's past isn't?

Google is the only one paying Mozilla's bills right now and that lifeline cannot be understated, but everything the company does needs to move it away from Google or any search sponsor by 2025. This is primarily for business reasons and diversification, but just as important it fixes Mozilla's hypocrisy and gets it some trust back.

Related to this, Mozilla just needs to pump more resources into Firefox itself. Make it so fast and light that it's a "no brainer" for even the layman to switch to over Chrome. Release polished, vetted, useful extensions and pay the best community developers donating their time. Even better: build [uBlock Origin](https://ublockorigin.com/)-style ad blocking as a native feature. Apple realized this advantage years ago and as Chrome's parent forces it to whittle away at tracking prevention and privacy features, Firefox can gain an even bigger competitive advantage. 

In 2 years Firefox should again become the obvious browser on speed, performance, memory management, privacy, and customization/user control. Mozilla should double down on the tech enthusiasts and family IT support specialists who formed its base; they're the ones who often recommend and install browsers for many others. Building up the userbase again via a free powerful Firefox creates a bigger captive audience for services.

### Mozilla should then release rock-solid privacy-first data services that people already want to pay for {#saas}

Mozilla's primary source of revenue in 5 years should be from services. Apple saw this years ago and built up their services segment to about $14B per quarter now, over 20% of its total revenue. It did this due to, in no small part, its focus on privacy. Mozilla is perfectly positioned to do this even better, selling data services that people are already paying for, at scale, and with a massive privacy focus. 

Mozilla should release services in all of these areas:

* **Password management:** beef up Lockwise into a full-fledged service, dedicated apps, and Firefox integration. **$5/month.**

* **Email:** it boggles my mind that Mozilla has not done this yet, considering they had the best original email client. Sell a privacy-focused email delivery service like Mailfence or Fastmail. Bonus points if it supports IMAP flags fully and correctly 😜. **$10/month or more, depending on accounts.**

* **VPN:** create an actual VPN service with apps cross-platform! I'm already paying for this and would pay more for region switching or even related DNS features. **$5/month.**

* **Document sync and sharing:** I will no longer install Dropbox on any machine and have been begging for a service like this. Integrate it with Firefox Send! Integrate it with Thunderbird and your new email service! Sell upgraded filesize or persistence tiers for Send. **$5-10/month.**

* **S3-compatible storage:** I pay Backblaze right now for large S3 storage to backup my documents and home media from my Synology NAS. Backblaze is great but I would pay Mozilla for this to support them and their mission. **$10-20/month.**

* **Video hosting:** this is going to cost a ton of money to do correctly but I would love a Vimeo-style video hosting service by Mozilla. I like Vimeo but I want to support Mozilla more, and if this integrated with S3 buckets to share media, even better. **$10/month.**

All of these need to be built privacy-first, backed by Mozilla's brand and mission statement. My family would move about $50/month we're already spending and probably more for document sync as I'm not using anything for that right now.

After this, Mozilla should leverage its new experience in delivering services and the other tools that it's built and develop a full-fledged business service offering to pull people away from GSuite. I hate using GSuite every day but it's right for our use case and it does its job well. I would move to Mozilla's suite in a heartbeat and feel great about that lengthy transition! Collaboration software built on Rust/WebAssembly as a principal use case would be incredible.

### Mozilla's north star should be "the Internet's much-needed infrastructure" to fully execute on its mission {#northstar}

Gmail should not synonymous with email, YouTube should not be "where videos are stored," and [Twitter and Facebook should definitely not be where public discourse takes place](/posts/facebook). All of these services are "core infrastructural" web services that should not be controlled or dominated by private for-profit ad companies with zero competition. It's a complete misalignment of importance and trust and Mozilla should take this on just as Wikipedia has with knowledge.

Mozilla's "final form" should ultimately be the primary builder and steward of our decentralized and federated Internet infrastructure&mdash;the counter to the private ones that are currently de facto. I can think of no higher accomplishment that would completely "ensure the Internet is a global public resource, open and accessible to all."

<p class="swqm"><em>"Oh yeah, just make a social network</em> 🙄<em>"</em> or <em>"lose $10B per year on hosting 5 trillion cat videos"</em> is not the idea. The idea is to make a more purposeful, federated content host to provide a viable alternative to the private ad-supported monopolies. Supporting the mission and/or paying for power features or additional storage can offset this, as could building in a creator-first revenue sharing arrangement.</p>

This should sound crazy because it _is_ crazy&mdash;this is the long term goal and would be an unbelievable coup. Having an actual, tangible north star like this can also serve to rally and direct the team and its users. Currently Mozilla has no real definition of success or anything tangible to point to.

## A moderate warning: Mozilla _is_ losing necessary trust with the libre world, its core demographic {#trust}

<p class="big">
Mitchell Baker's unfocused blog post on Mozilla's focus ended by saying they're "fortunate that Firefox and Mozilla retain a high degree of trust in the world." This is true to a certain extent and I very much would trust Mozilla to deliver privacy-focused services and software, but there's a limit to it and Mozilla is actually approaching that.
</p>

Mozilla only has so many chances before its core base gives up and the whole organization unravels. On its current trajectory&mdash;firing important teams like Servo and MDN and promoting the aimless VR stuff&mdash;this trust will begin waning and someone else will take up the cause.

### Baker's blog post unfortunately left me feeling that they _still don't get this_, and their "focuses" are worrying.

**Talking about the new focus on product**, Baker says that to start, this means "products that mitigate harms or address the kinds of the problems that people face today. Over the longer run, our goal is to build new experiences that people love and want, that have better values and better characteristics inside those products." I have no idea what this actually means but I suspect it's everything except for Firefox and useful web services. Why is this the initial focus?!

**When talking about the "new mindset,"** she starts by describing everything great about the Internet ("the decentralization, ... open source underpinnings, and the standards") and then immediately goes into a "but." Why must Mozilla shift anything to enable these? Why is she saying Mozilla won't be "trying to keep a piece of what we love" anymore, is it no longer defending decentralization? Why is she again talking about "advocacy"?

**When talking about community** and their volunteer developers, why does Baker link to a video on "transforming prison communities" as an example of what they need to be doing? This is great but how about their _developer community_ first?

The **focus on economics** is about the only thing I agree with in this manifesto. "Recognizing that the old model where everything was free has consequences, means we must explore a range of different business opportunities and alternate value exchanges." This is correct and they do need to experiment with their business model. I'm very curious to see how they begin to put this into practice.

#### Mozilla needs a visionary leader with a strong technical background and Baker isn't it.

Her blog post, the layoffs, and the internal memo did more to worry me about Mozilla's future than any other decision or event in Mozilla's long history. Mozilla still does have our trust now, but it's on a path to losing it and its current CEO will almost assuredly take it there if left unchecked and without better technical and business leadership.

[^1]: This is tough to estimate and [official numbers stop at 2011](https://en.wikipedia.org/wiki/Mozilla_Corporation#Google) where it was 85% of all revenue. We do know that Yahoo paid Mozilla $375MM annually from 2015 to 2017 to become the default search engine in Firefox, and that Mozilla exercised its right to terminate that contract when Oath bought Yahoo, at which point Google became the default again. Presumably the new Google deal was around this amount, though it's arguable either way given Firefox's declining userbase on one hand, and on the other that it was so eager to nuke the Yahoo deal and that Yahoo fought back. 

    Assuming the same annual revenue from Google, its share of [Mozilla's total $451MM 2018 revenue](https://www.mozilla.org/en-US/foundation/annualreport/2018/) would be 83% and its share of the [$391MM in search royalties](https://www.computerworld.com/article/3487825/mozilla-in-trouble-2018-revenue-fell-20-expenses-exceed-income-for-first-time.html) would be a whopping 96%!

[^2]: I rounded this to account for the mix of desktop and mobile over this timeframe. At the beginning of 2009 Firefox held about 30% of the browser market share, with mobile representing less than 1% overall. As of this summer, it has about 8% of the desktop market and 4% overall, or loss of about 73.3% and 86.7% respectively. 

[^3]: Mozilla didn't technically abandon Thunderbird, but up until January 2020 it was essentially abandonware. It announced that month that [Thunderbird would move to a new wholly-owned subsidiary](https://blog.thunderbird.net/2020/01/thunderbirds-new-home/), MZLA Technologies, so that it could "explore offering [its] users products and services that were not possible under the Mozilla Foundation" and "collect revenue through partnerships and non-charitable donations." Thunderbird has had [one release since then in July 2020](https://blog.thunderbird.net/2020/07/whats-new-in-thunderbird-78/) that adds dark mode, a redesigned compose window, new folder icons, a cleaner account setup wizard, and OpenPGP support. While I would love to use it as my daily driver, there is very little hope that it will ever be more than even a community labor of love.