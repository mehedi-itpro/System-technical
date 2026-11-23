# 08 - Telephony and intercom

Owner: ________  Last reviewed: ________

## Overview

| Item | Value |
|---|---|
| System | IP PABX (model or software) |
| Location | Rack or server |
| Version | |
| Support vendor | |
| Backup of configuration | Where and how often |

## External lines (trunks)

| Name | Provider | Type | Numbers | Channels | Notes |
|---|---|---|---|---|---|
| Trunk-1 (example) | Telco-A | SIP / PRI / GSM gateway | | 10 | |

## Numbering plan

| Range | Use |
|---|---|
| 100-199 | Head office staff (example) |
| 200-299 | Project site 1 |
| 800-899 | Hunt groups and queues |
| 9 | Dial out |

## Extensions

Keep the full list in a register (name, extension, device, site, voicemail). Summary:

| Type | Count | Notes |
|---|---|---|
| IP phones | | Model, VLAN 40 |
| Softphones | | |
| Analogue phones and fax | | Through gateway |

## Call routing

| Rule | Behaviour |
|---|---|
| Office hours | Main number rings reception, then a hunt group |
| After hours | Greeting, then voicemail |
| Holidays | |
| Emergency numbers | Always allowed |

## Intercom

| Location | Device | Connected to | Notes |
|---|---|---|---|
| Main gate (example) | | Extension 150 | |

## Network requirements

| Item | Value |
|---|---|
| Voice VLAN | 40, see [02](02-network.md) |
| QoS | Voice traffic prioritised on the router |
| Firewall | Only the provider's addresses may reach the PABX |
| Remote extensions | Over VPN only |

## Common tasks

How to add an extension, change a routing rule, reset a voicemail PIN and restore the configuration. Write each as numbered steps.
