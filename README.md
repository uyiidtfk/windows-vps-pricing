# Windows VPS Server: What Should It Cost, Which Plan Is Enough, and What Does Year Two Look Like?

A Windows VPS starts at roughly $8.50 a month in the mainstream market. OVHcloud's VPS-2 gives you 4 vCores, 8 GB RAM and 75 GB NVMe for that; Atlantic.Net starts its Windows range at $15.00 a month; Contabo prices CLOUD VPS 4 at €5.50 a month, discounted to €4.40 for the first 24 months. The same host sells Linux from $4 a month, and that gap is Microsoft licensing built into the Windows price rather than better hardware.

Three things decide whether you end up paying $100 or $500 a year: the RAM and vCPU tier you actually need, whether the advertised price survives month 25, and the add-ons that appear after checkout. All three are covered below, with the numbers each provider currently publishes.

## The short answer on sizing

- **Remote desktop for one or two people, a small .NET site, or a Windows-only desktop app** → the smallest plan with 4 GB RAM and 2 vCores. Fasthosts VPS 2 (2 vCPU / 4 GB / 120 GB NVMe) is the shape of that tier.
- **SQL Server Express, several sites, or a small team on RDP** → 8 GB RAM and 4 vCores on NVMe. OVHcloud VPS-2 and Contabo CLOUD VPS 4 sit here.
- **7×24 trading, ERP, or anything with a paid backup requirement** → 16 GB RAM upward, and budget for a backup add-on. Contabo CLOUD VPS 16 and OVHcloud VPS-4 are the reference points.

Windows entry plans across the market start at 4 GB, not 1 GB: Fasthosts' cheapest Windows VPS has 4 GB, IONOS's Windows L+ has 8 GB, OVHcloud's VPS-2 has 8 GB. That is the practical floor once the OS itself takes its share of memory.

