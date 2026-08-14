# Power Apps
**Date created:** 2026-08-14 UTC  
**Tags:** Automation, Best Practices, Configuration, Guidance, Security  

## Major Changes

- **Customize Views in Model-driven Apps**
  Overhauled and expanded guidance for customizing views, with a full restructure that modernizes best practices and terminology. Added solution-aware operations across SDK for .NET and Dataverse CLI, including creating, updating, retrieving, and deactivating views; replaced prior SetStateRequest with UpdateRequest and CLI PATCH examples. Expanded creation and retrieval guidance with updated property tables and end-to-end samples, and enhanced instructions for editing columns and custom icons, including read-only grid notes, updated layout XML, and tooltip localization. Introduced a new section listing community tools, and emphasized managing views as solution components using SolutionUniqueName to align changes with ALM practices.  
  https://learn.microsoft.com/en-us/power-apps/developer/model-driven-apps/customize-entity-views

## Moderate Changes

- **Send In-App Notifications Within Model-Driven Apps**
  Added guidance on supported URL formats for notification actions, covering HTTPS/HTTP, mailto, tel, Dynamics 365 deep links, and same-origin paths. Introduced security restrictions that block unsafe schemes (e.g., javascript:, data:), protocol-relative URLs, and bare relative paths, with updated examples and recommendations to use same-origin URLs starting with “/” to ensure reliable behavior.  
  https://learn.microsoft.com/en-us/power-apps/developer/model-driven-apps/clientapi/send-in-app-notifications

- **Work Queue Item (workqueueitem) table/entity reference (Microsoft Dataverse)**
  Documented a new attribute, latestflowrunid, including its metadata (display name, logical name, type, and usage). This addition helps identify the Flow run that processed a work item, improving automation traceability and troubleshooting.  
  https://learn.microsoft.com/en-us/power-apps/developer/data-platform/reference/entities/workqueueitem