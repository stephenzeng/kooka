# Dynamics 365 Customer Service
**Date created:** 2026-07-30 UTC  
**Tags:** Administration, Agent, AI, Security  

## New Articles

- **Customer Service Copilot tool privilege reference**

  Introduced a new reference that maps Customer Service Copilot tools to the Microsoft Dataverse privileges required for discovery and execution. Explains access behavior, including that all listed privileges are required for gated tools, while tools not in the map may appear but can fail with a 403 during execution. Includes comprehensive tool-to-privilege tables and identifies intentionally ungated tools, including environment operations. Provides administrator guidance for role assignment, validation, handling 403 errors, and cache TTL, with links to related setup topics.

  https://learn.microsoft.com/en-us/dynamics365/customer-service/develop/customer-service-tool-privilege-reference

## Moderate Changes

- **Manage Customer Knowledge Management Agent**

  Reworked the guidance on configuring case attributes for bulk and real-time knowledge harvesting, including clear limits for 1-to-1 (up to 10) and 1-to-many (up to 6) mappings. Added a default mapping table and clarified that all defaults except Title and Description can be remapped, disabled, or deleted, replacing older step-based instructions.

  https://learn.microsoft.com/en-us/dynamics365/customer-service/administer/admin-km-agent

- **Configure sensitivity labels for emails**

  Centralized setup guidance by replacing page-specific instructions with a shared include to ensure consistency and reduce duplication. Local prerequisite and legacy configuration details were removed, and the page now directs admins to consolidated steps.

  https://learn.microsoft.com/en-us/dynamics365/customer-service/administer/configure-email-sensitivity

- **Use sensitivity labels in emails**

  Streamlined end-user guidance by replacing in-page instructions with a shared include that consolidates how to apply labels and related behaviors. The article now points to centralized content for usage details and limitations to maintain a single source of truth.

  https://learn.microsoft.com/en-us/dynamics365/customer-service/use/use-sensitivity-labels