# 06 - Endpoints

Owner: ________  Last reviewed: ________

Full asset list: [`templates/asset-inventory.csv`](../templates/asset-inventory.csv).

## Fleet summary

| Item | Value |
|---|---|
| PCs and laptops | 150 (example) |
| Operating system | Windows 11 |
| Models in use | Two or three main models |
| Average age | |
| Refresh cycle | 4 to 5 years |

## Standard setup

| Item | Standard |
|---|---|
| Naming | `PC-<serial>` |
| Join type | Entra joined / hybrid joined |
| Encryption | BitLocker, keys saved in Entra ID |
| User rights | Standard user, no local admin |
| Security | Defender on, firewall on |
| Core software | Microsoft 365 Apps, browser, PDF reader, security agent |

## Management

| Item | Value |
|---|---|
| Tool | Microsoft Intune / other |
| Enrollment | Autopilot / manual |
| Updates | Update rings, see the Intune repo |
| Remote actions | Sync, lock, wipe, with who may use them |

Details for Intune live in [intune-endpoint-management](https://github.com/mehedi-itpro/intune-endpoint-management).

## Software

| Software | Version | Licence | Deployed by | Owner |
|---|---|---|---|---|
| Microsoft 365 Apps | Current channel | In M365 licence | Intune | IT |
| | | | | |

## Peripherals

| Type | Standard model | Notes |
|---|---|---|
| Printers | | Where they are, who supports them |
| Scanners | | |
| UPS | | |

## Lifecycle

| Stage | Process |
|---|---|
| Buy | Specification, approval, supplier |
| Set up | Standard setup above |
| Hand over | Handover checklist signed |
| Return | Wipe, check, return to stock |
| Dispose | Data wipe, certificate, asset register updated |
