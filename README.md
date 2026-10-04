# bulk proxies: how to size a bulk order and compare per-IP vs per-GB pricing without overpaying

Search for bulk proxies and you get three different products back, all wearing the same label. One is a pile of IP addresses with unlimited bandwidth attached. Another is a pile of traffic measured in gigabytes. The third is both, bundled at a discount. Pick the wrong unit and you either burn money on gigabytes you never consume or run out of IPs in the middle of a campaign.

This is a practical guide to buying residential proxies at volume: what the units actually mean, what the current rates look like at 9Proxy (the provider behind the link in this article), and how to do the math before you pay.

If you'd rather skip straight to the numbers, 👉 9Proxy's current package list is the fastest way to see the tiers side by side.

## What "bulk" means in proxies, and why the units don't compare

A "bulk proxy" purchase is almost always one of these:

- **Bulk IPs.** You buy a fixed number of residential IP addresses. Each one works for as long as it stays alive, and bandwidth through it is unlimited.
- **Bulk bandwidth.** You buy a pool of gigabytes and create as many proxy endpoints as you want. You're metered on data, not on addresses.
- **Bundles.** A few IP packages come with traffic attached, for teams running mixed workloads.

Datacenter vs residential is a separate axis. Datacenter IPs are cheap and fast but get blocked on harder targets. Residential IPs route through real home connections, which is why they survive anti-bot checks and why they cost more.

9Proxy sells residential only, in two models: per-IP and per-GB. That's it. No datacenter product on the menu, which matters if your project is the kind where datacenter IPs would do the job at a tenth of the price.

## Per-IP bulk buying: unlimited bandwidth, finite addresses

The per-IP model is 9Proxy's original product. You buy addresses, not traffic, so a job that moves 200 GB through 50 IPs costs the same as a job that moves 20 GB through 50 IPs.

What you're actually getting:

- **Unlimited bandwidth per IP** while the address is active, with no monthly subscription attached.
- **Unused IPs never expire.** Buy 5,000, use 800 this month, the rest sit on your balance.
- **Each forwarded IP is consumed.** This is the part most buyers miss. IP-based units are spent as you use them, and a residential IP typically stays alive somewhere between a few hours and about 24 hours.
- **The desktop app is mandatory.** IP-based proxies run through 9Proxy's app with local port forwarding. There's an auto-rotation proxy for cycling at custom intervals on selected ports.

That last point changes how you size an order. If your workflow pulls 100 fresh IPs a day, a 2,500-IP package lasts roughly three and a half weeks, not forever. If you burn 20 a day, the same package stretches past four months.

Here's the current per-IP ladder, including the wholesale tiers:

| Package size | Price per IP | Billing | Typical fit |
| --- | --- | --- | --- |
| 100 IPs | $0.24 | One-off, unused IPs don't expire | Proof of concept, small tests |
| 500 IPs | $0.144 | One-off | Solo operators, light multi-account work |
| 1,000 IPs + 500 bonus | $0.084 | One-off | Small teams with steady daily usage |
| 2,500 IPs | $0.084 | One-off | Several verticals running at once |
| 5,000 IPs | $0.072 | One-off | Agencies, mid-scale scraping |
| 15,000 IPs | $0.048 | One-off | Multi-region operations |
| 25,000 IPs | $0.035 | One-off | Resellers and heavy automation labs |
| 50,000 IPs | $0.029 | One-off | Platform-level volume |
| 100,000 IPs (business tier) | $0.023 | One-off | Industrial-scale crawling |
| 200,000 IPs (business tier) | $0.021 | One-off | Large reseller inventory |
| 500,000 IPs (business tier) | $0.018 | One-off | Wholesale distribution |

The headline rate on the site is $0.018 per IP, and that's the 500,000-IP tier. Everything below it sits between $0.024 and $0.144 per address.

👉 If your volume sits in the 5,000 to 50,000 range, it's worth comparing against the whole pricing ladder rather than guessing at the tier you need.

## Per-GB bulk buying: unlimited endpoints, metered traffic

The GB model is the one built for rotation-heavy work. Instead of buying addresses, you buy traffic and generate as many proxy endpoints as you like. Only the gigabytes get deducted.

