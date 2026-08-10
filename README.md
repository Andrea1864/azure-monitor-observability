# azure-monitor-observability
Azure Monitor observability and alerting lab for a fictional fintech company — TechPay Solutions
# Azure Monitor Observability Lab — TechPay Solutions

## Project Overview
This project implements Azure Monitor for infrastructure 
observability and security alerting for a fictional fintech 
company — TechPay Solutions S.L. It covers activity log 
analysis, alert rule configuration, and metrics monitoring.

## What This Project Covers
- Azure Monitor configuration for Log Analytics Workspace
- Activity log analysis — audit trail of all Azure operations
- 2 security alert rules for critical infrastructure events
- Metrics monitoring (Heartbeat) for workspace availability
- Action group configuration for security notifications
- GDPR compliance support through audit trail and alerting

## Alert Rules Implemented
| Alert | Trigger | Severity | Notification |
|---|---|---|---|
| Delete Workspace | Workspace deletion attempt | Critical | Email immediate |
| Admin Operations | Any administrative change | Medium | Email 24h review |

## Tools & Technologies
- Azure Monitor
- Azure Activity Log
- Azure Metrics
- Azure Alerts
- Log Analytics Workspace
- Action Groups

## GDPR Compliance Support
| Article | Azure Monitor Feature |
|---|---|
| Art. 32 — Security | Alert rules detect threats |
| Art. 5(1)(f) — Integrity | Activity log audit trail |
| Art. 33 — Breach notification | Alerts enable 72h response |
| Art. 30 — Records | Activity log as evidence |

## Key Findings from Activity Log
During this lab the following events were recorded:
- Sentinel workspace deployment (Thu Aug 06)
- Alert rule updates (Thu Aug 06)
- Role assignment creation (Thu Aug 06)
- New security recommendations from Microsoft Advisor

## Architecture
See [monitor-architecture.md](docs/monitor-architecture.md) 
for the full architecture diagram.

## Related Projects
- [Microsoft Sentinel Lab](https://github.com/Andrea1864/siem-microsoft-sentinel)
- [TechPay GDPR ROPA](https://github.com/Andrea1864/gdpr-ropa-fintech)
- [Microsoft Purview Lab](https://github.com/Andrea1864/microsoft-purview-data-protection)

## Author
Andrea Castillo— Law Graduate | Cybersecurity & GRC Specialist  
