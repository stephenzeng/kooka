# SharePoint
**Date created:** 2026-08-25 UTC  
**Tags:** Compliance, Configuration  

## Moderate Changes

- **Plan compliance requirements for SharePoint and OneDrive**

  
  Updated compliance guidance to include a new OneDrive sync app policy that lets admins exclude specific folders from being uploaded. Added references for configuring the setting on Windows (EnableODIgnoreFolderListFromGPO) and macOS (EnableODIgnoreFolders) to help enforce data governance and reduce unwanted sync.

  
  https://learn.microsoft.com/en-us/sharepoint/compliant-environment

- **Deploy and configure the OneDrive sync app for Mac**

  
  Added the EnableODIgnoreFolders setting to exclude specified folder names from OneDrive uploads, including behavior details and caveats. Documented that a sync app restart is required for changes to take effect and provided a sample .plist, along with adding the key to the macOS settings list to simplify deployment.

  
  https://learn.microsoft.com/en-us/sharepoint/deploy-and-configure-on-macos

- **Plan file sync for SharePoint and OneDrive in Microsoft 365**

  
  Expanded planning guidance from file-type exclusions to include folder-level upload exclusions. Introduced new policies for Windows (EnableODIgnoreFolderListFromGPO) and macOS (EnableODIgnoreFolders), clarified that excluded items remain on the local device, and updated navigation and headings to reflect the broader scope.

  
  https://learn.microsoft.com/en-us/sharepoint/plan-file-sync