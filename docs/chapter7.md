# Chapter 7 --- Audit Logging, Monitoring, and Alerting

## Unified Audit Log

How to activate the Unified Audit Log: [Turn auditing on or off \| Microsoft Learn](https://learn.microsoft.com/en-us/purview/audit-log-enable-disable)

**PowerShell Example**

Search-UnifiedAuditLog -StartDate (Get-Date).AddDays(-1)

## Alert Policies

How to create M365 health alerts: [Microsoft 365 Health Dashboard - Microsoft 365 admin \| Microsoft Learn](https://learn.microsoft.com/en-us/microsoft-365/admin/manage/health-dashboard-overview?view=o365-worldwide)

**PowerShell Example**

Get-ProtectionAlert
