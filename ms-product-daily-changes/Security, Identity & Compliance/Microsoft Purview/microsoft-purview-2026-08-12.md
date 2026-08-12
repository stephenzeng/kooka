# Microsoft Purview
**Date created:** 2026-08-12 UTC  
**Tags:** Configuration, Guidance  

## Moderate Changes

- **Automatically apply a sensitivity label to Microsoft 365 data**

  Clarified portal limits for auto-labeling policies: tenants can have up to 100 policies, and each policy can include or exclude up to 100 SharePoint or OneDrive locations; the All setting is not constrained by the 100-location limit. Added PowerShell guidance to target more than 100 SharePoint sites using adaptive scopes with New-AutoSensitivityLabelPolicy (-SharePointAdaptiveScopes and -SharePointAdaptiveScopesException), replacing static site lists without increasing portal limits.

  https://learn.microsoft.com/en-us/purview/apply-sensitivity-label-automatically