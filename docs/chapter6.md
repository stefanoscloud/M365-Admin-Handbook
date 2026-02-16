# Chapter 6 --- Privileged Access and Conditional Access (Adaptive Access)

## 6.1 Privileged Roles

**PowerShell Example: Enable PIM Role**

Start-MgRoleManagementDirectoryRoleAssignmentScheduleRequest

## 6.2 Administrative Units
Use AUs for scoping privileged objects management

**PowerShell Example: Create AU**

New-MgAdministrativeUnit -DisplayName \"EU-Users\"

## 6.3 Conditional Access

Getting started: [Microsoft Entra Conditional Access documentation - Microsoft Entra ID \| Microsoft Learn](https://learn.microsoft.com/en-us/entra/identity/conditional-access/)

**PowerShell Example**

Get-MgIdentityConditionalAccessPolicy
