# Power Platform
**Date created:** 2026-08-28 UTC  
**Tags:** Configuration, Governance, Guidance, Security  

## Moderate Changes

- **Secure the default environment**

  Added guidance to create a data policy for the default environment in managed environments, instructing admins to block all connectors using Advanced connector policies scoped to the default environment with empty Business/Non-Business groups. If managed environments aren’t available, it recommends blocking new connectors, restricting makers to prebuilt connectors, and limiting custom connectors to reduce data leakage risk and strengthen governance.

  https://learn.microsoft.com/en-us/power-platform/guidance/adoption/secure-default-environment