Where this model wins: scraping thousands of different targets, price monitoring across regions, ad verification, SERP tracking, anything where each request is small and you'd rather rotate through a large pool than pin yourself to specific addresses.

What's included:

- **Sticky or rotating sessions**, configurable per job.
- **Authentication by username/password or IP whitelisting.** The whitelist option skips credentials entirely, which is handy for cloud scripts.
- **Targeting down to country, state, city, ZIP, and ISP.**
- **Everything runs from the dashboard.** No app, no local port forwarding.
- **180-day validity on every GB package.** Your traffic doesn't vanish at the end of the month.
- **Sub-users.** You can split traffic across sub-accounts, useful when several clients share one balance.

| Package | Price per GB | Total | Validity |
| --- | --- | --- | --- |
| 5 GB | $3.00 | $15 | 180 days |
| 50 GB + 5 GB bonus | $2.10 | $105 | 180 days |
| 100 GB | $1.50 | $150 | 180 days |
| 200 GB | $1.00 | $200 | 180 days |
| 1,000 GB | $0.80 | $800 | 180 days |
| 2,000 GB | $0.75 | $1,500 | 180 days |

Larger traffic commitments drop further, down to $0.68 per GB at the top of the range. Go high enough and 9Proxy moves you into the Enterprise program, which removes the expiry entirely, adds team mode for one owner plus five members, per-member traffic controls, activity logs, and unlimited share codes.

The 180-day window is the detail that separates GB buying from most subscription-based providers. If your scraping is seasonal, you don't forfeit unused bandwidth when the month rolls over. Buy 200 GB in March, use half of it in June, the rest is still there.

👉 Traffic-based pricing only pays off when each request is light, so check the per-GB tiers before committing to a large package.

## Bundles: when you need both units

Some workloads need stable addresses for account sessions and rotating traffic for crawling at the same time. Bundles put both on one balance instead of forcing two separate purchases.

| Package | Price | What's inside |
| --- | --- | --- |
| Starter bundle | $30 | 100 IPs + 5 GB |
| Mid-tier bundle | $180 | 1,500 IPs + 50 GB |
| Pro bundle | $720 | 5,000 IPs + 500 GB |

Bundled traffic follows the same 180-day validity rule as standalone GB packages.

## How to size a bulk order without guessing

Two calculations cover most buying decisions.

**Bandwidth math.** Multiply your monthly request count by the average response size. 200,000 page fetches at roughly 250 KB each lands near 50 GB. At 9Proxy's $2.10 per GB tier, that's about $105 to cover the month, with 180 days to spend it.

**IP math.** Divide your package size by the number of fresh IPs you burn per day. That gives you the lifespan. A 2,500-IP package at 80 IPs a day runs out in about a month.

Now compare the two costs for your actual workload. If each request pulls a heavy page and you need long sessions, per-IP is usually cheaper because bandwidth stops mattering once you've bought the address. If each request is small and you want a new IP constantly, per-GB is the better unit, and buying IPs you'll never forward is just dead inventory.

The mistake worth avoiding: buying rotating bandwidth for a job that only needs a handful of static addresses in specific countries. That's the most common way to overspend in this category.

## Where 9Proxy's rates sit against the rest of the market

The residential proxy market splits roughly into three price bands. Premium providers like Bright Data and Oxylabs start around $4 to $6 per GB. Mid-market options such as Decodo sit near $2.75 to $4 per GB. Then there's the budget band, where 9Proxy's $0.75 to $3 per GB pricing lands, alongside providers like DataImpulse.

On per-IP volume, $0.018 at the wholesale end is unusually low for residential addresses, and that rate is what the provider leads with in its advertising.

Advertised specs, per the company's own documentation: 20 million-plus residential IPs across more than 90 countries, with a claimed 99.95% uptime.

Independent coverage is more measured. Directory listings put 9Proxy in the budget category with ratings around 3.9 out of 5, noting the per-IP model and the low entry price as the main draw. One reviewer flagged that the smaller pool compared with 100M-plus competitors could limit very specialised targeting, and that streaming services like Netflix sometimes detect the IPs. If your project is unblocking streaming catalogues, this isn't the provider to build on. If it's scraping product data, SERP tracking, or managing multiple accounts, the pool size is less of a constraint.

