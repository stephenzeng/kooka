# Dev and Admin for Dynamics 365 Business Central
**Date created:** 2026-08-14 UTC  
**Tags:** Best Practices, Guidance  

## Major Changes

- **File.View(Text [, Boolean]) Method**
  
  Updated guidance clarifies that File.View is supported only for Business Central on-premises; online scenarios should use File.ViewFromStream instead. The example now demonstrates opening an existing server-side file on the client using a full server path. Prior content showing PDF generation with Temp Blob and display via File.ViewFromStream was removed to prevent misuse. This change helps developers choose the correct API for their environment and avoid unsupported patterns in online deployments.
  
  https://learn.microsoft.com/en-us/dynamics365/business-central/dev-itpro/developer/methods-auto/file/file-view-method