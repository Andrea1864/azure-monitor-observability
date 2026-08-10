# Azure Monitor Architecture — TechPay Solutions

## Architecture Overview

Azure Resources
│
├── Log Analytics Workspace (law-sentinel-techpay)
├── Microsoft Sentinel (SecurityInsights)
└── Resource Group (rg-sentinel-lab)
│
▼
Azure Monitor
│
├── Activity Log ────────────────→ Who did what and when
│ ├── Administrative operations
│ ├── Security events
│ └── Resource changes
│
├── Metrics ─────────────────────→ Performance data
│ └── Heartbeat (workspace activity)
│
└── Alerts ──────────────────────→ Notifications
├── Delete Workspace Alert
└── Admin Operations Alert
│
▼
Action Group (ag-techpay-security)
│
▼
Email notification → Security team → Investigation


## Alert Rules Summary
| Alert | Trigger | Severity | Response |
|---|---|---|---|
| Delete Workspace | Workspace deletion attempt | Critical | Immediate |
| Admin Operations | Any admin change | Medium | 24h review |

## Integration with Microsoft Sentinel

Azure Monitor Activity Log
│
▼
Log Analytics Workspace
│
▼
Microsoft Sentinel
│
▼
KQL Detection Rules → Incidents → SOC Investigation


## Key Metrics Monitored
| Metric | Source | Purpose |
|---|---|---|
| Heartbeat | Log Analytics | Workspace availability |
| Alert count | Azure Monitor | Security event volume |
| Activity log events | Azure Activity | Audit trail |

## GDPR Compliance Support
| GDPR Article | Azure Monitor Feature |
|---|---|
| Art. 32 — Security | Alert rules detect threats |
| Art. 5(1)(f) — Integrity | Activity log audit trail |
| Art. 33 — Breach notification | Alerts enable 72h response |
| Art. 30 — Records | Activity log as evidence |
