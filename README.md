# dedicated server: what Sharktech's DDoS-protected bare metal actually costs, and which plan fits your workload

A dedicated server is an entire physical machine — CPU, RAM, storage, network port — rented to you alone, with no neighbors sharing your resources. For most people searching for one right now, the real question is narrower: how much does a usable machine cost per month, and what do you actually get for it. At Sharktech, the short answer is **$99/month for the entry configuration** (16GB RAM, 30TB bandwidth, DDoS protection included), with 10Gbps unmetered builds from $305.40/month on a recurring 40% discount.

This guide walks through the current plans, what's bundled, and the terms in Sharktech's service agreement that most reviews leave out — including the fact that **all payments are non-refundable**, which changes how you should approach your first order.

> **Quick pick:** If you just need a solid dedicated server to start with, the **$99/mo Intel Xeon E3-1270v5** plan (8 threads @ 3.6GHz, 16GB RAM, 2TB HDD or 120GB SSD, 30TB bandwidth, 1Gbps uplink, Chicago or Los Angeles) is the sensible entry point — down from the regular $159/mo. If your servers get attacked regularly, the **Chicago 10Gbps unmetered** build at **$305.40/mo** (40% off recurring) is the one built for that. Every plan ships with free setup and always-on DDoS filtering up to 60Gbps. 👉 [See Sharktech's current dedicated server pricing and stock](https://portal.sharktech.net/aff.php?aff=1626&url=https%3A%2F%2Fsharktech.net%2Fdedicated-servers%2F)

## What a dedicated server is — and when it beats a VPS

A dedicated server gives you exclusive use of one physical machine in a provider's data center. A VPS gives you a virtual slice of a shared machine. The VPS route is cheaper and scales instantly, but your CPU time and disk I/O are contested by whatever else lives on that hardware.

You need the dedicated option when three things are true: your workload is CPU- or disk-I/O-heavy (databases, game servers, virtualization hosts, parallel compute), you need predictable performance rather than burst performance, and you're comfortable managing the OS yourself. Hosting providers like Sharktech provision the whole machine and the network around it; what you run on it is your call — including installing Proxmox or another hypervisor and splitting the box into your own VMs.

One more scenario worth naming: if your servers attract DDoS traffic, shared environments often get you null-routed the moment an attack starts. This is exactly where Sharktech has specialized since 2003, and it's the main reason to pick them over a generic host.

## Sharktech dedicated server plans and current prices

Sharktech sells configurable bare-metal servers alongside a set of fixed promotional configurations. Here's what's currently listed on the official promo and product pages:

| Plan | CPU / RAM | Storage | Network | Price | Order |
| --- | --- | --- | --- | --- | --- |
| E3-1270v5 promo (Chicago or LA) | 8 threads @ 3.6GHz / 16GB | 2TB HDD or 120GB SSD | 1Gbps, 30TB/mo | ~~$159~~ **$99/mo** | [Order the $99/mo plan](https://portal.sharktech.net/aff.php?aff=1626&url=https%3A%2F%2Fsecure.sharktech.net%2Fhelpdesk%2Fcart.php%3Fa%3Dadd%26pid%3D470%26promocode%3Dv5LACHI) |
| LA NVMe build | Dual Xeon E5-2670v2 / 64GB | 1TB NVMe | 1Gbps unmetered | **$129/mo** | [Order the $129/mo LA server](https://portal.sharktech.net/aff.php?aff=1626&url=https%3A%2F%2Fsecure.sharktech.net%2Fhelpdesk%2Fcart.php%3Fa%3Dadd%26pid%3D606) |
| Dual E5-2637v2 (Chicago, Denver or LA) | 16 threads @ 3.5GHz / 32GB | 2TB HDD or 120GB SSD | 1Gbps, 30TB/mo | **$183.20/mo** | [Order the $183.20/mo build](https://portal.sharktech.net/aff.php?aff=1626&url=https%3A%2F%2Fsecure.sharktech.net%2Fhelpdesk%2Fcart.php%3Fa%3Dadd%26pid%3D473%26promocode%3DNew2637v2) |
| Dual E5-2670 unmetered (4 locations) | 32 threads @ 2.6GHz / 32GB | 2TB HDD or 120GB SSD | 1Gbps unmetered | **$159–$189/mo** by city | [Order the Amsterdam build at $159/mo](https://portal.sharktech.net/aff.php?aff=1626&url=https%3A%2F%2Fsecure.sharktech.net%2Fhelpdesk%2Fcart.php%3Fa%3Dadd%26pid%3D437%26promocode%3DE51Gams) |
| 10Gbps unmetered (Chicago) | E3-1270v2 @ 3.5GHz / 16GB | 2TB HDD or 240GB SSD | 10Gbps unmetered | ~~$509~~ **$305.40/mo** | [Order the $305.40/mo 10Gbps server](https://portal.sharktech.net/aff.php?aff=1626&url=https%3A%2F%2Fsecure.sharktech.net%2Fhelpdesk%2Fcart.php%3Fa%3Dadd%26pid%3D492%26promocode%3D10GbpsCHI) |
| Custom bare-metal catalog | Your spec | 2TB NVMe M.2 base | 10Gbps, 300TB/mo | from **$219/mo** | [Browse the bare-metal catalog](https://portal.sharktech.net/aff.php?aff=1626&url=https%3A%2F%2Fsharktech.net%2Fdedicated-servers%2F) |

A few details that don't fit in the table:

- **The Dual E5-2670 unmetered line is priced by city:** Amsterdam $159/mo, Chicago $169/mo (coupon `E51Gchi`), Los Angeles and Denver $189/mo. Same hardware everywhere — so if location doesn't matter to you, Amsterdam is $30/month cheaper than LA.
- **The promo discounts are recurring, not first-month teasers.** The $99 rate and the 40%-off Chicago 10Gbps rate apply as long as you keep the server, per Sharktech's own promo announcement. That makes the real first-year cost of the entry plan **$1,188**, versus $1,908 at the regular rate.
- The 10Gbps discount in Los Angeles is shallower: 20% off recurring (`10GbpsLA`), bringing that build to $631.20/mo. Chicago is the value pick for 10Gbps by a wide margin.
- Sharktech officially suggests the Dual E5-2637v2 build for Minecraft servers — 16 fast threads at 3.5GHz is a sensible fit for that workload.
- Spot configurations on the 10Gbps catalog page currently run **$189–$329/mo** depending on drive count (1x vs 4x M.2), all with free setup.

## What's included with every plan

Every Sharktech server comes with the same baseline, which is worth knowing before you compare raw prices:

- **DDoS protection up to 60Gbps, always on.** Filtering happens automatically at the network edge for all attack types within that range, at no extra cost. You can upgrade to cloud-based protection up to **100Gbps** if you need more headroom.
- **Free setup** on all listed servers — no activation fee hiding at checkout.
- **/29 IPv4 (5 usable IPs)** on the promotional plans, plus free IPv6 allocation (you select it on the order form).
- The **Sharktech SECURE management platform** and a bare-metal management panel for hardware-level control.
- **24/7/365 human support** and a **99.99% uptime** guarantee.
- On the bare-metal catalog line specifically: a **10Gbps port and 300TB/month of bandwidth** included from day one, with 2TB NVMe M.2 as the starting storage.

One thing to plan around: Sharktech's 10Gbps page currently states that due to component shortages and high demand, the usual 24-hour deployment target **can't be guaranteed right now**. Stock systems ship fastest; custom CPU/memory/drive builds take longer, and the sales team sets the expectation before you commit. Custom builds generally arrive within 1–2 weeks. If you're on a deadline, order the stock configuration.

## The fine print most reviews skip

Sharktech's Terms of Service contain several clauses that directly affect how you should buy, and they rarely make it into comparison articles:

1. **All payments are non-refundable.** The terms state this twice in bold, covering setup fees and monthly fees alike, whether or not you used the service. There's no trial and no money-back window. The practical consequence: start with a monthly term, not a long prepay.
2. **Servers are unmanaged.** Sharktech guarantees the machine is online and remotely reachable. Application-level problems — your web server config, your game panel, your scripts — are yours to fix. This is a provider for people who can run their own box.
3. **Fees add up if billing slips.** A declined card costs $1.00, accounts 4 days past due get interrupted, reconnection after non-payment is $50, late accounts carry a $25 fee, and chargebacks that Sharktech contest successfully trigger a $50–$150 administrative fee.
4. **Cancellation requires at least 7 days' notice** by email with your full account details — don't assume canceling on the due date works.
5. Billing disputes must be raised within **30 days** of the charge.

None of this is unusual for the dedicated server market, where non-refundable terms and unmanaged machines are the norm. But it means the "start cheap, test, escalate" approach should be done one monthly cycle at a time.

## Real-world performance and reputation

HostAdvice's expert review gives Sharktech a **9.3/10 overall** (pricing 9.2, features 9.6, support 9.3), based on a hands-on test of a 256GB RAM machine with 2TB NVMe storage. Their measured numbers: disk reads at **4.2 GB/s**, writes at **1.0 GB/s**, and sysbench CPU results of 479 events per second with ~2ms average latency. Those figures are the reviewer's own tests, so treat them as indicative rather than a guarantee for every configuration.

On the DDoS side — the reason most customers end up here — the official testimonial from Dingdian Network, a game server operator, describes attacks "ranging from 3Gbit to 8Gbit" hitting their servers, which "never skip a beat." That's a brand-published quote, so weigh it accordingly, but the pattern is consistent: filtering up to 60Gbps is on by default, and smaller volumetric attacks never reach your port in the first place.

Payment options are broader than most US hosts offer: credit card, PayPal, wire transfer, Western Union, and Alipay.

## Who shouldn't buy a dedicated server here

Honest limits, based on what's verified above:

- **If you need hourly or on-demand billing**, this isn't the fit. Sharktech has no per-hour plans; you're renting by the month. For short-lived or license-compliance workloads, cloud providers like AWS offer dedicated hosts billed by the hour instead.
- **If you can't manage a Linux/BSD/Windows server yourself**, the unmanaged support model will frustrate you. A managed VPS or a managed hosting plan serves beginners better.
- **If your workload is light**, a $99/month machine is overkill. A VPS at a fraction of the price handles most websites fine. Dedicated servers earn their cost through I/O, CPU guarantees, and attack resilience.
- **If you might need your money back**, remember the no-refund policy. Commit month by month until you're sure.

## How to order (and where the coupon goes)

The ordering flow is straightforward:

1. Pick a plan from the table above — the order links go straight to the pre-configured cart for that machine.
2. The promotional coupons (`v5LACHI`, `New2637v2`, `E51Gams`, `10GbpsCHI`, and the city variants) are already embedded in the cart links, so the discounted price should appear before you pay. **Check the line total in the cart matches the advertised price before entering payment** — that's the single easiest way to avoid a billing surprise on a non-refundable service.
3. On the order form, choose your data center location where the plan offers several, and tick the free IPv6 allocation if you want it.
4. Stock machines are targeted for 24-hour deployment; remember the current shortage caveat and allow extra time.

## FAQ

**Dedicated server vs VPS — which do I actually need?**
If you need guaranteed CPU, heavy disk I/O, custom virtualization, or frequent DDoS exposure, a dedicated server. If your site or app runs comfortably on shared resources and you value instant scaling, a VPS is cheaper and easier.

**Can I run Proxmox or my own VMs on a Sharktech server?**
Yes. The machine is fully yours, and the bare-metal management panel gives you hardware-level access. Installing and operating the hypervisor is your responsibility under the unmanaged support model.

**Does Sharktech offer refunds or a trial?**
No. All payments, including setup fees, are non-refundable under any circumstances, per the Terms of Service. Billing disputes must be raised within 30 days.

**Where are the data centers?**
Five locations: Los Angeles, Las Vegas, Denver, Chicago, and Amsterdam. Not every configuration is stocked in every city, which is why the same hardware can cost $30/month more or less depending on location.

## The bottom line, by scenario

Running game servers or anything that attracts attacks: go 10Gbps unmetered in Chicago at $305.40/mo, or the Dual E5-2637v2 at $183.20/mo if your traffic profile fits 1Gbps. Need fast storage on a budget: the $129/mo Los Angeles build with 1TB NVMe and 64GB RAM is the standout. Everyone else starting out: the $99/mo E3-1270v5 plan, month to month, no long commitment — you can always upgrade later, and Sharktech assists with migrations between plans.

Before you pay, reconfirm two things in the cart: the discounted total matches the advertised price, and you're okay with the no-refund terms at a monthly cadence. 👉 [Check Sharktech's current stock, prices, and DDoS-protected plans](https://portal.sharktech.net/aff.php?aff=1626&url=https%3A%2F%2Fsharktech.net%2Fdedicated-servers%2F)
