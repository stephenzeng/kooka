# Power Apps
**Date created:** 2026-08-15 UTC  
**Tags:** Compliance, Governance, Guidance, Security, Troubleshooting  

## Moderate Changes

- **FAQ for Power Apps vibe experience (preview)**

  Added a known limitation that published and previewed vibe apps block external images and other external content under a fixed platform Content Security Policy. Clarifies that the CSP restricts content origins to mitigate XSS and injection risks and cannot be customized at the app, environment, or tenant level, including via the Power Platform admin center. Developers should plan to host assets within allowed origins and avoid relying on external resources.

  https://learn.microsoft.com/en-us/power-apps/maker/common/faq-vibe

- **Invoke a function using Power Platform**

  Updated guidance to add the Environment table from the Dataverse connector instead of the generic Environment option, with steps reordered accordingly. Added a note that creating a new app in the same environment provisions the Environment table if it isn’t available. This reduces setup confusion and helps ensure functions can be invoked successfully.

  https://learn.microsoft.com/en-us/power-apps/maker/data-platform/functions-invoke