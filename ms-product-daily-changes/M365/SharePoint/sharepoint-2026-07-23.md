# SharePoint
**Date created:** 2026-07-23 UTC  
**Tags:** Governance, Other  

## Moderate Changes

- **Generate structured documents in a SharePoint document library**

  Added an important note clarifying that conditional sections are evaluated only at generation time and do not re-evaluate in Word for the web after field changes. Provided guidance to regenerate via the form or use Word for Windows to re-evaluate, documenting a current platform limitation that helps authors avoid confusion post-generation.

  https://learn.microsoft.com/en-us/sharepoint/copilot-in-sharepoint-structured-document-generation

- **Restrict discovery of SharePoint sites and content**

  Removed the “Apply Restricted Content Discovery to multiple sites” section, retiring prior guidance for bulk application across sites. Administrators should rely on current, supported approaches for configuration, as earlier notes on propagation behavior and guardrails are no longer included.

  https://learn.microsoft.com/en-us/sharepoint/restricted-content-discovery