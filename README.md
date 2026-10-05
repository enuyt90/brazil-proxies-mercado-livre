# Brazil Proxies: How to Pick Brazilian Residential IPs for Mercado Livre Scraping, pt-BR SERP Tracking and Ad Verification

Brazil is one of the cheaper countries to buy proxy traffic in, which is good news, because Brazilian work tends to be volume-heavy. Scraping Mercado Livre listings eats gigabytes fast. So does pulling local search results across a dozen cities. The question is rarely "are Brazilian IPs affordable" — it's which proxy type survives contact with the target, and whether the per-GB number on the pricing page is the number you actually pay.

This walks through what people use Brazilian IPs for, how the four proxy types differ, what the real cost looks like on a pay-as-you-go provider, and where the setup gets fiddly.

## What people actually do with Brazilian IPs

A Brazilian exit IP isn't a general-purpose anonymity tool. It solves specific problems, and most of them are commercial.

**Localized pricing and listings.** Mercado Livre, Magazine Luiza, Americanas and Casas Bahia all serve different prices, stock states and shipping terms depending on where the request originates. Pull those pages from a US datacenter and you get a version of the site that no Brazilian buyer ever sees. Mercado Envios labels, "chega amanhã" delivery promises and seller reputation data are all location-sensitive.

**Portuguese-language SERP tracking.** Rankings on google.com.br don't mirror google.com. Local packs, shopping units, the mix of .com.br domains versus international ones, and the way Portuguese queries get matched — none of that reproduces from an IP in Frankfurt. If you're tracking keyword positions for a Brazilian market, the IP is part of the measurement instrument.

**Ad verification.** A campaign aimed at São Paulo needs to be checked from São Paulo. Creative rendering, landing page redirects, promo banners with local pricing and delivery cutoffs behave differently per region, and checking them from outside Brazil tells you almost nothing.

**Streaming and geo-locked content.** Globoplay, SporTV, SBT and RecordTV restrict access by location. This is the use case that gets advertised hardest and understood worst — residential IPs work for it, but a session that drops mid-episode because the underlying device went offline is a normal residential-pool behavior, not a bug.

**Ticketing, drops and account work.** Brazilian event sales and sneaker releases often queue by region. Multi-account operations on Brazilian platforms need each account on its own IP, and mobile IPs carry the highest trust there because carrier-grade NAT means one address is shared by thousands of real subscribers, making it expensive for a platform to block outright.

**App and network testing on Brazilian carriers.** If you're validating how a product behaves on Vivo, Claro or TIM, you need IPs from those networks, not just from Brazil.

## The four types of Brazilian IPs, and which one you need

| Type | Where the IP comes from | Detection risk | Typical 2026 price | Best for |
| --- | --- | --- | --- | --- |
| Residential | Real home broadband connections | Low | ~$1–8/GB | Mercado Livre, SERPs, ad verification, streaming |
| Mobile | 4G/5G/LTE carrier networks | Lowest | ~$2–15/GB | Social accounts, anti-fraud-gated flows, app testing |
| Datacenter | Server subnets | High | ~$0.50–3/GB | High-volume pulls from sites without serious bot defenses |
| ISP / static residential | Datacenter-hosted IPs registered to ISPs | Low | ~$1.50–5/IP/month | Long-lived accounts that need a fixed address |

The rule that saves the most money: don't pay mobile rates for work a datacenter IP would survive. Brazilian news portals, some smaller retailers and plenty of public data sources don't run aggressive bot detection, and $0.50/GB gets that job done. Save the $2/GB mobile traffic for the targets that actually fingerprint their visitors.

The other thing to know up front: **static ISP proxies are a different product category**, and not every provider sells them. If your workflow needs the same Brazilian IP for months on end, check that before you buy anything else.

## What Brazilian IPs should cost right now

Fair ranges for 2026 sit around $1–8/GB for residential, $0.50–3/GB for datacenter and $2–15/GB for mobile. Value-tier pay-as-you-go providers cluster near the bottom of those bands; enterprise pricing sits at the top.

The headline rate is rarely the full story. Three things move the real number:

- **Traffic expiry.** If unused gigabytes reset at the end of the month, your effective cost per useful gigabyte is higher than advertised — you paid for data you never got to spend.
- **Targeting surcharges.** Country-level targeting is usually included. State, city, ZIP and ASN filtering frequently isn't.
- **Minimum commitments.** A low per-GB rate paired with a large mandatory monthly spend has a higher entry cost than a slightly higher rate with a $5 start.

One concrete reference point: DataImpulse prices residential at $1/GB with no subscription, country targeting included, and traffic that never expires. Brazil costs the same as anywhere else on that grid — there's no Brazil premium. The catch is granularity, and it's worth spelling out because it changes budgets.

> Country targeting on DataImpulse's residential and mobile pools is free. State, city, ZIP code and ASN filters are billed at double the standard rate on residential plans, so a São Paulo-only residential job runs at an effective ~$2/GB, not $1/GB. Datacenter lists those same targeting options as included features.

