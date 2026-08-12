# Power Apps
**Date created:** 2026-08-12 UTC  
**Tags:** Configuration, Guidance  

## Moderate Changes

- **Embed a code app in an iframe**

  Updated guidance by removing a note that previously blocked embedding code apps in native desktop or mobile applications, reducing ambiguity around supported embedding scenarios. Tenant access limitations remain unchanged, helping admins and makers assess deployment constraints.

  https://learn.microsoft.com/en-us/power-apps/developer/code-apps/how-to/embed-iframe

- **Link to Microsoft Fabric**

  Updated the Finance and operations compatibility matrix: removed version 10.0.46, adjusted minimum platform/application builds for 10.0.47 and 10.0.48, and added support for 10.0.49 with defined minimum builds. This helps teams plan upgrades and ensure supported configurations.

  https://learn.microsoft.com/en-us/power-apps/maker/data-platform/fabric-link-to-data-platform

- **updateContext (Client API reference)**

  Removed preview labels to reflect that the updateContext API is now generally available. This signals production readiness without changes to API behavior.

  https://learn.microsoft.com/en-us/power-apps/developer/model-driven-apps/clientapi/reference/Xrm-Copilot/updatecontext

- **Xrm.Copilot (Client API reference) in model-driven apps**

  Reorganized method listings to clearly separate generally available methods from preview methods, moving executeEvent and executePrompt into the preview section. This clarifies stability and support expectations for developers.

  https://learn.microsoft.com/en-us/power-apps/developer/model-driven-apps/clientapi/reference/xrm-copilot