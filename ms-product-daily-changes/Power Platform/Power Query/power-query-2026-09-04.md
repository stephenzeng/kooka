# Power Query
**Date created:** 2026-09-04 UTC  
**Tags:** Automation, Best Practices, Configuration, Deprecation, Guidance, Licensing, Troubleshooting  

## Major Changes

- **Dataflow storage options**

  Announced deprecation of Bring Your Own Lake (customer-owned Azure Data Lake Storage) for analytical Power Platform dataflows effective October 31, 2026. Existing BYOL dataflows continue to run, but new analytical dataflows should use the managed data lake or standard dataflows with Dataverse where appropriate. Updated configuration guidance remains applicable until the deprecation date to help teams plan transitions and avoid disruption.

  https://learn.microsoft.com/en-us/power-query/dataflows/configuring-storage-and-compute-options-for-analytical-dataflows

- **Connect Azure Data Lake Storage Gen2 for dataflow storage**

  Added a deprecation notice that new analytical Power Platform dataflows writing to customer-owned ADLS via BYOL won’t be allowed after October 31, 2026. Clarified that existing BYOL dataflows continue and historical CSV files remain accessible, with guidance to connect via ADLS Gen2 or Azure Blob Storage connectors. Recommended using managed data lake for new analytical dataflows or standard dataflows with Dataverse, noting the time-bounded ability to create BYOL dataflows until the cutoff date.

  https://learn.microsoft.com/en-us/power-query/dataflows/connect-azure-data-lake-storage-for-dataflow

- **Create and use dataflows in Microsoft Power Platform**

  Introduced the BYOL deprecation timeline for analytical Power Platform dataflows, ending creation of new BYOL dataflows on October 31, 2026 while allowing existing ones to continue. Updated comparisons and guidance to steer new scenarios to managed data lake or standard dataflows with Dataverse. Announced retirement of referenced linked entities: creation disabled September 1, 2026 and existing ones stop on October 31, 2026, with migration steps to copy consuming dataflows, validate refresh, and replace cascade refresh with separate schedules or Power Automate orchestration.

  https://learn.microsoft.com/en-us/power-query/dataflows/create-use

- **Link tables between dataflows**

  Announced retirement of referenced linked entities for Power Platform dataflows: creation disabled September 1, 2026 and existing usages stop on October 31, 2026. Provided a migration path by copying the consuming dataflow to convert references, validating refresh, and deleting the old dataflow. Noted that this change doesn’t affect Power BI dataflows and that cascade refresh and dependency/delete validation are not available with standard references, recommending separate refresh schedules or Power Automate orchestration.

  https://learn.microsoft.com/en-us/power-query/dataflows/linked-tables

- **Using the output of Power Platform dataflows from other Azure data workloads**

  Announced that creating new analytical Power Platform BYOL dataflows won’t be allowed after October 31, 2026; existing BYOL dataflows continue and their CSV outputs remain accessible. Clarified that those outputs can still be consumed via ADLS Gen2 or Azure Blob Storage connectors. Recommended using managed data lake for new analytical dataflows or standard dataflows backed by Dataverse to ensure continuity.

  https://learn.microsoft.com/en-us/power-query/dataflows/using-output-power-platform-dataflows-other-azure

- **Consume data from dataflows**

  Added deprecation for creating new analytical Power Platform BYOL dataflows after October 31, 2026, with existing BYOL dataflows continuing and CSVs remaining available. Clarified consumption behavior: depending on host and storage, consumption creates either a linked table with coordinated refresh or a standard Dataflows connector reference that reads the latest upstream data without cascade refresh. Announced retirement of referenced linked entities with dates and provided migration guidance, including copying consuming dataflows, validating refresh, and orchestrating schedules or using Power Automate.

  https://learn.microsoft.com/en-us/power-query/dataflows/using-the-output-of-power-platform-dataflows

- **What licenses do you need to use dataflows**

  Updated licensing and capability guidance to reflect the BYOL deprecation timeline: new BYOL creation ends October 31, 2026, with existing BYOL dataflows continuing thereafter. Revised tables to indicate customer-provided storage is limited to existing BYOL dataflows after the cutoff and to note the shift to standard Dataflows connector references as referenced linked entities retire on October 31, 2026. Added migration guidance and clarified distinctions between Power BI and Power Platform dataflows in the ADLS context.

  https://learn.microsoft.com/en-us/power-query/dataflows/what-licenses-do-you-need-in-order-to-use-dataflows

## Moderate Changes

- **Transition from ODBC to ADBC drivers in Power BI and Fabric**

  Introduced the pq-adbc-advisor workspace audit tool, outlining its impact reporting, risk classifications, covered assets, and limitations, with step-by-step instructions for running tenant-wide audits in Fabric. Updated the migration checklist to start with auditing using pq-adbc-advisor and expanded the FAQ to help locate remaining legacy ODBC usage.

  https://learn.microsoft.com/en-us/power-query/transition-to-adbc

- **Understanding the differences between dataflow types**

  Updated policy and timelines for analytical dataflows storage, clarifying that Power BI can use customer-provided ADLS and that existing Power Platform BYOL dataflows continue while new BYOL creation ends October 31, 2026. Recommended Dataverse-managed analytical storage for new Power Platform scenarios and aligned the comparison table to reflect these storage options.

  https://learn.microsoft.com/en-us/power-query/dataflows/understanding-differences-between-analytical-standard-dataflows