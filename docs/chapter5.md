# Chapter 5 --- M365 Apps and Endpoint Management with Intune {#chapter-5-m365-apps-and-endpoint-management-with-intune .unnumbered}

## Enrollment & Compliance {#enrollment-compliance}

**PowerShell Example: List Devices**

Get-MgDevice

## Endpoint Security

**PowerShell Example: List ASR Rules**

Get-MpPreference \| Select-Object AttackSurfaceReductionRules_Ids

## M365 App Policies and MAM policies

Utilize the Microsoft Office Deployment Tool (ODT) and the config.microsoft.com portal for creating and applying policies.

- <https://www.microsoft.com/en-us/download/details.aspx?id=49117&msockid=19122ead46d865c23f3b39af47af64ee>

- [Microsoft 365 Apps admin center](https://config.office.com/)

**PowerShell Example**

Get-MgBetaDeviceAppManagementMobileAppConfiguration

You can complement the above with Intune MAM policies for Microsoft 365 Apps.

- [Policies for Microsoft 365 Apps - Microsoft Intune \| Microsoft Learn](https://learn.microsoft.com/en-us/intune/intune-service/apps/app-office-policies)
