# buy http proxy: residential HTTP/HTTPS vs cheap lists, real plan prices, and how to pick without overpaying

Two different people type "buy http proxy" into the same search box, and they end up buying two completely different things.

The first wants volume: hundreds or thousands of endpoints, as cheap as possible, and doesn't care where they come from. That buyer usually ends up with a shared proxy list that works for about forty minutes. The second wants requests to a real site to succeed — stay logged in, load the page, keep the session alive — and has already wasted money on the first option.

The gap between those two buyers is the entire decision. So before we get to pricing, it's worth being precise about what "HTTP proxy" actually describes.

## HTTP is a protocol, not a product category

An HTTP proxy is a server that forwards HTTP requests on your behalf. That's it. "HTTP" tells you which protocol the proxy speaks, not what kind of IP sits behind it, how many other people share it, or whether it survives a CAPTCHA.

Most providers that let you buy an HTTP proxy offer it across several underlying IP types, and the IP type is what determines whether your job works:

- **Datacenter IPs** — fast, cheap, hosted on cloud infrastructure. Sites that care about traffic quality spot them quickly.
- **Residential IPs** — IPs assigned by real consumer ISPs to real devices. Higher trust, higher cost.
- **Mobile IPs** — carrier-assigned, high trust, high price.

Protocol support and IP type are separate axes. When someone advertises "buy HTTP proxies starting at $2/GB," they're usually selling residential IPs that happen to accept HTTP and SOCKS5 connections. When a paid list advertises "10,000 HTTP proxies for $20," they're usually reselling datacenter IPs of unknown provenance that were public last week.

If you specifically need to know how to buy an HTTP proxy that survives contact with a real website, the second option is where the money disappears.

## Where cheap HTTP proxy lists break

Public and ultra-cheap proxy lists have a real use case: quick geo-checks, rotating through endpoints for low-stakes requests, testing whether your scraper handles proxy failures gracefully. They're fine for that.

They stop being fine the moment a request matters. The IPs are shared, often recycled, and frequently already logged by anti-bot vendors. You get connection resets mid-session, occasional outright hijacking, and no support channel when it goes wrong. There's also the part nobody puts on the sales page: many of those lists are scraped from infected devices, which means you're routing your traffic — including credentials — through hardware you don't control and can't audit.

That isn't a moral lecture, it's a practical one. Proxies that were never properly sourced have a short useful life and unpredictable behaviour, which is exactly the opposite of what you want when you're paying per request.

## What to check before you pay

Five things separate a provider you'll keep using from one you'll regret:

1. **What the IPs actually are.** Residential, datacenter, ISP, or mobile. "Premium" tells you nothing.
2. **How billing works.** Per GB, per IP, or per request — and whether traffic expires.
3. **Targeting granularity.** Country is the minimum. City, ZIP, and ISP-level targeting is what makes location-dependent work possible.
4. **Session control.** Can you hold one IP for a fixed window, or rotate on every request?
5. **What happens when an IP dies.** Auto-replacement, or a support ticket and a wait?

One provider that answers all five clearly is 9Proxy, a residential proxy service that's been running since 2021 and sells into the mid-market rather than the enterprise tier.

## How 9Proxy's HTTP proxy offering works

9Proxy's network is residential-only — around 20 million IPs across 90+ countries, which is the figure most consistently reported across independent 2025–2026 reviews. You'll see larger numbers floating around the web; treat the headline count with a bit of suspicion either way.

Everything runs over **HTTP, HTTPS, and SOCKS5**, which is why it's relevant here at all. You're buying residential IPs, but you connect to them over the HTTP protocol like you would with any other proxy endpoint.

Targeting goes down to country, state, city, ZIP, and ISP, and you can bind those selections to specific ports.

The more interesting part is that 9Proxy splits its product into two billing models that fit genuinely different workflows:

**IP-based** — you buy a fixed number of residential IPs. Each activated IP gets unlimited bandwidth. Unused IPs in your balance don't expire. Each individual IP stays alive anywhere from a few hours up to roughly 24 hours, which suits session-stable work: multi-accounting, ad verification, anything where the same identity needs to persist across many requests.

**GB-based** — you buy traffic instead of IPs. You generate unlimited endpoints from the dashboard, no desktop app needed, and use sticky or rotating sessions as you like. Traffic is valid for 180 days. This is the right model when your requests rotate constantly and each one uses very little data.

Both authenticate with username/password or IP whitelisting. Both are managed from the same dashboard, alongside an API for generating proxy lists, rotating IPs, checking wallet balance, and managing sub-users.

