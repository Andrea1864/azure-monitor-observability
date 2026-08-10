# Alert Rule: TechPay - Delete Workspace

## Overview
- **Alert Name**: TechPay-Alert-DeleteWorkspace
- **Severity**: Critical
- **Resource**: law-sentinel-techpay (Log Analytics Workspace)
- **Region**: France Central

## Condition
- **Signal type**: Activity Log
- **Operation**: Delete Workspace
- **Evaluation frequency**: Every 6 hours

## Why This Alert Matters
Deleting the Sentinel workspace would:
- Destroy all security logs and audit trails
- Blind the SOC to ongoing attacks
- Violate GDPR Art. 32 (security of processing)
- Potentially constitute evidence tampering

## Action Group
- **Group name**: ag-techpay-security
- **Notification**: Email to Security team
- **Response SLA**: Immediate investigation required

## GDPR Connection
- Art. 32 — Security of processing
- Art. 5(1)(f) — Integrity and confidentiality
- Art. 33 — Breach notification support
