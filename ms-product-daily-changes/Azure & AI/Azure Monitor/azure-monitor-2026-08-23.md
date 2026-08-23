# Azure Monitor
**Date created:** 2026-08-23 UTC  
**Tags:** Configuration, Get Started, Guidance, Monitoring  

## New Articles

- **Submit data for externally evaluated signals**

  Introduced a how-to article for the Health Report Ingestion API (preview) that enables submitting externally evaluated health signals to Azure Monitor health model entities. Provides setup steps, including prerequisites and installing the health-models Azure CLI extension, plus example CLI/PowerShell commands to ingest reports with evaluation rules, TTL, and context. Explains how to verify entity and signal state via queries, maintain freshness by resubmitting, and understand expiration and health propagation within the model. Includes links to related conceptual and CLI documentation for end-to-end implementation.

  https://learn.microsoft.com/en-us/azure/azure-monitor/health-models/health-report-ingestion

## Moderate Changes

- **Signals in Azure Monitor health models (preview)**

  Added a new External health signal type to support signals evaluated by applications or other monitoring systems. This clarifies how to represent and ingest third-party or custom health inputs and links to guidance for submitting the data.

  https://learn.microsoft.com/en-us/azure/azure-monitor/health-models/signals