That's the difference between a $50 job and a $100 job, and it's documented rather than hidden — DataImpulse's own parameter documentation states that state-level traffic is billed at twice the standard rate.

## The full DataImpulse lineup

DataImpulse runs four products on one pay-as-you-go model. There's no free tier; access starts at $5, which is enough real traffic to test Brazil targeting before committing.

| Proxy type | Plan | Traffic | Price | Rate per GB | Get it |
| --- | --- | --- | --- | --- | --- |
| Residential | Intro | 5 GB | $5 | $1.00 | [start with the 5 GB residential intro](https://dataimpulse.com/residential-proxies/?aff=86938) |
| Residential | Basic | 50 GB | $50 | $1.00 | [grab the 50 GB residential plan](https://dataimpulse.com/residential-proxies/?aff=86938) |
| Residential | Advanced | 1 TB | $800 | $0.80 | [see the 1 TB residential tier](https://dataimpulse.com/residential-proxies/?aff=86938) |
| Residential | Custom | 5 TB+ | from $4,000 | quoted | [request custom residential volume](https://dataimpulse.com/residential-proxies/?aff=86938) |
| Datacenter | Intro | 10 GB | $5 | $0.50 | [open the 10 GB datacenter intro](https://bit.ly/dataimPulse) |
| Datacenter | Basic | 100 GB | $50 | $0.50 | [check the 100 GB datacenter plan](https://bit.ly/dataimPulse) |
| Datacenter | Advanced | 1 TB | $450 | $0.45 | [review the 1 TB datacenter tier](https://bit.ly/dataimPulse) |
| Datacenter | Custom | 5 TB+ | from $2,250 | quoted | [ask for custom datacenter pricing](https://bit.ly/dataimPulse) |
| Mobile | Intro | 2.5 GB | $5 | $2.00 | [try the 2.5 GB mobile intro](https://bit.ly/dataimPulse) |
| Mobile | Basic | 25 GB | $50 | $2.00 | [see the 25 GB mobile plan](https://bit.ly/dataimPulse) |
| Mobile | Advanced | 1 TB | $1,600 | $1.60 | [look at the 1 TB mobile tier](https://bit.ly/dataimPulse) |
| Mobile | Custom | 5 TB+ | from $8,000 | quoted | [request custom mobile volume](https://bit.ly/dataimPulse) |
| Premium Residential | Intro | 1 GB | $5 | $5.00 | [start with 1 GB premium residential](https://dataimpulse.com/premium-residential-proxies/?aff=86938) |
| Premium Residential | Basic | 10 GB | $50 | $5.00 | [see the 10 GB premium residential plan](https://dataimpulse.com/premium-residential-proxies/?aff=86938) |
| Premium Residential | Custom | 1 TB+ | custom quote | quoted | [ask about premium residential volume](https://dataimpulse.com/premium-residential-proxies/?aff=86938) |

Every plan includes rotating and sticky sessions, HTTP/HTTPS/SOCKS5, username-password and IP-whitelist authentication, and traffic that doesn't expire. The company publishes a 99.51% success rate and claims 99.9% uptime — note that it does **not** publish an average response time, which is worth knowing if you're comparing providers on latency figures alone.

### How to read that grid

The residential pricing curve is unusually flat. From 5 GB through roughly 850 GB it stays at $1/GB, and the only discount step arrives at 1 TB. Buying 200 GB costs $200. Buying 50 GB costs $50. There is no intermediate reward for committing to more.

That actually simplifies planning. Estimate your monthly Brazilian traffic honestly, buy that, and let the remainder roll over. A month where Mercado Livre scraping spikes doesn't waste anything, because unused gigabytes stay in the account.

For a typical Brazilian marketplace job at, say, 20 GB/month of residential traffic with country-level targeting, you're looking at $20/month plus whatever you lose to retries. Add city-level filtering and that doubles. The comparison that matters isn't $1/GB versus $0.80/GB — it's cost per successfully scraped record, and a cheap pool that returns blocks is more expensive than a slightly pricier one that doesn't.

## Setting up a Brazil-targeted endpoint

Country selection is a parameter, not a separate purchase. DataImpulse's documented format appends targeting to the username, separated by a double underscore, with parameters formatted as `key1.value1,value2;key2.value1`:

bash
curl -x "http://yourlogin__cr.br:yourpassword@gw.dataimpulse.com:823" https://api.ipify.org/


The host is `gw.dataimpulse.com`. Port 823 handles HTTP/HTTPS; port 824 is the SOCKS5 endpoint. The `cr.br` segment is the country selector, and you can pass multiple countries with a comma if you're comparing Mercado Livre Brazil against Argentina or Mexico.

Everything else is configurable from the dashboard, which generates a ready-made proxy list and a live cURL string that updates as you change settings — useful for a sanity check without leaving the browser.

Rotating versus sticky is the decision that matters most for Brazilian work:

- **Rotating** assigns a fresh IP per request. This is what you want for scraping listings at volume, because distributing requests across many addresses is what keeps success rates up.
- **Sticky** pins one IP to a port for a defined window, configurable from 1 to 120 minutes, averaging around 30. Use it for login flows or multi-step journeys where the IP changing mid-session would break things.

One honest caveat: sticky duration isn't guaranteed. These are real users' connections, and when the device goes offline the session rotates to the next available IP automatically. If you're building anything stateful, handle a mid-session IP change rather than assuming it won't happen.

## Where this setup has limits

Worth stating plainly, because they'll show up in your first week:

- **No static ISP proxies.** DataImpulse sells rotating residential, mobile, datacenter and premium residential. Long-term account management on a fixed Brazilian IP isn't something you can buy here.
- **Granular targeting doubles residential cost.** City, ZIP and ASN filtering is billed at 2× on residential. Datacenter includes those filters.
- **Minimum order thresholds.** The first order can be as small as $5, but at least one published review reports the minimum rising to $50 on subsequent top-ups. If you're planning a small ongoing pilot, confirm this with support before you budget on it.
- **Some categories are blocked.** A community review reports that government sites, banking and payment domains, bandwidth-sharing platforms and mail services are excluded, alongside a default 2000-thread concurrency limit.
- **Refund terms differ by payment method.** Intro plans carry a 7-day money-back guarantee on card payments, contingent on less than 80% of traffic being consumed. Crypto purchases on intro plans are non-refundable.
- **Brazilian pool size isn't a headline number.** DataImpulse publishes a per-country IP count list. Check Brazil's figure on that list before you buy — that's exactly what it's there for, and it beats taking anyone's word about coverage.

## Free Brazilian proxy lists and why they fail

Public lists update hourly and look tempting if you just want to see what google.com.br shows. For a single manual check, fine.

For anything recurring, the numbers don't work. Independent analysis of free proxy lists puts success rates somewhere around 15–30%, with nodes dying within 12–48 hours. The IPs are also shared with hundreds of other users, meaning most are already flagged by the time you get them. And since these are anonymous third-party operators, they can read or modify any unencrypted request passing through — which is why you should never route credentials or payment data through one.

The gap between a free Brazilian IP and a paid one isn't speed. It's whether the request succeeds at all.

## A buying checklist for Brazilian proxies

Before you spend anything:

1. Confirm the provider's per-country IP count for Brazil, not just its global pool figure.
2. Work out whether your target needs a rotating residential IP, a sticky one, or a mobile one. Paying mobile rates for Mercado Livre product pages is overspending.
3. Check how city and ZIP targeting is billed. On residential pools it's often a multiplier, and it's the line item that blows up budgets.
4. Verify the provider supports the country parameter on the pool you're buying, and test it with a `curl` call to an IP lookup endpoint before running a real job.
5. Check the minimum order size and whether purchased traffic expires.
6. Read the refund terms by payment method, not just the headline guarantee.

## FAQ

**Residential or mobile IPs for Mercado Livre?**
Residential, in most cases. Product pages, pricing and seller data don't require carrier-grade IPs. Reach for mobile only if you're hitting flows with fraud scoring attached, like account creation or checkout testing.

**Can I target São Paulo or Rio de Janeiro specifically?**
Yes, through city-level filtering — but on residential plans that traffic is billed at twice the standard per-GB rate. Datacenter lists city, ZIP and ASN filtering as included.

**Does a Brazil proxy change my browser fingerprint?**
No. A proxy changes the IP. Platforms also read language settings, timezone, screen size and OS. An IP that says Brazil paired with a browser reporting US English and a New York timezone is a mismatch, and mismatches are what trigger verification prompts. If you're running account work, pair the proxy with an antidetect browser profile configured for Brazil.

**Is there a free trial?**
No. The lowest entry point is a $5 intro plan. Intro plans carry a 7-day money-back guarantee on card payments as long as under 80% of the traffic is used.

**How do I check my IP is actually Brazilian?**
Route a request to an IP lookup service through the proxy and read the country field. It's a two-second test and worth running on every new plan.

**Is scraping Brazilian sites legal?**
Collecting publicly accessible data is generally treated as legitimate for market research and price monitoring, but Brazil's LGPD imposes rules on personal data, and scraping behind authentication or circumventing access controls sits in different territory. Get your own legal read for anything beyond public pages.

## The short version

Brazilian IPs are cheap, Brazilian work is volume-heavy, and the two facts point the same direction: buy per-gigabyte traffic that doesn't expire, keep country targeting free, and only pay the city-targeting multiplier when the job genuinely depends on it.

DataImpulse fits that shape at $1/GB residential with a $5 entry point and rollover traffic — a reasonable place to run a real Brazilian test rather than a sandbox demo. What it won't do is give you static ISP addresses or a free tier, so if either is a hard requirement, look elsewhere first.

👉 [Start with the $5 intro plan and test Brazil targeting on your own traffic](https://bit.ly/dataimPulse)
