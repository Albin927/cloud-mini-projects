# Project 13: Azure VM Security Log Monitoring

## Objective

Configured Azure monitoring to collect Windows security events from a virtual machine and used Kusto Query Language (KQL) to identify failed login attempts.

## Azure Services Used

- Azure Virtual Machine
- Azure Monitor
- Log Analytics Workspace
- Windows Security Events
- Kusto Query Language (KQL)

## KQL Query

```kql
Event
| where EventID == 4625
| project TimeGenerated, Computer, RenderedDescription
| sort by TimeGenerated desc