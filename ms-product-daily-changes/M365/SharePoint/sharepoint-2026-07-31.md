# SharePoint
**Date created:** 2026-07-31 UTC  
**Tags:** Administration, Analytics, Governance, Security  

## New Articles

- **Data access governance reports - get sites and files shared via special SharePoint groups**

  Introduced a new article that explains how to run a snapshot report to find sites and files shared via the special SharePoint groups “Everyone except external users” and “Everyone.” It details when to use the report to uncover oversharing that could surface in Microsoft 365 Copilot, required roles, and operational limits. Step-by-step guidance is provided to run and download the report, with full descriptions of all CSV columns and example scenarios. The article also notes system exceptions and links to remediation guidance and related content.

  https://learn.microsoft.com/en-us/sharepoint/data-access-governance-detailed-eeeu-everyone-permissions-report

## Moderate Changes

- **Data access governance reports for SharePoint and OneDrive sites**

  Added a section for the “sites and files shared via special SharePoint groups” report that flags content made broadly accessible through Everyone/EEEU. The update explains how the report accelerates cleanup through scripting and links to the detailed usage guide.

  https://learn.microsoft.com/en-us/sharepoint/data-access-governance-reports

- **Manage Data access governance reports using SharePoint Online PowerShell**

  Added guidance to generate item-level reports for Everyone/EEEU sharing via PowerShell, including required module version, role prerequisites, supported scopes, and known limits and exclusions. Updated examples to use the new ReportEntity value for item-level reporting and aligned sample report names accordingly.

  https://learn.microsoft.com/en-us/sharepoint/powershell-for-data-access-governance

- **Restrict SharePoint site access with Microsoft 365 groups and Microsoft Entra security groups**

  Expanded support to include OneDrive for restricted site access controls. Clarified that these policies are enforced in organization-wide search and Copilot, preventing visibility for users outside the control group even if they have direct file permissions.

  https://learn.microsoft.com/en-us/sharepoint/restricted-access-control