If you want to see how the two models price out side by side, 👉 [👉 compare the current 9Proxy IP and GB packages here](https://bit.ly/9-Proxy).

## Full plan and price breakdown

9Proxy moved its IP-based and bundle pricing on 1 June 2026 — the first adjustment since launch. GB-based pricing was left untouched. The figures below reflect the current structure.

Packages are purchased as balances, not subscriptions, so a single payment covers one package rather than recurring monthly billing.

### IP-based residential packages — unlimited bandwidth per IP

| Package | Price per IP | Total | Buy |
| --- | --- | --- | --- |
| 100 IPs | $0.24 | $24 | [Bring in 100 IPs](https://bit.ly/9-Proxy) |
| 500 IPs | $0.144 | $72 | [Pick up 500 IPs](https://bit.ly/9-Proxy) |
| 1,000 IPs + 500 bonus | $0.084 | $126 | [Get 1,000 IPs plus 500 free](https://bit.ly/9-Proxy) |
| 2,500 IPs | $0.084 | $210 | [Scale to 2,500 IPs](https://bit.ly/9-Proxy) |
| 5,000 IPs | $0.072 | $360 | [Load 5,000 IPs](https://bit.ly/9-Proxy) |
| 15,000 IPs | $0.048 | $720 | [Order 15,000 IPs](https://bit.ly/9-Proxy) |
| 25,000 IPs | $0.035 | $863 | [Stock 25,000 IPs](https://bit.ly/9-Proxy) |
| 50,000 IPs | $0.029 | $1,438 | [Buy 50,000 IPs in bulk](https://bit.ly/9-Proxy) |

### Business IP packages — high volume

| Package | Price per IP | Total | Buy |
| --- | --- | --- | --- |
| 100,000 IPs | $0.023 | $2,300 | [Request 100,000 IPs](https://bit.ly/9-Proxy) |
| 200,000 IPs | $0.021 | $4,140 | [Request 200,000 IPs](https://bit.ly/9-Proxy) |
| 500,000 IPs | $0.018 | $8,625 | [Request 500,000 IPs](https://bit.ly/9-Proxy) |

### GB-based residential packages — 180-day validity

| Package | Price per GB | Total | Buy |
| --- | --- | --- | --- |
| 5 GB | $3.00 | $15 | [Start with 5 GB of traffic](https://bit.ly/9-Proxy) |
| 50 GB + 5 GB bonus | $2.10 | $105 | [Take the 50 GB pack plus 5 GB](https://bit.ly/9-Proxy) |
| 100 GB | $1.50 | $150 | [Buy 100 GB of traffic](https://bit.ly/9-Proxy) |
| 200 GB | $1.00 | $200 | [Buy 200 GB of traffic](https://bit.ly/9-Proxy) |
| 1,000 GB | $0.80 | $800 | [Buy 1,000 GB of traffic](https://bit.ly/9-Proxy) |
| 2,000 GB | $0.75 | $1,500 | [Buy 2,000 GB of traffic](https://bit.ly/9-Proxy) |

### Enterprise GB packages — no expiry

| Package | Price per GB | Total | Buy |
| --- | --- | --- | --- |
| 3,000 GB | $0.72 | $2,160 | [Enterprise 3,000 GB](https://bit.ly/9-Proxy) |
| 6,000 GB | $0.70 | $4,200 | [Enterprise 6,000 GB](https://bit.ly/9-Proxy) |
| 10,000 GB | $0.68 | $6,800 | [Enterprise 10,000 GB](https://bit.ly/9-Proxy) |

Enterprise adds team mode (one owner plus up to five members), per-member traffic controls, activity logs, unlimited data validity shared inside the team, and dedicated support.

### Bundle packages — IPs plus traffic

| Bundle | Contents | Price | Buy |
| --- | --- | --- | --- |
| Starter | 100 IPs + 5 GB | $30 | [Grab the Starter bundle](https://bit.ly/9-Proxy) |
| Popular | 1,500 IPs + 50 GB | $180 | [Grab the Popular bundle](https://bit.ly/9-Proxy) |
| Pro | 5,000 IPs + 500 GB | $720 | [Grab the Pro bundle](https://bit.ly/9-Proxy) |

Bundled traffic carries the same 180-day validity as standalone GB packages. If you need both stable IPs and flexible rotation, the bundles price below buying the two components separately.

## Which package actually fits your job

Here's the mapping, without pretending every option is equally good for everyone.

**Testing the water:** the 100 IP package at $24, or 5 GB at $15 if your work is bandwidth-shaped. Enough to run a few hundred real requests against your actual targets and see what the success rate looks like on your traffic.

**Multi-account or profile work:** IP-based, 500 IPs and up. Unlimited bandwidth per IP means you're not watching a traffic meter while a session runs. The 1,000 + 500 tier is the better value at $126 than 1,000 raw IPs would be at the same per-unit rate.

**Scraping with heavy rotation:** GB-based. The 50 + 5 GB pack at $105 is the sweet spot for light ongoing work; the 200 GB tier at $1.00/GB is where per-request cost stops being annoying.

**Reseller or agency:** the 25,000 and 50,000 IP tiers, or Business packages past 100,000. Per-IP cost drops to $0.029 and below. 9Proxy also runs a reseller programme with wholesale pricing.

**Mixed workloads:** bundles. Starter covers a small client pilot, Pro covers a shop running several verticals at once.

## Setting up the HTTP proxy itself

The mechanics are unremarkable, which is a good thing.

For GB-based IPs, everything happens in the dashboard. Create a sub-user, assign traffic, generate endpoints with your country/city/ISP filters, and export as `.txt` or `.csv`. Auth is username/password or an IP whitelist. A structured username carries the targeting, in this shape:


<subaccount>-country-<code>-st-<state>-city-<city>-isp-<isp>-ssid-<session_id>-sst-<session_time>


Then it's a standard HTTP connection. In `curl`:


curl -x http://USER:PASS@gate.9proxy.com:7777 https://httpbin.org/ip


In Python, the same credentials drop straight into the `proxies` dict. Proxifier handles apps that have no native proxy settings; FoxyProxy handles Chrome. IP-based packages historically required the 9Proxy desktop app for local port forwarding, though the browser-based Proxy2Web tool now removes that requirement on tablets, remote machines, and locked-down systems.

9Proxy also publishes an API if you'd rather provision endpoints programmatically than click through a dashboard.

## The parts that will actually annoy you

Worth knowing before checkout rather than after.

**No openly advertised free trial.** Third-party reviews consistently flag this. There's a narrow refund policy — credit for IPs that die within roughly 60 seconds — which is why Trustpilot complaints tend to come from buyers who picked the wrong plan and couldn't recover the spend. Buy the smallest tier first, run your real workload against it, then scale.

**Residential only.** No datacenter, ISP, or mobile products. If your job genuinely needs cheap datacenter throughput, this isn't the provider — and bundling residential IPs into a task that doesn't need them is just paying more for the same result.

**Streaming is off the table.** 9Proxy has signalled that media streaming services (YouTube being the example given) are no longer supported on IP-based plans under its updated acceptable use policy. Confirm current terms if streaming was the plan.

**Published performance numbers are vendor claims.** 9Proxy advertises roughly 99.5% success rate, ~0.6s average response time, and 99.95% uptime. Independent benchmark data puts success around 97% with P95 latency nearer 1.3s on rotating residential. Both are plausible; neither is an SLA you can hold anyone to. Test on your own targets.

**Pool size figures vary.** The 20M/90-country figure is the most consistently corroborated. Some promotional pages claim considerably more.

On payments: cards, bank cards, Apple Pay, Google Pay, Alipay, and crypto through CoinPayments (BTC, ETH, LTC, TRX, USDT on both TRC20 and ERC20, DOGE, DAI, BCH). Crypto payments reportedly carry a +5% IP bonus. 9Proxy's affiliate programme also advertises a 5% discount for referred users, which is what the invite link on this page carries.

One more cost lever: the Today List lets you reuse IPs forwarded in the previous 24 hours without spending a new IP from your balance, provided the IP is still online. On IP-based plans that can meaningfully cut how many IPs a project actually consumes. Auto Refresh replaces dead IPs within about a minute, which matters more than it sounds — a session that dies mid-run costs you the run.

## Questions people ask before buying

**Do I need a desktop app?** For GB-based proxies, no — the dashboard handles everything. For IP-based proxies, the desktop app was the traditional route; Proxy2Web is the browser-based alternative.

**Can I get the same IP twice?** Yes, using structured session parameters in the username and a sticky session window. GB-based proxies let you set that window yourself.

**What happens to unused IPs?** They stay in your balance without expiring until activated. Unused GB traffic follows the 180-day validity window, unless you're on an Enterprise package.

**Is there a monthly subscription?** No. 9Proxy bills by balance — you buy a package, you spend it. No recurring charge to forget about.

## The short version

If you're buying an HTTP proxy to route real traffic into real websites and you don't want to babysit connection failures, the protocol is the easy part — the IP type behind it is what you're actually paying for. Residential IPs with unlimited bandwidth per IP are the pragmatic choice for session-based work; per-GB billing is the pragmatic choice when your requests rotate constantly and each one is small.

9Proxy sits at the affordable end of that market with a dual billing model that lets you switch based on workload rather than switching providers. Start with the 100 IP or 5 GB tier, run your own targets through it, and let the results decide whether the next purchase is 500 IPs or 50,000.

👉 [👉 Create your 9Proxy account and test the HTTP endpoint on your own workload](https://bit.ly/9-Proxy)
