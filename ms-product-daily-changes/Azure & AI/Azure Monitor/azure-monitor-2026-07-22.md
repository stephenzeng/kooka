# Azure Monitor
**Date created:** 2026-07-22 UTC  
**Tags:** Monitoring  

## Major Changes

- **Signals in Azure Monitor health models (preview)**

  Introduced Azure Resource Health as a new signal type, allowing platform health to directly influence an entity’s health state. Added Dynamic thresholding for Azure resource signals with settings for Threshold type, Sensitivity, and Lookback window to adapt to normal patterns and seasonality. Guidance and UI updates explain how to enable Resource Health in the entity editor and how dynamic thresholds behave, improving accuracy and reducing manual tuning.

  https://learn.microsoft.com/en-us/azure/azure-monitor/health-models/signals

## Moderate Changes

- **Analyze health state of Azure Monitor health models (Preview)**

  Added “Data annotations” to show contextual notes on the health timeline as markers or in the entity details pane. Clarified that annotations must be added programmatically and provided CLI guidance using az monitor health-models entity add-data-annotation.

  https://learn.microsoft.com/en-us/azure/azure-monitor/health-models/analyze-health

- **Azure Monitor health model concepts**

  Introduced “Dynamic thresholds,” which use machine learning baselines instead of static limits and support lookback window and sensitivity tuning. Documented fallback behavior during warm-up or missing data and where to configure dynamic thresholds in the designer.

  https://learn.microsoft.com/en-us/azure/azure-monitor/health-models/concepts

- **Configure signals in an Azure Monitor health model (preview)**

  Expanded configuration steps for metric signals to use Dynamic thresholds, including how to set Threshold type and tune Sensitivity and Lookback window. Clarified Unknown status behavior for metrics and charts when there’s no traffic, with a reference to the dynamic thresholds guidance.

  https://learn.microsoft.com/en-us/azure/azure-monitor/health-models/tutorial-signals

- **Dependency Agent in Azure Monitor VM insights**

  Expanded uninstallation guidance with version-specific steps. For Windows, detailed the correct uninstaller and noted signature differences on older versions; for Linux, added instructions for the provided script (newer versions) and package manager commands for Debian/Ubuntu and RPM-based distros (earlier versions).

  https://learn.microsoft.com/en-us/azure/azure-monitor/vm/vminsights-dependency-agent

- **VM Insights Map and Dependency Agent retirement guidance**

  Added a Log Analytics query to find Dependency Agent installations, classify resource types, generate portal links, and flag outdated versions. Linked to detailed Windows and Linux manual removal steps to streamline cleanup and migration.

  https://learn.microsoft.com/en-us/azure/azure-monitor/vm/vminsights-maps-retirement