# Microsoft Viva
**Date created:** 2026-09-02 UTC  
**Tags:** Configuration, Governance, Guidance, Security  

## Major Changes

- **Viva Glint Export APIs**

  Updated the setup workflow to require allowlisting the Entra application ID in the Viva Glint portal, with step-by-step UI guidance, screenshots, and confirmation via the Activity audit log for allowlist and export actions. Clarified how to locate the experience name (clientUuid) directly from the portal URL to streamline configuration. Documented that leaving start and end dates empty exports the last 13 months of data across multiple endpoints. Added PowerShell request samples for survey-level and survey-cycle-level exports to simplify automation. Revised Export Status API values to notStarted, running, succeeded, and failed to improve status clarity and consistency.

  https://learn.microsoft.com/en-us/viva/glint/setup/viva-glint-raw-data-export-apis