## Fine print that changes the real cost

Before a large purchase, these are the terms that decide whether the rate you saw is the rate you pay:

**IP-based packages need the desktop app.** Running 200 browser profiles through an app on one machine gets awkward. If your stack lives in the cloud, the GB model is the one that fits, since it works entirely from the dashboard.

**Residential IPs die at uneven rates.** A few hours to about 24 hours per address is normal for this category. Independent reviews note a replacement window of roughly 60 seconds for IPs that arrive dead, which softens the problem, but you're still managing churn.

**The GB model caps your traffic, not your endpoints.** Creating 50,000 endpoints costs nothing extra. Draining your balance does.

**There's no standard self-serve free trial.** Trial codes are promotional and typically come from support, so budget for a small paid test rather than waiting on a free tier. A 5 GB pack at $15 is enough to measure success rates on your targets before you commit to 2,000 GB.

**Payment options are broad.** Cards, bank cards, crypto including USDT, BTC, ETH, LTC and DOGE, plus Alipay, Apple Pay and Google Pay. Crypto is the usual choice if you want to buy a large balance without card limits getting in the way.

## Getting the best rate on a bulk order

Volume tiers aren't hidden, they're the whole pricing structure. Moving from 100 IPs to 500 cuts the per-IP rate by 40%; moving to 5,000 IPs cuts it by 70%. If your monthly burn is anywhere near the next tier, buying up once is almost always cheaper than buying twice.

A few other levers:

- **Payment-method bonuses.** Some payment options carry an extra 5% discount or a 5% product bonus.
- **Weekend usage rebates.** 9Proxy runs a "Green Sunday" promotion giving 10% of Sunday usage back as credit — worth knowing if your schedule is flexible.
- **Price history.** The provider raised IP-based and bundle prices on 1 June 2026, the first increase since launch, moving the entry per-IP headline rate from $0.015 to $0.018. GB-based packages were untouched. That means today's bandwidth pricing has been stable for a long time, while IP pricing is the line item that moves.
- **Reseller and affiliate terms.** Wholesale pricing on 200,000-plus IP tiers, plus a lifetime affiliate program paying up to 15% commission with a discount for referred buyers.

👉 The bundle packages are the simplest way to test both units on one balance before committing to a six-figure IP order.

## Quick answers

**How many proxies do I need for scraping?**
Enough to cover your daily concurrency and rotation needs. Work backwards from requests per hour, then multiply by the number of parallel workers. Most teams start too large, discover half their IPs unused, and downshift on the second purchase.

**Do bulk proxy packages expire?**
At 9Proxy, unused IPs don't expire. GB packages carry 180-day validity, and Enterprise plans remove the expiry entirely.

**Is per-IP or per-GB cheaper?**
Per-IP wins when pages are heavy and sessions are long, because bandwidth is unlimited. Per-GB wins when requests are small and you need constant rotation. Run the two calculations on your own numbers before choosing.

**Can I resell these proxies?**
The business tiers at 100,000 IPs and above exist for exactly that, with wholesale per-IP pricing and dedicated support.

**Is 9Proxy good for streaming?**
Independent reviews report detection on services like Netflix. Residential proxies can work for it, but this provider is aimed at scraping, automation, and account management rather than geo-unblocking catalogue content.

## The short version

Bulk proxy buying is a unit problem before it's a price problem. If you need stable addresses with unlimited bandwidth, buy IPs and size the order around your daily burn rate. If you need constant rotation with light requests, buy gigabytes and stop counting addresses. If you need both, a bundle is cheaper than two separate purchases.

9Proxy's numbers are straightforward: $0.018 to $0.24 per IP depending on volume, $0.75 to $3.00 per GB depending on commitment, no subscriptions, and 180 days to use the traffic. The trade-offs are the mandatory app on IP-based packages, a 20-million-IP pool that's smaller than the premium providers', an uneven IP lifespan, and no datacenter option.

👉 If those terms fit your workflow, the full package list and current rates are one click away.
