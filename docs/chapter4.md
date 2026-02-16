# Chapter 4 --- Identity Synchronization and Hybrid Identity

## 4.1 Choosing Identity Model

Review: https://learn.microsoft.com/en-us/microsoft-365/enterprise/deploy-identity-solution-identity-model?view=o365-worldwide and also check the M365 admin portal relevant deployment guide.

- Cloud‑only

- Entra Connect Sync

- Entra Cloud Sync

- Federation

## 4.2 Hybrid Identity Operations

**PowerShell Example: Check Sync Status**

Get-ADSyncScheduler

## 4.3 Identity Governance

**PowerShell Example: List Access Reviews**

Get-MgIdentityGovernanceAccessReviewDefinition
