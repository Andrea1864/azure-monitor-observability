# Scenario Overview — TechPay Solutions Azure Monitor Lab

## Company Profile
- **Name**: TechPay Solutions S.L.
- **Sector**: Financial Technology (Fintech)
- **Employees**: 50
- **Location**: Barcelona, Spain
- **Services**: Digital payment processing, peer-to-peer 
  transfers, virtual card issuing

## Monitoring Context
TechPay uses Azure Monitor to ensure operational visibility 
and security compliance across its Azure infrastructure. 
Azure Monitor complements Microsoft Sentinel by providing:
- Infrastructure health monitoring
- Security alert rules for critical operations
- Audit trail of all administrative actions
- Metrics and performance data

## Resources Monitored
| Resource | Type | Purpose |
|---|---|---|
| law-sentinel-techpay | Log Analytics Workspace | SIEM data storage |
| rg-sentinel-lab | Resource Group | Infrastructure container |
| Azure subscription 1 | Subscription | Full environment scope |

## Regulatory Context
| Regulation | Monitoring Requirement |
|---|---|
| GDPR Art. 32 | Security monitoring and audit trails |
| GDPR Art. 5(1)(f) | Integrity and confidentiality |
| DORA Art. 10 | ICT monitoring and detection |
| ENS (Spain) | Continuous monitoring obligation |
