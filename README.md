# VPS pricing: what JustHost's $1.99 plan actually costs, when the 12-month rate pays off, and which tier to pick (full plan table)

JustHost's VPS pricing starts at **$1.99/mo** for 1 core, 512 MB of RAM and 5 GB of NVMe storage. Three things sit behind that figure. An IPv4 address costs **$3.31/mo** on top and IPv6 is the free option, the port on that plan is a 10 Mbps fair-share port, and every lower per-month rate on the page is conditional on paying 12 months up front. Add IPv4 and the $1.99 plan is a $5.30/mo server.

What follows is the full lineup at the rates JustHost publishes, what monthly and 12-month payment each work out to over a year, the three places where a neighbouring tier is the better buy, and the workloads where a different provider is cheaper.

> **Quick pick:** Double Star at **$5.67/mo** when you pay 12 months (2 cores, 2 GB RAM, 20 GB NVMe, 200 Mbps) covers a small site, a database and two or three containers. If you only need a shell, a tunnel endpoint or IPv6-only services, VPS Promo at $1.99/mo is enough. 👉 [Check JustHost's current VPS plans and rates](https://justhost.asia/en/services/vps/tariffs-all?ref=196392)

## JustHost VPS plans and prices

| Plan | vCPU / RAM | NVMe / fair-share port | Price (monthly → 12-month) | Order |
| --- | --- | --- | --- | --- |
| VPS Promo | 1 core / 512 MB | 5 GB / 10 Mbps | **$1.99/mo** (no 12-month rate shown) | [Order](https://justhost.asia/en/services/vps/tariffs/promo-c1r512nvme?ref=196392) |
| New Star | 1 core / 1 GB | 10 GB / 100 Mbps | $3.81/mo → **$3.05/mo** | [Order](https://justhost.asia/en/services/vps/tariffs/new-star-c1r1024nvme?ref=196392) |
| Sirius | 1 core / 1 GB | 20 GB / 300 Mbps | $4.85/mo → **$3.88/mo** | [Order](https://justhost.asia/en/services/vps/tariffs/sirius?ref=196392) |
| Arcturus | 1 core / 2 GB | 30 GB / 300 Mbps | $6.92/mo → **$5.53/mo** | [Order](https://justhost.asia/en/services/vps/tariffs/arcturus?ref=196392) |
| Double Star | 2 cores / 2 GB | 20 GB / 200 Mbps | $7.08/mo → **$5.67/mo** | [Order](https://justhost.asia/en/services/vps/tariffs/double-star-c2r2048nvme?ref=196392) |
| Alpha Centauri | 2 cores / 2 GB | 40 GB / 400 Mbps | $8.99/mo → **$7.19/mo** | [Order](https://justhost.asia/en/services/vps/tariffs/alpha_centauri?ref=196392) |
| Bright Star | 4 cores / 4 GB | 30 GB / 300 Mbps | $9.80/mo → **$7.84/mo** | [Order](https://justhost.asia/en/services/vps/tariffs/bright-star-c4r4096nvme?ref=196392) |
| Vega | 2 cores / 4 GB | 80 GB / 500 Mbps | $13.44/mo → **$10.75/mo** | [Order](https://justhost.asia/en/services/vps/tariffs/vega?ref=196392) |
| Capella | 4 cores / 4 GB | 120 GB / 750 Mbps | $18.30/mo → **$14.64/mo** | [Order](https://justhost.asia/en/services/vps/tariffs/capella?ref=196392) |

Two larger tiers sit above Capella. Rigel runs 4 cores, 8 GB RAM and 200 GB of NVMe; Aldebaran runs 8 cores, 32 GB RAM, 700 GB and a 750 Mbps port. I could not confirm their current rates, so pull the numbers from the plan pages before you budget for one. JustHost also lists a separate NVMe plan called Azha that doesn't appear in the main price list.

The three "Star" entry plans (New Star, Double Star, Bright Star) carry a minimum order of 3 months. The constellation-named plans have no such note.

## What the $1.99 headline leaves out

The only add-on that changes the effective monthly price of the cheap plans is IPv4. JustHost gives every VPS a free IPv6 address and prices a dedicated IPv4 at **$3.31/mo**. On the $1.99 plan that's a 166% increase; on Capella it's 18%. If your workload can live on IPv6 (a monitoring node, a backup target, an internal service behind a CDN), the promo plan stays at $1.99. If you need a v4 address for mail, game traffic or client access, budget for it from the start.

Traffic is unmetered but not uncapped. The plan cards pair each port speed with an equivalent monthly volume: 10 Mbps works out to 4+ TB, 100 Mbps to 31+ TB, 500 Mbps to 155+ TB and 750 Mbps to 232+ TB. That's how an "unmetered" VPS is usually built: no transfer counter, but a port ceiling, with a fair-share clause behind it. You can buy more port speed at **$2.50/mo per extra 10 Mbps**, and a dedicated 1 Gbps port is listed at $333.33/mo, which tells you the shared ports are the intended option for normal use.

Everything else that matters is included rather than billed: KVM virtualization, built-in DDoS filtering, free migration from another host, SSH access, and the ability to add CPU, RAM or disk without moving the server. Human sysadmin work is the exception at **$9.16/hour**. 👉 [See what the $1.99 plan bundles](https://justhost.asia/en/services/vps/tariffs/promo-c1r512nvme?ref=196392)

## Monthly vs 12 months: the actual difference

The 12-month rate is a flat 20% off the monthly rate on every plan that shows one. Here's what that is in dollars.

| Plan | Monthly × 12 | 12-month rate × 12 | Saved |
| --- | --- | --- | --- |
| Arcturus | $83.04 | $66.36 | $16.68 |
| Double Star | $84.96 | $68.04 | $16.92 |
| Vega | $161.28 | $129.00 | $32.28 |
| Capella | $219.60 | $175.68 | $43.92 |

A year of Double Star prepaid costs $68.04, less than six months of Liquid Web's cheapest VPS. The saving is real but small in absolute terms, which makes the decision easy: if you're keeping the server for three months or more, take the 12-month rate. If you're testing an app for a fortnight, pay monthly and keep the flexibility.

One caveat before you prepay. The price list shows a monthly rate and a discounted 12-month rate; it does not publish a separate renewal figure for the term after that. Ask support what the rate reverts to when your 12 months end, and get the refund terms in writing at the same time, because the pricing page doesn't state a refund window. 👉 [Start with the Double Star plan page](https://justhost.asia/en/services/vps/tariffs/double-star-c2r2048nvme?ref=196392)

## Where a neighbouring tier beats the obvious choice

Plan tables reward a second look, because two adjacent rows often differ in ways that matter more than the price gap.

**Sirius vs New Star.** New Star is $3.81 and Sirius is $4.85 for the same 1 GB of RAM. The extra $1.04 buys double the disk (20 GB vs 10 GB) and triple the port speed (300 Mbps vs 100 Mbps). Ten gigabytes disappears fast once you add a database and logs, so Sirius is the better buy for almost everyone who was looking at New Star.

**Arcturus vs Double Star.** Both have 2 GB of RAM and both land near $7/mo: Arcturus at $6.92 with 1 core, 30 GB and 300 Mbps; Double Star at $7.08 with 2 cores, 20 GB and 200 Mbps. Arcturus is cheaper and gives you more disk and bandwidth; Double Star gives you a second core. Take Arcturus for a content site or a file-serving job, Double Star if you're running something that benefits from parallel workers.

**Vega vs Bright Star.** Bright Star is $9.80 for 4 cores, 4 GB and 30 GB of disk. Vega is $13.44 for 2 cores, 4 GB and 80 GB with a 500 Mbps port. If your bottleneck is compilation, image processing or many small concurrent requests, Bright Star saves you $3.64/mo. If it's storage, media delivery or backups, Vega's extra 50 GB and 200 Mbps are worth more than the two cores you give up.

The order I'd rank resources in for typical small-project work: RAM first, then disk, then port speed, then core count. Core count only moves to the front for CPU-bound jobs.

## Who should not buy a JustHost VPS

JustHost sells unmanaged KVM servers with paid sysadmin time. If you want someone else to own the operating system, the $9.16/hour rate is the number to weigh against a host that bundles management. Liquid Web's cheapest Cloud VPS is $11/mo for 1 vCPU, 2 GB RAM, 60 GB of storage and 2 TB of bandwidth, and its VPS line is built around managed support rather than raw specs per dollar.

If you need a lot of RAM cheaply, Contabo's Core VPS starts at 8 GB and runs to 96 GB with up to 18 vCPU and 100–600 GB of SSD or 50–300 GB of NVMe. Its advertised entry figure of €4.40/month is a 24-month, tax-inclusive equivalent, roughly €105.60 across the term, and its "unlimited traffic" is subject to a fair-use policy that allows throttling. JustHost's comparable 8 GB tier is Rigel, so price the two against each other before assuming either wins.

If you want a control panel and tooling rather than a bare server, Hostinger's KVM 1 is $6.49/mo on a 24-month prepay ($155.76 up front) and renews at $11.99/mo on the same term, with cPanel, Plesk, CyberPanel and DirectAdmin supported plus a public API and AI-assisted server management. That renewal step from $6.49 to $11.99 is the thing to model before committing two years.

| Provider | Entry rate | What that number actually is |
| --- | --- | --- |
| JustHost | $1.99/mo | Monthly rate, 1 core / 512 MB / 5 GB, 10 Mbps port; IPv4 +$3.31/mo |
| Liquid Web | $11/mo | Monthly list price, 1 vCPU / 2 GB / 60 GB / 2 TB |
| Hostinger | $6.49/mo | 24-month prepay average; $155.76 today, renews at $11.99/mo |
| Contabo | €4.40/mo | 24-month subscription, tax-inclusive equivalent (≈€105.60 total) |

These four numbers are not the same kind of number, and treating them as one market price is how people end up disappointed at checkout.

## FAQ

**Is the traffic really unlimited?**
It's unmetered with a port ceiling and a fair-share rule. The cheapest plan's 10 Mbps port is about 4 TB a month, Capella's 750 Mbps port about 232 TB. Nothing counts your gigabytes, but sustained saturation of a shared port is what the fair-share clause exists for.

**Do I have to pay for IPv4?**
Only if you need it. IPv6 is free on every plan; IPv4 is $3.31/mo. On VPS Promo that's the difference between $23.88 and $63.60 a year.

**Can I change plan or datacenter later?**
JustHost says you can add CPU, RAM or disk without migrating the server, and switch location from the client area. Locations listed include seven US cities (Atlanta, Chicago, Dallas, Los Angeles, New York, San Jose, Seattle), London, Brussels, Kyiv, Istanbul, Singapore, the UAE, Switzerland and Sweden, across 41 countries.

**Is the 512 MB plan usable?**
For a shell, a DNS secondary, a WireGuard endpoint or a monitoring agent, yes. A 512 MB box won't run a modern database alongside a web app, and 5 GB of disk leaves little room once the OS is installed.

**Which plan should a single small website use?**
Arcturus at $6.92/mo, or $5.53/mo on the 12-month rate. One core and 2 GB handles a typical CMS with a small database, and 30 GB of disk absorbs logs and backups for a while.

## Final selection rules

- Shell access, IPv6-only service, tunnel endpoint: **VPS Promo, $1.99/mo**.
- One small site with IPv4, database included: **Arcturus, $5.53/mo** on 12 months, or Sirius at $3.88/mo if 10 GB less disk is fine.
- Two to four containers or a busier app: **Double Star, $5.67/mo**, and step up to Alpha Centauri at $7.19/mo when 20 GB of disk isn't enough.
- Storage or media heavy: **Vega, $10.75/mo**, or Capella at $14.64/mo for the 750 Mbps port.
- 8 GB of RAM and up: Rigel or Aldebaran, priced against Contabo's 8 GB entry tier before you decide.

Four things to confirm in the order form before you pay: whether you need IPv4 and the extra $3.31, whether the 12-month rate is available on the term you're choosing, what the rate becomes after that term ends, and what the refund and cancellation terms are. Those four answers change the real cost more than the difference between any two adjacent rows in the table.

👉 [See JustHost's current VPS pricing, locations and plan details](https://justhost.asia/?ref=196392)
