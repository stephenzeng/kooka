# Power Platform
**Date created:** 2026-08-19 UTC  
**Tags:** Analytics, Automation, Best Practices, Configuration, Consumption, Governance, Guidance, Licensing, Monitoring, Performance, Security  

## New Articles

- **Connect Power Apps to a centralized data warehouse with Dataverse virtual tables**

  Introduced a new reference architecture showing how to use Dataverse virtual tables to surface read-only warehouse data alongside editable Dataverse records in Power Apps. The article includes an end-to-end workflow, architecture diagram, and component overview spanning Azure SQL, Dataverse, Power Apps, and Power Automate. It details operational, security, performance, and ALM considerations, with guidance on minimizing datasets, scoping access, and using pipelines. Related resources help teams implement virtual tables and integrate with broader data platforms.

  https://learn.microsoft.com/en-us/power-platform/architecture/reference-architectures/power-apps-virtual-tables

## Moderate Changes

- **Dataverse capacity-based storage details**

  Clarified how capacity notifications and overage status differ from the validation used for environment lifecycle operations. Updated guidance emphasizes that operations like create, copy, restore, recover, convert, and adding a Dataverse database require sufficient available Database, File, or Log capacity for the specific type, regardless of tenant-level effective capacity.

  https://learn.microsoft.com/en-us/power-platform/admin/capacity-storage

- **Overview of Power Platform and Copilot Studio reference architectures**

  Added a new entry highlighting how to connect Power Apps to a centralized data warehouse using Dataverse virtual tables. This expands the catalog with an integration pattern for accessing enterprise data without moving or duplicating it.

  https://learn.microsoft.com/en-us/power-platform/architecture/reference-architectures/

- **Microsoft Dataverse reference architectures and solution ideas**

  Expanded the solution ideas by adding a design that connects to a centralized data warehouse through Dataverse virtual tables. This helps teams integrate read-only enterprise data into app experiences while maintaining Dataverse for transactional records.

  https://learn.microsoft.com/en-us/power-platform/architecture/products/microsoft-dataverse

- **Power Apps reference architectures and solution ideas**

  Added a scenario for using Dataverse virtual tables to work with centralized enterprise data in Power Apps. The entry guides when to leverage virtual tables to keep warehouse data authoritative while building app experiences in Dataverse.

  https://learn.microsoft.com/en-us/power-platform/architecture/products/power-apps

- **View security recommendations**

  Introduced a security recommendation for Power Pages to renew website authentication keys before they expire to prevent downtime. The recommendation (High severity, refreshed daily, managed environments) identifies sites with expired or soon-to-expire keys and notes it can take up to a day for resolved items to clear.

  https://learn.microsoft.com/en-us/power-platform/admin/security-recommendations

- **Dataverse capacity-based storage overview**

  Retitled a section to “Storage reporting optimization,” clarified that legacy licensing customers won’t see the optimized capacity report, and refined guidance on how lifecycle operations are evaluated. The update stresses that operations depend on available capacity within each storage type (Database, File, Log), not on cross-type borrowing, helping admins understand when actions may be blocked.

  https://learn.microsoft.com/en-us/power-platform/admin/whats-new-storage