# Azure Monitor
**Date created:** 2026-08-27 UTC  
**Tags:** Configuration, Guidance, Monitoring, Troubleshooting  

## Moderate Changes

- **Enable private link for monitoring virtual machines and Kubernetes clusters in Azure Monitor**

  Clarified that OpenTelemetry-based metrics collection for virtual machines doesn’t support Private Link, and that the guidance applies to logs stored in Log Analytics workspaces. Added a link to metrics collection limitations to set expectations and prevent misconfiguration.

  https://learn.microsoft.com/en-us/azure/azure-monitor/fundamentals/private-link-vm-kubernetes

- **Tutorial: Create an Azure Monitor health model by using Bicep (preview)**

  Reworked deployment and verification to use Azure CLI with separate Bash and PowerShell tabs, replacing Azure PowerShell examples. Added a Git Bash on Windows tip (set MSYS_NO_PATHCONV=1) to avoid path conversion issues, switched verification to az monitor health-models entity show, and standardized parameter quoting.

  https://learn.microsoft.com/en-us/azure/azure-monitor/health-models/tutorial-bicep

- **Analyze the health and status of your virtual machine with Azure Monitor**

  Updated the note to remove preview language for the OpenTelemetry-based metrics experience and to reference the renamed article. This improves clarity on availability and directs readers to the current guidance.

  https://learn.microsoft.com/en-us/azure/azure-monitor/vm/vminsights-performance

- **Migrate from logs-based to OpenTelemetry metrics for Azure virtual machines**

  Removed the preview disclaimer to reflect the updated status of the metrics-based experience. The migration guidance remains unchanged, signaling readiness for broader adoption.

  https://learn.microsoft.com/en-us/azure/azure-monitor/vm/vm-opentelemetry-migrate