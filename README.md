# System Technical Documentation Kit

Templates for documenting a company's IT systems: network, servers, Microsoft 365, Azure, endpoints, security, backup and telephony. Fill them in once, keep them current, and anyone on the team (or a new hire, or an auditor) can understand the environment without asking the one person who built it.

## Why

Most small IT teams know their systems well but have them written down badly or not at all. Then the one person goes on leave and nobody knows which router is at which site, who owns the Azure subscription, or how the phone system is wired.

This kit gives you a standard set of documents and registers to fix that.

## Important: keep real data private

This repo contains **templates and example values only**. All IPs, names and numbers here are made up.

When you document a real company:

1. Copy this kit into a **private** repository or an internal wiki.
2. Never store passwords, keys, recovery codes or tokens in it. Store them in a password vault and write only where they are kept.
3. Treat the filled-in version as confidential. It is a map of your network.

## What is inside

| File | Covers |
|---|---|
| [docs/01-environment-overview.md](docs/01-environment-overview.md) | Company, sites, users, owners, contacts |
| [docs/02-network.md](docs/02-network.md) | Sites, links, IP plan, routers and firewalls, DNS, DHCP, Wi-Fi, VPN |
| [docs/03-servers.md](docs/03-servers.md) | Servers and virtual machines, roles, patching |
| [docs/04-microsoft-365-and-entra.md](docs/04-microsoft-365-and-entra.md) | Tenant, domains, licences, admin roles, Conditional Access, mail |
| [docs/05-azure.md](docs/05-azure.md) | Subscriptions, resource groups, naming, networking, cost |
| [docs/06-endpoints.md](docs/06-endpoints.md) | PCs, standard image, management, software |
| [docs/07-security-and-backup.md](docs/07-security-and-backup.md) | Accounts, MFA, logging, backup, recovery, incidents |
| [docs/08-telephony.md](docs/08-telephony.md) | IP PABX, extensions, trunks, intercom |
| [docs/09-change-log.md](docs/09-change-log.md) | Review routine and change log |
| [templates/](templates/) | CSV registers: assets, IP plan, servers, licences |

## How to use it

1. Start with the overview, then the network. These are what people need most in an outage.
2. Fill every table. Write `n/a` instead of leaving a blank, so a gap is a decision and not an oversight.
3. Put a **last reviewed** date and an **owner** on every document.
4. Review every quarter, and update the document in the same sitting as any change.
5. Link to other repos or runbooks instead of copying them. For example, endpoint management details can point to [intune-endpoint-management](https://github.com/mehedi-itpro/intune-endpoint-management).

## Style rules

- Write for someone who has never seen the system.
- Use tables for facts, short sentences for reasons.
- Record **why** a decision was made, not only what was done.
- Diagrams: use Mermaid so they live in the repo and can be edited.

## বাংলায় সংক্ষেপে

কোম্পানির IT সিস্টেমের (network, server, Microsoft 365, Azure, PC, security, backup, টেলিফোন) ডকুমেন্টেশনের জন্য ফাঁকা টেমপ্লেট। সত্যিকারের তথ্য ভরার সময় অবশ্যই প্রাইভেট রিপো বা অভ্যন্তরীণ উইকি ব্যবহার করুন। পাসওয়ার্ড কখনো লিখবেন না, শুধু লিখবেন কোথায় রাখা আছে।

## Author

Mehedi, enterprise IT infrastructure, Dhaka, Bangladesh.

## License

[MIT](LICENSE)
