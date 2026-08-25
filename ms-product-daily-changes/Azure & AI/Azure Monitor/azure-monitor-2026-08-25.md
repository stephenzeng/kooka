# Azure Monitor
**Date created:** 2026-08-25 UTC  
**Tags:** Best Practices, Configuration, Get Started, Guidance, Monitoring  

## New Articles

- **Add data annotations to Azure Monitor health models (preview)**

  Introduced a how-to guide for using data annotations with health models, including prerequisites and installing the Azure CLI health-models extension. Provides step-by-step commands (Bash and PowerShell) to add annotations with key-value details and descriptions, plus examples to filter and retrieve annotations for entities. Explains how to view annotations in the Azure portal and how they appear on health timelines. This helps teams capture operational context, correlate events with health signals, and accelerate troubleshooting.

  https://learn.microsoft.com/en-us/azure/azure-monitor/health-models/data-annotations

- **Health modeling with Azure Monitor health models (preview)**

  Added a conceptual article outlining a commitment-first approach that links customer outcomes to workload components and telemetry. Covers core concepts including entities and relationships, signal sources (metrics, logs, PromQL, Resource Health, external), health states, impact and dependency propagation, discovery methods, and visualization (Graph, Timeline, Entity details). Describes alerting on health state changes and includes a detailed example to illustrate modeling commitments and dependencies. This guidance helps teams align monitoring to business outcomes, focus alerts on customer impact, and build actionable health models.

  https://learn.microsoft.com/en-us/azure/azure-monitor/health-models/health-modeling

## Moderate Changes

- **Use the Azure CLI (preview)**

  Streamlined the annotations guidance by removing lengthy CLI and PowerShell walkthroughs and pointing readers to a dedicated procedure article. The page now focuses on conceptual guidance and portal timeline context, reducing duplication and helping readers find task-focused instructions more efficiently.

  https://learn.microsoft.com/en-us/azure/azure-monitor/health-models/cli

- **Create a new Azure Monitor health model (preview)**

  Updated the introduction to emphasize defining customer commitments and workload outcomes before building a health model, with links to dedicated modeling guidance. This improves planning and ensures models are aligned to business goals, while the article continues to cover creation in the Azure portal.

  https://learn.microsoft.com/en-us/azure/azure-monitor/health-models/create