# Dynamics 365 Customer Insights
**Date created:** 2026-09-01 UTC  
**Tags:** Best Practices, Configuration, Guidance, Performance  

## Major Changes

- **Understand automated segment refresh and data freshness**

  Substantially expanded guidance clarifies automated segment refresh intervals (introduced Feb 17, 2025) and how they apply to unused segments, active segments with or without behavioral data, and expired segments. It explains the mechanics of refresh (data sync vs. segment execution), where calculations occur (Dataverse vs. separate store), and how Dataverse sync latency impacts perceived freshness. The article adds best practices for timing journeys (one-time, dynamic, repeating), balancing execution time and interval, and improving freshness by reducing segment complexity/count, allowing sync time, setting custom intervals, and coordinating quiet times. This helps teams plan reliable activation schedules and make informed trade-offs between freshness and performance.

  https://learn.microsoft.com/en-us/dynamics365/customer-insights/journeys/auto-segment-management

- **Connect to Delta tables in Azure Data Lake Storage**

  Expanded support now includes Delta tables with minReaderVersion up to 3, enabling features such as deletion vectors, liquid clustering, and table features write, while keeping TimestampNTZ, type widening, and variant unsupported. The guidance clarifies how to lower the Delta protocol or disable features at the workspace level, and notes that existing tables can drop features to become compatible. Additional refinements improve advice on table selection, primary key selection, data profiling, schema change handling, and full refresh behavior to streamline ingestion and reduce integration issues.

  https://learn.microsoft.com/en-us/dynamics365/customer-insights/data/connect-delta-lake