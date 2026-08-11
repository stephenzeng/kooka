# Microsoft Fabric
**Date created:** 2026-08-11 UTC  
**Tags:** Analytics, Billing, Configuration, Consumption, Deprecation, Governance, Guidance, Performance  

## New Articles

- **Resource profiles in Microsoft Fabric overview**

  Introduced Spark resource profiles that apply tested Spark and Delta Lake configurations for common workloads, with writeHeavy as the default workspace profile. Explained how to select a profile via spark.fabric.resourceProfile and enable profile-specific auto-updates with spark.fabric.resourceProfile.<profileName>AutoUpdate, which refresh tuned values without changing pool size or autoscale. Detailed profile optimization targets and V-Order defaults, and provided guidance on when to use each profile (for example, Power BI/DirectLake scenarios).

  https://learn.microsoft.com/en-us/fabric/data-engineering/resource-profiles-overview

- **Measure Model for Planning**

  Introduced the Measure Model as a semantic enrichment framework that treats existing DAX measures as baselines and lets users extend them with visual measures—without changing backend code. Described benefits such as hierarchical measure organization, measure-level simulations, and cascading impact visualization that keeps actuals and forecasts aligned. Presented a no-code planning approach for business users with a practical example bringing Revenue Actuals and Forecasts together.

  https://learn.microsoft.com/en-us/fabric/iq/plan/planning-concept-measure-model

- **Statistical Forecasting Algorithms in Predict**

  Added an overview of forecasting algorithms available in Predict, including MSTL trend decomposition, the Exponential Smoothing family (with parameter optimization), and ARIMA/SARIMA with Auto ARIMA selection. Provided examples of model orders and a selection guide to help choose the right approach based on seasonality, trend, and data characteristics. Helps practitioners match algorithms to business scenarios for more accurate forecasts.

  https://learn.microsoft.com/en-us/fabric/iq/plan/planning-concept-predict

## Moderate Changes

- **Develop, execute, and manage Microsoft Fabric notebooks**

  Added instructions for running a selection of code within a cell, including steps, a screenshot, and notes on variable and import availability. Updated the keyboard shortcuts to include Ctrl+Shift+Enter for running selected code, improving interactive development efficiency.

  https://learn.microsoft.com/en-us/fabric/data-engineering/author-execute-notebook

- **Use partitioned compute in Dataflow Gen2 (Preview)**

  Clarified billing behavior for partitioned runs: parallel execution reduces wall-clock time, but each partition accrues capacity units for its own processing duration, which can lead to similar or higher total CU than sequential runs. Included a link to Dataflow Gen2 pricing to support cost planning.

  https://learn.microsoft.com/en-us/fabric/data-factory/dataflow-gen2-partitioned-compute

- **Fabric data agent Python SDK (preview)**

  Updated migration guidance for querying data agents: begin moving from the OpenAI Assistants API to the OpenAI Responses API starting August 11, 2026, ahead of Assistants API deprecation on August 26, 2026. Only querying code changes; creation, configuration, and publishing remain the same to minimize disruption.

  https://learn.microsoft.com/en-us/fabric/data-science/fabric-data-agent-sdk

- **Delivery guarantees for Business, Fabric, and Azure Events**

  Clarified at-least-once delivery with a defined 24-hour retry window from event generation. Reinforced that duplicates and out-of-order events can occur and that consumers should implement deduplication and ordering safeguards.

  https://learn.microsoft.com/en-us/fabric/real-time-hub/fabric-event-delivery-guarantees

- **Native execution engine for Fabric Data Engineering**

  Expanded limitations to distinguish behavior across runtimes, noting several correctness issues resolved in Runtime 2.0 (Apache Spark 4.1) and clarifying ANSI SQL mode support (unsupported on 1.3, supported on 2.0). Refined details on function behaviors and configuration errors specific to Runtime 1.3, and clarified that separate managed private endpoints are required for Blob and DFS when NEE is enabled.

  https://learn.microsoft.com/en-us/fabric/data-engineering/native-execution-engine-overview

- **Workspace administration settings in Microsoft Fabric**

  Added a setting to cap maximum Spark job lifetime, with guidance on enabling it and specifying duration. Clarified which user-submitted jobs are affected and which system-managed operations are excluded, and noted that jobs are automatically cancelled when the limit is reached.

  https://learn.microsoft.com/en-us/fabric/data-engineering/workspace-admin-settings