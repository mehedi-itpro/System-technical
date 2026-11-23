# 03 - Servers

Owner: ________  Last reviewed: ________

Full list: [`templates/server-inventory.csv`](../templates/server-inventory.csv).

## Hosts and virtual machines

| Name | Type | Role | OS | Site | IP | Backup | Owner |
|---|---|---|---|---|---|---|---|
| HV-01 | Physical host | Hyper-V host | Windows Server (example) | HO | 10.10.20.11 | Yes | IT |
| DC-01 | VM | Domain controller, DNS | Windows Server (example) | HO | 10.10.20.21 | Yes | IT |
| FS-01 | VM | File server | Windows Server (example) | HO | 10.10.20.31 | Yes | IT |

## Directory and identity

| Item | Value |
|---|---|
| Active Directory domain | corp.example.com (example) |
| Functional level | |
| Domain controllers | |
| Sync to Entra ID | Entra Connect on ______ / not used |
| FSMO role holders | |

## Roles and dependencies

For each important service, write what it needs to work (DNS, DHCP, a database, a licence server). When a service fails, this table tells you where to look.

| Service | Runs on | Depends on | Users affected if down |
|---|---|---|---|
| File shares | FS-01 | DC-01, DNS | Everyone |
| ERP (example) | | | |

## Patching

| Item | Value |
|---|---|
| Method | Windows Update / WSUS / other |
| Window | Day and time |
| Order | Test, then non-critical, then critical |
| Who approves | |
| Rollback | Snapshot or backup before patching |

## Hardware support

| Device | Warranty ends | Vendor contact |
|---|---|---|
| HV-01 | | |

## End of life

List servers on an operating system that is out of support, and the plan to replace them.

| Server | OS | Support ends | Plan |
|---|---|---|---|
| | | | |
