# Chapter 2 --- Tenant Initialization and Setup {#chapter-2-tenant-initialization-and-setup .unnumbered}

***Greenfield, brownfield, multi‑geo, and MTO operations***

1.  

## Greenfield Tenant Setup

**The initial M365 tenant setup checklist:**

- Add custom domains and configure company branding

- Configure DNS records

- Create break‑glass accounts with FIDO2 passwordless authentication

- Enable MFA + SSPR

- Configure Entra Tenant Properties and User/Group properties

- Configure baseline Conditional Access policies

- Enable unified audit logging at tenant level

- Plan for M365 guest users and SharePoint/OneDrive external/guest sharing policy defaults

- Run M365 setup checklist and advanced deployment guides available at:

  - [Setup - Microsoft 365 admin center](https://admin.cloud.microsoft/?#/featureexplorer)

  - [Advanced deployment guides for Microsoft 365 and Office 365 products - Microsoft 365 Enterprise \| Microsoft Learn](https://learn.microsoft.com/en-us/microsoft-365/enterprise/setup-guides-for-microsoft-365?view=o365-worldwide)

**PowerShell Example: Add Domain**

New-MgDomain -Id \"contoso.com\"

## Brownfield Tenants (existing tenants)

**Audit checklist of an existing tenant or multiple tenants**

- Identity configuration

- Conditional Access policies

- Licensing usage

- Security posture

- SharePoint/Teams sprawl

- Mail flow rules

**PowerShell Example: List CA Policies**

Get-MgIdentityConditionalAccessPolicy

## Tenant‑to‑Tenant Migration Scenarios  {#tenanttotenant-migration-scenarios}

**A tenant-to-tenant migration may be needed in case of Geo/Billing center changes. Key Tasks include:**

- Domain transfer

- Identity consolidation

- Mailbox migration

- SharePoint/OneDrive migration

- Teams migration

- Post‑migration cleanup

## Multi‑Geo & Multi-tenant Organization (MTO) {#multigeo-multi-tenant-organization-mto}

Review requirements and features at:

- [Microsoft 365 Multi-Geo - Microsoft 365 Enterprise \| Microsoft Learn](https://learn.microsoft.com/en-us/microsoft-365/enterprise/microsoft-365-multi-geo?view=o365-worldwide)

- [Plan for multitenant organizations in Microsoft 365 - Microsoft 365 Enterprise \| Microsoft Learn](https://learn.microsoft.com/en-us/microsoft-365/enterprise/plan-multi-tenant-org-overview?view=o365-worldwide)

**PowerShell Example: Assign Geo Location**

Set-MsolUser -UserPrincipalName user@contoso.com -UsageLocation \"DE\"

## M365 service performance checks

Use Microsoft Connectivity Test to determine performance: [Microsoft 365 network connectivity test](https://connectivity.office.com/)
