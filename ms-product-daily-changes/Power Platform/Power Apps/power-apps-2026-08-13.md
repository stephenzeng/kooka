# Power Apps
**Date created:** 2026-08-13 UTC  
**Tags:** Configuration, Deprecation, Guidance, Identity  

## Moderate Changes

- **Work with Microsoft Entra ID group teams**

  Clarified that team member synchronization only includes Entra group members already provisioned as users in Dataverse. Administrators should create Dataverse user records for new Entra group members before synchronization to ensure team membership is accurately reflected.

  https://learn.microsoft.com/en-us/power-apps/developer/data-platform/aad-group-team

- **App navigation in model-driven apps with Power Apps**

  Updated guidance for configuring areas, including localized titles and descriptions, and introduced a Generative page option that uses natural language to create pages. Expanded dashboard guidance to cover Dataverse and Power BI embedded dashboards, and aligned publishing steps to use Save and Publish.

  https://learn.microsoft.com/en-us/power-apps/maker/model-driven-apps/app-navigation

- **Add the rich text editor control to a model-driven app with Power Apps**

  Removed references to unsupported custom-storage properties and clarified that imageEntity and attachmentEntity used with the classic editor are not compatible with the modern rich text editor. This helps avoid misconfiguration and guides makers to use supported capabilities in the modern control.

  https://learn.microsoft.com/en-us/power-apps/maker/model-driven-apps/rich-text-editor-control