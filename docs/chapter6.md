# Chapter 6 --- Privileged Access and Conditional Access (Adaptive Access) {#chapter-6-privileged-access-and-conditional-access-adaptive-access .unnumbered}

## Privileged Roles

**PowerShell Example: Enable PIM Role**

Start-MgRoleManagementDirectoryRoleAssignmentScheduleRequest

## Administrative Units

**PowerShell Example: Create AU**

New-MgAdministrativeUnit -DisplayName \"EU-Users\"

## Conditional Access

Getting started: [Microsoft Entra Conditional Access documentation - Microsoft Entra ID \| Microsoft Learn](https://learn.microsoft.com/en-us/entra/identity/conditional-access/)

**PowerShell Example**

Get-MgIdentityConditionalAccessPolicy