👉 [Check AVA Hosting's current Windows VPS plans against these thresholds](https://my.ava.hosting/aff.php?aff=15562)

## What the market looks like right now

Every figure below comes from the provider's own product page, in the currency that page quotes. Plan names change and so do promo windows, so confirm on the order page before you pay.

| Provider and plan | vCPU · RAM · storage | Windows versions offered | Price and term |
| --- | --- | --- | --- |
| Contabo CLOUD VPS 4 | 4 vCPU / 8 GB / 100 GB SSD | 2016, 2019, 2022, 2025 | €5.50/mo list; €4.40/mo for the first 24 months |
| Contabo CLOUD VPS 8 | 8 vCPU / 24 GB / 300 GB SSD or 150 GB NVMe | 2016, 2019, 2022, 2025 | €14.00/mo list; €11.20/mo for the first 24 months |
| Contabo CLOUD VPS 16 | 16 vCPU / 64 GB / 500 GB SSD or 250 GB NVMe | 2016, 2019, 2022, 2025 | €37.00/mo list; €29.60/mo for the first 24 months |
| OVHcloud VPS-2 | 4 vCores / 8 GB / 75 GB NVMe | Windows Server, pre-installed | from $8.50/mo |
| OVHcloud VPS-3 | 6 vCores / 12 GB / 100 GB NVMe | Windows Server, pre-installed | from $12.32/mo |
| OVHcloud VPS-4 | 8 vCores / 24 GB / 200 GB NVMe | Windows Server, pre-installed | from $23.37/mo |
| Fasthosts VPS 2 | 2 vCPU / 4 GB / 120 GB NVMe | 2016, 2019, 2022, 2025 | £22/mo list; £14/mo for 3 months |
| Fasthosts VPS 4 | 4 vCPU / 8 GB / 240 GB NVMe | 2016, 2019, 2022, 2025 | £42/mo list; £27/mo for 3 months |
| Fasthosts VPS 8 | 8 vCPU / 16 GB / 480 GB NVMe | 2016, 2019, 2022, 2025 | £78/mo list; £52/mo for 3 months |
| Atlantic.Net Windows VPS | varies by plan tier | 2008 R2 SP1 through 2025, Datacenter, with or without Desktop Experience | from $15.00/mo |

Two things stand out in that table. Windows Server 2025 is now on the menu at every host that lists versions, and NVMe has replaced SATA SSD as the default on new plans. If a provider you are considering still sells Windows Server 2016 as its headline image, it is not necessarily a problem, but you should be choosing 2022 or 2025 unless an application pins you to an older release.

## The first price is not the price

Contabo's plan page labels its discounts "for the first 24 months." Fasthosts labels its £14 "for 3 months." Both are real discounts, and both expire.

Run the arithmetic on Fasthosts VPS 2. Three months at £14 is £42. The remaining nine months of year one at the £22 list price cost £198. Year one totals £240, not the £168 you get if you multiply £14 by 12. Over two years it is £504. That is a 50% difference between the advertised number and reality, on the very first plan in the range.

Contabo's discount is longer and gentler but still ends. CLOUD VPS 4 at €4.40 for 24 months costs €105.60, then reverts to €5.50. A 36-month total is €105.60 plus 12 × €5.50, so €171.60. Budget €4.40 across all three years and you come up €13.20 short.

The habit worth building: convert any Windows VPS offer to a 36-month total at list price before you compare it to anything. Then check the same plan at month 25. A host that shows you the renewal price up front is telling you something useful about how it treats customers.

## What the sticker price leaves out

Atlantic.Net publishes its extras, which makes it a good example of what to look for elsewhere. One IPv4 is included; each additional one costs $3.65 a month, or $43.80 a year. Inbound traffic is unmetered, but outbound beyond the free allowance is $0.02 per GB. Optional daily backups cost 20% of the server price, with a $1.00 monthly minimum.

OVHcloud includes a daily backup of the previous 24 hours but charges for Premium backup and snapshots. Its unlimited traffic also excludes datacentres in Asia-Pacific, which matters if your users are there. Fasthosts includes one IPv4 and free IPv6, then sells Cyber Protect and Plesk Web Host Edition (the latter at £5 a month) as add-ons. Contabo includes one to three snapshots depending on the plan and sells Auto Backup separately.

A $15 Windows VPS with a second IP and daily backups is closer to $22 a month. That is still cheap, but it is the number you should be comparing against other providers, not the headline.

👉 [See what AVA Hosting bundles into its Windows VPS plans before you add extras](https://my.ava.hosting/aff.php?aff=15562)

## Windows is usually a one-way door

IONOS states plainly that if you pick Windows on a VPS+, you cannot switch it to Linux later; you have to place a new order. That is not unique to IONOS. Rebuilding a server from one OS family to another usually means reprovisioning, and some hosts bill it as a new contract.

Region availability has the same trap. OVHcloud's Local Zones do not offer Windows at all, along with preinstalled apps, additional storage, monitoring, Additional IP, load balancers and managed databases. If you pick a Local Zone for latency reasons and assume you can add Windows there, you will find out at checkout.

Access is the other thing people discover late. Windows VPS is reached over RDP using the IP, username and password the host issues; Linux boxes use SSH. If your office firewall blocks outbound RDP, or you need to restrict RDP to specific source IPs, sort that out before you migrate anything. Atlantic.Net's Datacenter images come with and without Desktop Experience, and the version without it has a smaller footprint but no full graphical desktop, which is fine for a service host and wrong for a machine you plan to drive by mouse.

👉 [Compare AVA Hosting's Windows VPS options and confirm the OS and region before ordering](https://my.ava.hosting/aff.php?aff=15562)

## The first hour after delivery

At these prices every host in this article is unmanaged. You get root or administrator access and a working network, and everything above that is yours. Contabo's own setup guide reads like a to-do list for the first hour, and it transfers to any provider:

1. Run Windows Update and reboot when prompted.
2. Restrict RDP access to trusted IPs, or put it behind a VPN, at the firewall.
3. Use strong, unique passwords for every component you install.
4. Remove unused roles and services and apply the latest security patches.
5. Install the components you actually need (IIS, .NET, SQL Server) and configure DNS if you are hosting sites.
6. Set up backups and basic monitoring so you can see a failure and recover from it.

Step 2 is the one people skip. An RDP port open to the internet with a weak password is the most common way a cheap Windows VPS turns into someone else's crypto miner.

## Which version, and how much RAM

Windows Server 2022 or 2025 unless a line-of-business app demands otherwise. Contabo and Fasthosts both list 2016 through 2025, Atlantic.Net goes back to 2008 R2 SP1, and OVHcloud does not enumerate versions on its Windows VPS page, so ask before ordering if you need a specific build.

On memory, the market has already answered for you. Windows plans start at 4 GB at Fasthosts, 8 GB at OVHcloud and IONOS. If you are running SQL Server alongside a web app, treat 8 GB as the working floor and move to 16 GB before you start tuning. Storage type matters more than capacity for database workloads: NVMe plans at OVHcloud and Fasthosts will feel different from SATA SSD at the same size.

## How to decide

- **One person on RDP, or a single small .NET site** → the cheapest 4 GB Windows plan you can find. Paying for 16 GB here buys nothing.
- **SQL Server Express, two or three sites, a small support team** → 8 GB RAM, 4 vCores, NVMe. This is the tier most buyers land on.
- **Trading terminal, ERP, or a system that must stay up** → 16 GB and up, plus a paid backup add-on and a documented restore test.

Before you pay, confirm two things: the price at month 4 or month 25, whichever the promo ends at, and whether you can change the OS or add an IP later without reordering. Those two answers separate a plan that fits from one you will be migrating away from in six months.

👉 [Start with AVA Hosting's Windows VPS lineup and check the renewal terms before checkout](https://my.ava.hosting/aff.php?aff=15562)
