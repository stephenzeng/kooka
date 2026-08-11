# Azure Monitor
**Date created:** 2026-08-11 UTC  
**Tags:** Automation, Best Practices, Billing, Configuration, Deprecation, Get Started, Guidance, Monitoring, Performance, Security, Troubleshooting  

## New Articles

- **Create an Azure Monitor health model by using Bicep (preview)**

  Introduced a step-by-step tutorial and full Bicep template for deploying an Azure Monitor health model, including entities, relationships for roll-up, and inline signals with thresholds. Provides deployment guidance via Azure CLI and PowerShell, with required parameters and managed identity, plus verification steps in CLI and the portal’s Graph view. Covers regional availability, evaluation latency expectations, and cleanup, enabling teams to quickly stand up repeatable, infrastructure-as-code health models.

  https://learn.microsoft.com/en-us/azure/azure-monitor/health-models/tutorial-bicep

## Major Changes

- **Azure Monitor Agent extension versions**

  Overhauled AMA release notes to emphasize a support policy focused on versions from the last year, clarified monthly cadence, and noted separate regional rollouts for Windows and Linux with release notes starting at rollout. Updated the version summary and added an Aug 2026 release for Linux 1.44 and Metrics 2.2026.703.954 with security dependency updates, CVE remediations, and support for Azure Linux 4, Rocky Linux 10, OTLP port overrides/disable via DCR, AKS workload identity for custom OTLP metrics, and GovSG. Improved metrics buffering and ingestion counters and fixed issues including rare transformed log corruption/loss, SELinux labeling for log rotation, syslog config regeneration, Metrics Extension policy reversion, and metric type attribute corrections.

  https://learn.microsoft.com/en-us/azure/azure-monitor/agents/azure-monitor-agent-extension-versions

- **Azure Monitor data platform**

  Restructured and expanded guidance for clarity, including a new comparison table of metrics vs. logs and refined sections on native metrics vs. Prometheus. Strengthened logs guidance, clarified distributed tracing with an emphasis on Application Insights, and streamlined related topics. Significantly updated the Changes section to reflect Change Analysis running on Azure Resource Graph with onboarding-free usage, plus new approaches to troubleshoot and query changes across subscriptions.

  https://learn.microsoft.com/en-us/azure/azure-monitor/fundamentals/data-platform

## Moderate Changes

- **Autoscale in Azure Monitor**

  Refined the overview structure, including renaming the schedule-based scaling section and elevating Predictive autoscale to its own section for better discoverability. Updated the Supported services list by removing Azure Media Services, helping readers avoid relying on a capability that’s no longer listed as supported.

  https://learn.microsoft.com/en-us/azure/azure-monitor/autoscale/autoscale-overview

- **Custom metrics in Azure Monitor (preview)**

  Added clear guidance to use the generally available OpenTelemetry-based approach via Application Insights (including VM system metrics) instead of native custom metrics. Clarified pricing and retention details, and refined best practices on auditing limits, avoiding variable metric names, and managing high-cardinality dimensions with associated cost impacts.

  https://learn.microsoft.com/en-us/azure/azure-monitor/metrics/metrics-custom-overview

- **Deep investigations in the Azure Copilot Observability Agent**

  Clarified that Investigate opens a Temporary chat automatically scoped to the triggering alert, with an initial message outlining the planned analysis and correlated signals. Noted that the agent requests more context or confirmation before proceeding, and removed references to Azure Agent Credit (AAC) and the Start chat button.

  https://learn.microsoft.com/en-us/azure/azure-monitor/aiops/observability-agent-deep-investigations

- **Azure Monitor REST API walkthrough**

  Retitled the article and standardized API paths, resource IDs, and examples, including corrected authentication steps and updated PowerShell example. Added a parameters reference table, corrected query details, and clarified multi-resource metrics queries with refreshed examples and troubleshooting to reduce errors in cross-resource scenarios.

  https://learn.microsoft.com/en-us/azure/azure-monitor/platform/rest-api-walkthrough