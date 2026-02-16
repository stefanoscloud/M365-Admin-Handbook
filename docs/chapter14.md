# Chapter 14 --- M365 Operational Checklists {#chapter-14-m365-operational-checklists .unnumbered}

This section provides typical daily, weekly and monthly operational tasks for M365 administrators. The checklists can be expanded based on the needs of each organization.

## Daily Checklist {#daily-checklist .unnumbered}

- Review Defender XDR alerts

- Review Purview DLP alerts

- Check service health dashboard

- Review risky sign‑ins

- Validate overnight Intune deployments

- Check mail flow status

- Review audit log for anomalies

**Daily PowerShell Examples**

Get-MgSecurityAlert -Filter \"status ne \'resolved\'\"

Search-UnifiedAuditLog -StartDate (Get-Date).AddHours(-24)

Get-MgRiskyUser

## Weekly Checklist {#weekly-checklist .unnumbered}

- Review Conditional Access sign‑in patterns

- Validate license assignments

- Review Teams/SharePoint sprawl

- Run Maester security tests

- Review PIM activations

- Check backup status

**Weekly PowerShell Examples**

Get-MgIdentityConditionalAccessPolicy

Get-MgUserLicenseDetail

Get-SPOSite

## Monthly Checklist {#monthly-checklist .unnumbered}

- Access reviews

- User onboarding and offboarding scripts

- DLP policy tuning

- Sensitivity label analytics

- Update documentation

- Review admin role assignments

- Patch Intune baselines

- Validate BCDR procedures

**Monthly PowerShell Examples**

Get-MgIdentityGovernanceAccessReviewDefinition

Get-DlpCompliancePolicy

Get-MgDirectoryRoleMember

