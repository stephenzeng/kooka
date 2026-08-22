# Microsoft Purview
**Date created:** 2026-08-22 UTC  
**Tags:** Best Practices, Billing, Compliance, Configuration, Deprecation, Get Started, Governance, Guidance, Monitoring, Security, Troubleshooting  

## New Articles

- **Best practices for on-demand classification on endpoints and billing**

  Added guidance to plan and run on-demand classification on Windows endpoints at scale. Clarifies the billing model (pay-as-you-go for actively classified files) and how previously classified results can be reused under defined conditions to control cost. Recommends approaches to improve estimation accuracy and throughput, including pilot runs, phased rollouts, batching, and handling offline devices. Highlights operational tips such as starting classification before estimation reaches 100%, maintaining a change-freeze on classifiers, and planning regular follow-up scans, with links to get started, monitoring, and FAQ content.

  https://learn.microsoft.com/en-us/purview/endpoints-best-practices

- **FAQ and reference for endpoint scans**

  Introduced a comprehensive FAQ covering feature behavior, costs, and operations for on-demand classification on Windows endpoints. Explains differences between classification and labeling, when rescans are needed, where to view usage, and how estimates can differ from actuals. Details device and results considerations (concurrency, excluded folders, unsupported platforms, and interpretation of items-for-review vs audit logs), notes current feature gaps, and links to related setup, best practices, and troubleshooting articles.

  https://learn.microsoft.com/en-us/purview/endpoints-faq-reference

- **Monitor and troubleshoot endpoint scans**

  Provided end-to-end guidance to monitor progress and resolve issues in endpoint scans. Defines key metrics and statuses for estimation and classification, explains skipped and failed files, and maps common symptoms to likely causes with recommended actions. Covers error categories (access, encryption, format, lock, I/O, system), expected discrepancies between estimation and results, agent downgrade considerations, and when to contact support, with pointers to related getting started, best practices, and FAQ resources.

  https://learn.microsoft.com/en-us/purview/endpoints-monitor-troubleshoot

- **Get started with on-demand classification for endpoints**

  Introduced the feature, its scope, and how it complements real-time Endpoint DLP. Provides a step-by-step workflow for creating scans (scope, classifiers, filters), running estimation and classification, and reviewing results, including prerequisites and required roles. Includes notes on device-level bandwidth throttling and links to best practices, monitoring/troubleshooting, and FAQ to accelerate successful rollout.

  https://learn.microsoft.com/en-us/purview/on-demand-classification-endpoints

## Major Changes

- **What's new in Microsoft Purview**

  Expanded July 2026 updates span labeling, governance, DLP, lifecycle, and shared capabilities. Data Governance introduces a deprecation: Purview protection policies no longer support Azure SQL Database, and adds guidance to configure manual BC/DR for Data Map. DLP gains a preview to detect classification failures in Exchange Online and refreshed Fabric governance experiences to surface DLP activity and adoption. Information Protection updates streamline auto-labeling with a pre-flight checklist, deeper troubleshooting, clearer rules for label removal/downgrade, licensing/configuration pointers, and group support details; lifecycle updates require three distinct approvers for priority cleanup policies; and access governance adds expiring role-group assignments with automatic revocation—improving control, clarity, and operational resilience.

  https://learn.microsoft.com/en-us/purview/whats-new