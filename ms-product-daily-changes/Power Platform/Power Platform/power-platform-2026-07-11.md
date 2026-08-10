# Power Platform
**Date created:** 2026-07-11 UTC  
**Tags:** Administration, AI, Automation, Programming  

## Major Changes

- **pac admin**
  
  Added a new pac admin query command to run tenant-level resource queries. Documented parameters for output format and file, inline or file-based queries, and default behaviors. Updated the command index and keywords to include the new verb, enabling admins to script queries and export results effectively.  
  https://learn.microsoft.com/en-us/power-platform/developer/cli/reference/admin

- **pac copilot**
  
  Introduced a new --authoring-mode (-am) option for pac copilot init to choose between classic and cli-copilot authoring shapes. Removed the pac copilot init-skills command and its related documentation to streamline the command set. These changes clarify how to initialize agent authoring and reduce confusion around deprecated capabilities.  
  https://learn.microsoft.com/en-us/power-platform/developer/cli/reference/copilot

- **pac model**
  
  Introduced pac model genpage add and pac model genpage remove to attach or detach generative pages without re-uploading or deleting records. Expanded genpage list to support environment-wide listing by default, optional app scoping, and an --include-unpublished switch for drafts, with an environment option documented. Clarified genpage upload behavior for creating versus updating pages and referenced using genpage add to attach existing pages. Updated keywords to include the new verbs, improving discoverability and lifecycle management for generative pages.  
  https://learn.microsoft.com/en-us/power-platform/developer/cli/reference/model

## Moderate Changes

- **Recommendations for continuous performance optimization**
  
  Updated automated performance testing guidance to recommend Power Platform Playwright samples instead of Power Apps Test Engine. This broadens coverage from standalone canvas apps to all types of Power Apps.  
  https://learn.microsoft.com/en-us/power-platform/well-architected/performance-efficiency/continuous-performance-optimize

- **Microsoft Power Platform CLI Command Groups**
  
  Removed the (Deprecated) label from pac modelbuilder in the CLI reference table, indicating it is no longer deprecated. This signals continued support for the Dataverse code generator.  
  https://learn.microsoft.com/en-us/power-platform/developer/cli/reference/

- **Power Platform inventory schema reference**
  
  Added a known limitation explaining that built-in Power Automate actions (HTTP, Control, Data operations) are not connectors and will not appear in powerPlatformConnectors. This helps admins correctly interpret inventory data, especially when HTTP calls appear without a connector.  
  https://learn.microsoft.com/en-us/power-platform/admin/inventory-schema

- **Power Platform Playwright samples overview**
  
  Removed the advisory note positioning these samples as the recommended alternative to Power Apps Test Engine and removed the related See also link. The content now focuses on the samples without prescriptive comparisons while retaining the migration guide.  
  https://learn.microsoft.com/en-us/power-platform/developer/playwright-samples/overview

- **Recommendations for performance testing**
  
  Replaced references to Power Apps Test Engine with Power Platform Playwright samples. This aligns guidance to support testing across all types of Power Apps.  
  https://learn.microsoft.com/en-us/power-platform/well-architected/performance-efficiency/performance-test

- **Power Platform inventory**
  
  Expanded access requirements with a detailed Microsoft Entra roles table, clarifying full-visibility and AI-scoped roles, and noted that Power Platform RBAC roles are not supported for inventory access. Added a known issue where workflow agent flows from Microsoft 365 Copilot may lack environment information due to storage in a hidden tenant environment.  
  https://learn.microsoft.com/en-us/power-platform/admin/power-platform-inventory

- **Recommendations for designing a reliability testing strategy**
  
  Updated testing recommendations to use Power Platform Playwright samples instead of Power Apps Test Engine. This change extends testing guidance beyond standalone canvas apps to all Power Apps.  
  https://learn.microsoft.com/en-us/power-platform/well-architected/reliability/testing-strategy

- **pac tool**
  
  Documented a new pac tool init-skills subcommand to extract AI skill definition files. Included options to select skills and specify an output folder, making it easier to bootstrap skill assets.  
  https://learn.microsoft.com/en-us/power-platform/developer/cli/reference/tool

- **Power Platform developer tools**
  
  Removed the table entry for Power Apps Test Engine (preview), including its link and description. This streamlines the tools list and reflects current recommendations.  
  https://learn.microsoft.com/en-us/power-platform/developer/tools