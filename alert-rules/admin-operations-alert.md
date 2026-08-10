# Alert Rule: TechPay - Administrative Operations

## Overview
- **Alert Name**: TechPay-Alert-AdminOperations
- **Severity**: Medium
- **Resource**: law-sentinel-techpay (Log Analytics Workspace)
- **Region**: France Central

## Condition
- **Signal type**: Activity Log
- **Operation**: All Administrative Operations
- **Evaluation frequency**: Every 6 hours

## Why This Alert Matters
Monitoring all administrative operations ensures:
- Full audit trail of configuration changes
- Detection of unauthorized modifications
- Compliance with GDPR Art. 32
- Support for incident investigation

## Examples of Monitored Operations
| Operation | Risk Level | Action |
|---|---|---|
| Delete Workspace | Critical | Immediate response |
| Change retention settings | High | DPO notification |
| Modify access controls | High | Security review |
| Create new diagnostic settings | Medium | Log and review |

## Action Group
- **Group name**: ag-techpay-security
- **Notification**: Email to Security team
- **Response SLA**: Review within 24 hours

## GDPR Connection
- Art. 32 — Security of processing
- Art. 5(1)(f) — Integrity and confidentiality
- Art. 30 — Records of processing activities
