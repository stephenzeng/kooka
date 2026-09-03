# SharePoint
**Date created:** 2026-09-03 UTC  
**Tags:** Best Practices, Compliance, Configuration, Governance, Troubleshooting  

## Moderate Changes

- **Restrict OneDrive and SharePoint site creation by users**

  Updated restricted site creation policies to clarify that the "Team" site type applies only to classic SharePoint team sites, excluding group-connected sites. This refinement helps admins avoid unintentionally restricting modern, group-connected site creation and align policies with current site architectures.

  https://learn.microsoft.com/en-us/sharepoint/restricted-site-creation

- **Manage unlicensed OneDrive user accounts**

  Clarified that unlicensed OneDrive accounts for users deleted in Entra ID are removed through the standard OneDrive deletion process, even if those accounts were archived. This sets clear expectations for retention and cleanup so admins can plan deprovisioning and data access accordingly.

  https://learn.microsoft.com/en-us/sharepoint/unlicensed-onedrive-accounts

- **IT Admins - Use OneDrive policies to control sync settings**

  Added guidance that enabling the policy creates the registry key HKLM\SOFTWARE\Policies\Microsoft\OneDrive SharePointOnPremFrontDoorUrl and emphasized including a trailing slash in the URL (for example, https://sharepoint.contoso.local/) to prevent sync setup failures. This clarification reduces configuration errors and improves reliability during OneDrive sync deployment.

  https://learn.microsoft.com/en-us/sharepoint/use-group-policy