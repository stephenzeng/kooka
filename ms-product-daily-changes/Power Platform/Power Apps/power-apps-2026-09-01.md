# Power Apps
**Date created:** 2026-09-01 UTC  
**Tags:** Best Practices, Deprecation, Governance, Guidance  

## Major Changes

- **Frequently asked questions when transitioning from legacy data integration services to Fabric link and Azure Synapse Link for Dataverse**

  Clarified that the retirement applies only to the legacy Export to Data Lake environment add-in, not to Link to Fabric or Azure Synapse Link for Dataverse. Set a firm service stop date of November 30, 2026, with no extensions, while confirming existing Link to Fabric profiles remain supported. Removed outdated decommissioning timelines and past-due extension guidance. Expanded uninstall steps to note no downtime or restarts, progressive CDC disablement, and that existing lake files remain accessible.

  https://learn.microsoft.com/en-us/power-apps/maker/data-platform/azure-synapse-link-transition-FAQ

## Moderate Changes

- **Transition from legacy data integration services**

  Updated guidance to prioritize Link to Microsoft Fabric with low-latency sync, and clarified that Azure Synapse Link is recommended when exporting to your own storage account. Reorganized integration options and refined decision criteria to simplify choosing the right path.

  https://learn.microsoft.com/en-us/power-apps/maker/data-platform/azure-synapse-link-transition-from-FnO

- **Best practices: Collaborating and co-developing apps using Power Apps**

  Expanded best practices to cover comments, copresence, real-time coauthoring, component libraries, code components, solutions, source control, and ALM. Refined the overview of low-code platform capabilities and repositioned Dataverse as a secure cloud data platform for fusion teams, while removing outdated examples.

  https://learn.microsoft.com/en-us/power-apps/guidance/co-develop/overview

- **Responsive design guidelines in Power Apps**

  Clarified responsive design guidance by recommending horizontal and vertical auto-layout containers as the primary layout approach. Advised disabling Scale to Fit, managing aspect ratio and orientation, using formulas over fixed positions, and following a systematic process to convert nonresponsive apps for consistent experiences across devices and input modes.

  https://learn.microsoft.com/en-us/power-apps/guidance/coding-guidelines/responsive-design-guidelines