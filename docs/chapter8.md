# Chapter 8 --- Purview Compliance, Data Classification and Sensitivity Labels

## 8.1 Data Discovery and Data Lifecycle Management

Getting started:

- Lifecycle management: [Get started with data lifecycle management \| Microsoft Learn](https://learn.microsoft.com/en-us/purview/get-started-with-data-lifecycle-management)

- M365 data locations: [Microsoft 365 data locations - Microsoft 365 Enterprise \| Microsoft Learn](https://learn.microsoft.com/en-us/microsoft-365/enterprise/o365-data-locations?view=o365-worldwide)

- Information Protection Scanner: [Learn about the Microsoft Purview Information Protection scanner \| Microsoft Learn](https://learn.microsoft.com/en-us/purview/deploy-scanner)

- Information Protection Client: <https://www.microsoft.com/en-us/download/details.aspx?id=53018&msockid=19122ead46d865c23f3b39af47af64ee>

- Self-service data discovery and access: <https://learn.microsoft.com/en-us/purview/legacy/concept-self-service-data-access-policy>

**PowerShell Example**

Get-Label

## 8.2 Sensitivity Labels

Getting started: [Get started with sensitivity labels \| Microsoft Learn](https://learn.microsoft.com/en-us/purview/get-started-with-sensitivity-labels)

Use Sensitive Information Types (SIT) and Trainable Classifiers for your data: [Get started with trainable classifiers \| Microsoft Learn](https://learn.microsoft.com/en-us/purview/trainable-classifiers-get-started-with)

**PowerShell Example**

Get-LabelPolicy

## 8.3 Retention policies and archiving policies

Use Purview modern retention policies, as per: <https://learn.microsoft.com/en-us/purview/create-retention-policies?tabs=teams-retention>

Use legacy MRM policies for archiving policies to Exchange Online archive: [Customize an archive and deletion policy (MRM) for mailboxes \| Microsoft Learn](https://learn.microsoft.com/en-us/purview/set-up-an-archive-and-deletion-policy-for-mailboxes)

## 8.4 Insider Risk Management & Adaptive Protection

Getting started: [Get started with Insider Risk Management \| Microsoft Learn](https://learn.microsoft.com/en-us/purview/insider-risk-management-configure)

**PowerShell Example**

Get-MgSecurityUserRisk

## 8.5 Information Barriers (IB)

Create IB segments and define IB operations mode, as per your requirements.

Getting started: [Get started with Information Barriers \| Microsoft Learn](https://learn.microsoft.com/en-us/purview/information-barriers-policies)

## 8.6 DLP Policies

Getting started: [Get started with endpoint data loss prevention \| Microsoft Learn](https://learn.microsoft.com/en-us/purview/endpoint-dlp-getting-started)

**PowerShell Example**

Get-DlpCompliancePolicy

## 8.7 Purview Compliance Score

Manage your Compliance Manager Secure Score as per: <https://learn.microsoft.com/en-us/purview/compliance-manager-scoring>
