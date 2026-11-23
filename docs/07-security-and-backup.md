# 07 - Security and backup

Owner: ________  Last reviewed: ________

## Security baseline

| Control | Standard | Status |
|---|---|---|
| MFA for all users | Required | |
| Admin accounts separate from daily accounts | Required | |
| Break-glass accounts | Two, tested, monitored | |
| Legacy authentication | Blocked | |
| Disk encryption on all PCs | Required | |
| Local admin passwords | Unique per device (LAPS) | |
| Antivirus and EDR | Defender on all PCs and servers | |
| Firewall | Default deny from the internet | |
| Patching | See [03](03-servers.md) and [06](06-endpoints.md) | |
| Password vault | Name of the tool and who has access | |

Mark each line **Yes, No or Partly**. A line marked No needs an owner and a date in the risk table below.

## Logging

| Source | Where logs go | Kept for | Who reviews |
|---|---|---|---|
| Microsoft 365 and Entra sign-ins | | | |
| Routers and firewalls | | | |
| Servers | | | |

## Backup

| System | What is backed up | Tool | Frequency | Kept for | Stored where | Copy off-site or offline |
|---|---|---|---|---|---|---|
| File server | Shares | | Daily | 30 days | | Yes |
| Microsoft 365 | Mail, OneDrive, SharePoint | | Daily | | | |
| Network devices | Config exports | | Weekly | | | |
| Azure workloads | | | | | | |

Rule of thumb: three copies, two types of storage, one copy off-site or offline.

## Recovery targets

| System | Recovery time target | Data loss target | Last restore test | Result |
|---|---|---|---|---|
| File server | | | | |
| Email | | | | |
| Domain controller | | | | |

A backup that has never been restored is a hope, not a backup. Test each system at least twice a year and record the result.

## Incident response

| Step | Who | Notes |
|---|---|---|
| Report | Anyone to IT helpdesk | Channel and phone number |
| Assess | IT lead | Severity, what is affected |
| Contain | IT | Isolate the device, reset credentials, block sign-in |
| Recover | IT | Restore from backup |
| Review | IT lead, within a week | What happened, what changes |

External contacts: ISP, Microsoft partner, legal, insurer. Lost or stolen device: wipe procedure is in the endpoint repo.

## Open risks

| Risk | Impact | Owner | Fix by |
|---|---|---|---|
| | | | |
