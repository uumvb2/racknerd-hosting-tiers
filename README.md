# cheap wordpress hosting plans: what $10.49 a year actually gets you, and how to pick the right RackNerd tier

Most "cheap WordPress hosting" pages you'll open this week advertise a $3-ish monthly price, then quietly renew at three to five times that. RackNerd runs the opposite play: the promo price you sign up at **is** the renewal price, locked for as long you keep the account. Their shared hosting starts at **$10.49/year** for the 30 GB promo tier, which works out to about $0.87 a month, and every tier ships with cPanel, LiteSpeed, CloudLinux, daily offsite backups, and one-click WordPress install.

This article breaks down the full plan lineup, the math on what you really pay, the limits that only show up in the fine print, and a setup walkthrough — so you can decide in one read.

> **Quick pick:** running one blog, portfolio, or small business site? The Shared 30 GB promo tier at $10.49/year is enough — a typical WordPress install takes 500 MB to 1 GB, and most content sites never pass 10 GB of actual disk use. 👉 [Order the 30 GB promo tier at $10.49/year](https://my.racknerd.com/aff.php?aff=11397&pid=933)

## RackNerd's shared hosting plans, all of them

RackNerd sells two parallel lines of shared hosting, and mixing them up is the most common way people overpay. The **promo tiers** bill annually (tied to their Black Friday, 11.11, and New Year promo cycles), run on NVMe storage, and cap the number of domains on the lower tiers. The **standard tiers** bill monthly with no contract, use SSD storage, and allow unlimited domains.

First, the promo annual tiers — this is where the headline prices live:

| Plan | Storage | Monthly transfer | Hosted domains | Price | Buy |
| --- | --- | --- | --- | --- | --- |
| Shared — 30 GB | 30 GB NVMe | 3 TB | 3 (1 primary + 2 add-on) | $10.49/year | [Get the 30 GB promo plan](https://my.racknerd.com/aff.php?aff=11397&pid=933) |
| Shared — 85 GB | 85 GB NVMe | 10 TB | 11 (1 primary + 10 add-on) | $24.99/year | [Get the 85 GB promo plan](https://my.racknerd.com/aff.php?aff=11397&pid=934) |
| Shared — 200 GB | 200 GB NVMe | 30 TB | Unlimited add-on domains | $59.00/year | [Get the 200 GB promo plan](https://my.racknerd.com/aff.php?aff=11397&pid=935) |

And the standard monthly tiers, for anyone who doesn't want to prepay a year:

| Plan | Storage | Monthly transfer | Hosted domains | Price | Buy |
| --- | --- | --- | --- | --- | --- |
| Shared — 30 GB | 30 GB SSD | 2 TB | Unlimited | $5.59/month | [Order the 30 GB monthly plan](https://my.racknerd.com/aff.php?aff=11397&pid=81) |
| Shared — 100 GB | 100 GB SSD | 3 TB | Unlimited | $9.59/month | [Order the 100 GB monthly plan](https://bit.ly/RacKnerd) |
| Shared — 200 GB | 200 GB SSD | 5 TB | Unlimited | $15.59/month | [Order the 200 GB monthly plan](https://bit.ly/RacKnerd) |

Every tier — promo or standard — includes the same core stack: cPanel, LiteSpeed Web Server with LSCache, CloudLinux isolation, KernelCare, free Let's Encrypt SSL with auto-renewal, Softaculous one-click installs, JetBackup daily offsite backups, free migration from any cPanel host, and 24/7 support with a published average ticket response around 10 minutes. The tiers differ only in storage, bandwidth, and domain count. There's no "starter plan that secretly lacks backups" trick here.

At checkout you pick a datacenter: Los Angeles, New York (Newark, NJ — added in October 2025), Frankfurt, Strasbourg, or Singapore. Pick whichever is closest to your readers, not to you.

## What you're actually paying for under the hood

The reason this stack matters for WordPress specifically: the current shared fleet runs on **AMD Ryzen 7950X** processors (boost up to 5.70 GHz per core), 128 GB DDR5 RAM per node, Gen4 NVMe storage, CloudLinux 9, and **LiteSpeed Enterprise** as the web server.

WordPress is mostly single-threaded PHP, so per-core clock speed drives how fast your pages render. That 5.7 GHz boost figure is the number that matters, and it's the same spec managed WordPress hosts charge a multiple of this price for.

The software side covers the things you'd otherwise pay separate licenses for:

- **LiteSpeed + LSCache** — server-level caching that serves cached pages as static files before PHP even gets involved. During a traffic spike from social media, this is the difference between your site surviving and collapsing.
- **CloudLinux 9** — every account sits in its own container with fixed CPU, RAM, and I/O limits, so a neighbor's runaway plugin can't drag your site down.
- **cPGuard** — malware scanning and a WAF that blocks brute-force logins and xmlrpc abuse. A standalone license for this class of tool runs $200+/year; it's included.
- **JetBackup** — daily backups copied offsite to Wasabi cloud storage, restorable yourself from inside cPanel.
- **Softaculous** — one-click installer for WordPress and 400+ other apps.

If you tried to assemble this stack yourself on a cheap VPS, the cPanel license alone would run you $15+ a month before you added LiteSpeed, CloudLinux, JetBackup, and everything else. That's the actual benchmark for whether $10.49 a year is a real deal or a bait number.

## The real cost math, including renewals

This is the part most roundup articles skip, and it's where cheap hosting deals usually fall apart.

The standard industry pattern, per CNET's 2026 hosting roundup: shared and WordPress plans advertise at $3–$8 a month, then renew at $11–$26 a month. The advertised price is a first-term teaser; the renewal is where they make it back.

RackNerd's promo tiers work differently. The official FAQ language on their specials is that they're **lifetime recurring** — you renew at the same rate for as long as you keep the service. So the honest comparison looks like this:

- **Promo 30 GB:** $10.49/year, every year. No jump at renewal.
- **Typical $3/mo competitor:** ~$36 year one, then $132–$312/year after renewal.
- **RackNerd standard monthly 30 GB:** $5.59/month ($67.08/year), no contract, cancel anytime.

The gap between RackNerd's two lines matters too. Annual promo billing gets you $10.49; paying month-to-month for the equivalent standard plan costs $67.08 over the same year — roughly six times as much. If you're confident the site will live past a few months, the annual promo tier pays for itself immediately. If you're genuinely unsure you'll keep the site running (a test project, a two-month event site), the monthly plan is the smarter buy, precisely because you can walk away.

One more math note: on the promo tiers, the 30 GB plan works out to about $0.87/month, the 85 GB to about $2.16/month, and the 200 GB to about $4.92/month. If you host more than three domains, the 85 GB tier at $24.99/year is cheaper per domain than stacking two 30 GB plans — and it bumps you from 3 TB to 10 TB of monthly transfer. 👉 [Check the 85 GB promo plan if you're hosting multiple sites](https://my.racknerd.com/aff.php?aff=11397&pid=934)

## The limits the promo pages don't lead with

Three things belong in your decision before you click buy, and none of them appear in the marketing copy.

**There is no money-back guarantee.** RackNerd's terms are explicit about this — no refund window, unlike the standard 30-day guarantees at most mainstream hosts. This is the clearest trade behind the low price. The practical workaround: if you're unsure, start on the $5.59 monthly plan instead of prepaying a year, and upgrade to the promo tier once you know you're staying.

**Resource caps are identical on every tier.** Each CloudLinux account gets 100% of one CPU core, 1 GB of physical RAM, and 80 MB/s of I/O — on the 30 GB plan and the 200 GB plan alike. Buying more storage buys you disk, bandwidth, and domains; it does not buy a faster WordPress admin or headroom for a traffic spike. A single high-traffic WooCommerce site will hit the same ceiling regardless of tier. For that workload, RackNerd's VPS line (their 1 GB KVM VPS special runs $21.99/year with dedicated resources) is the better fit.

**Promo tiers cap your domains.** Unlimited domains exist only on the standard monthly tiers and the 200 GB promo tier. The 30 GB promo stops at 3 domains (1 primary + 2 add-on), the 85 GB at 11. If your plan is "one account, many sites," read those caps before choosing.

Also worth knowing: this is shared hosting with WordPress optimization, not managed WordPress hosting. There's no one-click staging environment and no host-pushed core updates — you update WordPress yourself like on any cPanel host.

## Setting up WordPress: the actual steps

Activation is fast — orders typically provision within 5–15 minutes of checkout, and the welcome email contains your cPanel login. From there:

1. Open cPanel from the RackNerd client area.
2. Find **Softaculous Apps Installer** in the Software section and click WordPress.
3. Fill in your domain, site name, admin username, email, and password. Leave the install directory blank to put WordPress at the root.
4. Hit Install. The whole thing takes under a minute, and your dashboard lives at `yourdomain.com/wp-admin`.
5. Install the free **LiteSpeed Cache** plugin from the WordPress plugin directory. This is the step most people miss — it activates the server-level LSCache that's already running on the hosting stack, and it improves load times with zero configuration.
6. If your domain is registered elsewhere, update the nameservers to the ones in your welcome email. DNS propagation takes 1–24 hours depending on your registrar.

Already on another cPanel host? Migration is free — you open a support ticket after ordering and their team moves the site for you. That removes the usual "switching hosts is a weekend of pain" objection.

Payment at checkout covers PayPal, credit cards, crypto, and wire transfer, so it works whether or not you have a "proper" business card.

## Who should look elsewhere

Being honest about the fit saves everyone time:

- **You run one high-traffic store or a site with real spikes.** The 1 GB RAM cap per account is the binding constraint. RackNerd's KVM VPS line starts at $21.99/year for 1 GB of dedicated RAM, or step up to 2–4 GB tiers from $25.89–$39.89/year when their specials are live.
- **You want managed WordPress features** — staging sites, automatic plugin updates, a support team that fixes WordPress itself. Look at managed hosts; you'll pay more, and that's what the premium buys.
- **You might want a refund.** With no money-back guarantee, prepaying a year is a commitment. The monthly plan is the low-risk entry point.
- **You need a control panel other than cPanel.** This line is cPanel-centric by design.

## FAQ

**Does RackNerd shared hosting work for WooCommerce?** For a small or low-traffic store, yes — the LiteSpeed stack handles cached page serving well. Just know the 1 GB RAM account cap applies; a store with heavy plugins and real order volume belongs on a VPS instead.

**Is the promo price really the renewal price?** Yes. The promo annual rates are recurring at the same rate for the life of the account — $10.49 stays $10.49. That's the single biggest difference from first-term-teaser pricing elsewhere.

**Can I migrate my existing WordPress site for free?** Yes, from any cPanel-based host. Order first, then open a support ticket and the team handles the transfer.

**Which datacenter should I pick?** Whichever is closest to your visitors: Los Angeles for Asia-Pacific-friendly West Coast latency, Newark/New York for US East and Europe, Frankfurt or Strasbourg for Europe, Singapore for Southeast Asia.

## The short version before you order

One site, want the cheapest workable option, fine with paying a year up front → the **30 GB promo tier at $10.49/year**, full stop. Several sites or a media-heavy blog → the **85 GB at $24.99/year**, which is the sweet spot between the entry tier and reseller territory. Not sure you'll stick with it → **$5.59/month standard plan**, decide later. Managing client sites who each need their own login → that's a reseller hosting question, not a bigger shared plan.

Two things to check before checkout: pick the datacenter nearest your audience, and remember the no-refund policy when choosing your billing cycle. 👉 [Compare all of RackNerd's current shared hosting plans and promo pricing](https://bit.ly/RacKnerd)
