# Chapter 3 --- Entra Organizational Structure, RBAC, and Licensing {#chapter-3-entra-organizational-structure-rbac-and-licensing .unnumbered}

## Documenting the Organization

**What to Document**

- Departments

- Security groups

- Existing Active Directory or local group policies (GPO)

- Existing MDM/MAM (Intune) policies

- Regions

- User personas and business roles

- Data sensitivity

- Collaboration patterns and business flows

## RBAC Strategy

Start with minimum two (2) and maximum four (4) global admins. Setup break glass access administrator accounts. Delegate the Billing Admins and the Privilege Role Admins, then use PIM to delegate all other non-global admin roles to groups/users as required by your organization setup. Entra ID P2 licensing is a must for proper RBAC and role delegation management (via PIM). Consider the RBAC schemas of each M365 service (e.g. Entra RBAC, Defender XDR unified RBAC, Purview RBAC, etc). You may need to assign role groups from non-Entra services to your Global admins for them to be enabled for specialized administration scenarios, e.g. the Exchange Online OrganizationManager role group.

**PowerShell Example: List Directory Roles**

Get-MgDirectoryRole

**Assign Role**

Add-MgDirectoryRoleMember -DirectoryRoleId \$role -DirectoryObjectId \$user

## Restricting Group Creation

Manage who can create groups in your M365 tenant by implementing instructions at: [Manage who can create Microsoft 365 Groups \| Microsoft Learn](https://learn.microsoft.com/en-us/microsoft-365/solutions/manage-creation-of-groups?view=o365-worldwide).

**PowerShell Example**

Set-MsolCompanySettings -UsersPermissionToCreateGroupsEnabled \$false

## Licensing Strategy

Checkout comparisons of the M365 licensing plans at: [Microsoft 365 Business Plans and Pricing \| Microsoft 365](https://www.microsoft.com/en-us/microsoft-365/business/microsoft-365-plans-and-pricing). Checkout the available security licensing suites at: <https://www.microsoft.com/en-us/security/pricing/enterprise/security-suites>

**PowerShell Example: Assign License**

Set-MgUserLicense -UserId user@contoso.com -AddLicenses @{SkuId=\$e3}
