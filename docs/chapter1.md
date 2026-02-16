# Chapter 1 --- Foundations of Microsoft 365 Administration#chapter1

***Connecting to Microsoft 365 services and establishing operational access***

Microsoft 365 administration relies on three primary access methods: **PowerShell**, **APIs**, and **administrative Web-based portals**. A competent administrator must be fluent in all three.

## PowerShell Connectivity#11-powershell-connectivity

**Microsoft Graph PowerShell examples assume installation of the relevant modules from the Powershell Gallery. The following modules must be installed per-case when needed:**

- Install-Module Microsoft.Graph -Scope AllUsers

- Install-Module Microsoft.Entra -Scope AllUsers

- Install-Module MSOnline -Scope AllUsers (legacy)

- Install-Module AzureAD -Scope AllUsers (legacy)

- Install-Module ExchangeOnlineManagement -Scope AllUsers

- Install-Module Microsoft.Online.SharePoint.PowerShell -Scope AllUsers

- Install-Module MicrosoftTeams -Scope AllUsers

- Install-Module Microsoft.Graph.Intune -Scope AllUsers

- Install-Module Microsoft.Graph.Security -Scope AllUsers

**Microsoft Graph and Entra**

Connect-MgGraph -Scopes \"User.ReadWrite.All\",\"Group.ReadWrite.All\"

Get-MgUser -All

Get-EntraUser

**Exchange Online PowerShell**

Connect-ExchangeOnline

Get-Mailbox

**Teams PowerShell**

Connect-MicrosoftTeams

Get-Team

**SharePoint Online PowerShell**

Connect-SPOService -Url https://contoso-admin.sharepoint.com

Get-SPOSite

**Intune Graph SDK**

Get-MgDeviceManagement

**Security and Compliance Powershell**

Import-Module ExchangeOnlineManagement

Connect-IPPSSession -UserPrincipalName \<UPN\> \[-ConnectionUri \<URL\>\] \[-AzureADAuthorizationEndpointUri \<URL\>\] \[-DelegatedOrganization \<String\>\] \[-PSSessionOption \$ProxyOptions\]

**Real‑World Scenario**  
HR updates 4,000 job titles. PowerShell is the only scalable method to manage them.

## API / SDK Connectivity {#api-sdk-connectivity}

**Graph API Example (GET user)**

GET https://graph.microsoft.com/v1.0/users

**Using Graph Explorer**

Ideal for testing queries before automation. Available at: <https://developer.microsoft.com/en-us/graph/graph-explorer>.

**Using Postman with OAuth2**

Used for secure automation pipelines and for testing MgGraph APIs. Available at: <https://www.postman.com/product/>.

**Scenario**   
Security team needs automated export of risky sign‑ins → Graph API + Logic App.

## Administrative Portals

- Microsoft 365 Admin Center (<https://admin.cloud.microsoft>). This includes links to all other administrative Web portals.

- Entra Admin Center

- Defender XDR

- Purview

- Intune

- Exchange / SharePoint / Teams Admin Centers

**Scenario**  
Helpdesk operator needs password reset only → assign "Helpdesk Administrator."

## CSP Operations (GDAP + Lighthouse) {#csp-operations-gdap-lighthouse}

**GDAP** provides least‑privilege delegated access for Cloud Service Providers (CSP).  
**Lighthouse** provides multi‑tenant monitoring. Documentation available at: <https://learn.microsoft.com/en-us/microsoft-365/lighthouse/m365-lighthouse-overview?view=o365-worldwide>.

--- 
Go back to ToC: 
https://github.com/stefanoscloud/M365-Admin-Handbook/blob/main/docs/index.md
