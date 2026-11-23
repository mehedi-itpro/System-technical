# 04 - Microsoft 365 and Entra ID

Owner: ________  Last reviewed: ________

## Tenant

| Item | Value |
|---|---|
| Tenant name | example.onmicrosoft.com |
| Tenant ID | Keep it out of public repos |
| Primary domain | example.com |
| Other domains | |
| Region | |
| Technical contact | |

## Licences

Full list: [`templates/license-inventory.csv`](../templates/license-inventory.csv).

| Licence | Bought | Assigned | Used for |
|---|---|---|---|
| Microsoft 365 Business Premium (example) | 100 | 96 | Staff |
| Exchange Online only (example) | 20 | 18 | Shared and site mailboxes |

## Admin accounts

Names and roles only. No passwords.

| Account | Role | MFA | Notes |
|---|---|---|---|
| admin.name@ (example) | Global Administrator | Yes, phishing-resistant | Daily admin |
| Break-glass 1 | Global Administrator | Offline key | Excluded from Conditional Access, sign-in alerts on |
| Break-glass 2 | Global Administrator | Offline key | Same |

Rules: at most five Global Administrators, separate admin and daily accounts, review the list every quarter.

## Conditional Access

| Policy | Applies to | Requirement | State |
|---|---|---|---|
| Require MFA for all users (example) | All users | MFA | On |
| Require compliant device (example) | All users, Windows | Compliant device | Report-only |
| Block legacy authentication (example) | All users | Block | On |

## Email

| Item | Value |
|---|---|
| MX | Points to Microsoft 365 |
| SPF | Record in place, yes or no |
| DKIM | Enabled for the primary domain, yes or no |
| DMARC | Policy: none / quarantine / reject |
| Shared mailboxes | |
| Mail flow rules | |
| External forwarding | Blocked or allowed, and why |

## Collaboration

| Item | Value |
|---|---|
| SharePoint sites | |
| Teams policy | |
| External sharing | |
| OneDrive Known Folder Move | On or off |

## Groups and naming

How groups, mailboxes and sites are named, and who may create new ones.

## Joiner, mover, leaver

| Step | Who | Where it is written down |
|---|---|---|
| New user: account, licence, groups, PC | | |
| Role change | | |
| Leaver: block sign-in, revoke sessions, convert mailbox, wipe device | | |
