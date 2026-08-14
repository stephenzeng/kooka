# Azure Monitor
**Date created:** 2026-08-14 UTC  
**Tags:** Configuration, Guidance, Monitoring, Security  

## Moderate Changes

- **Azure Monitor Agent extension versions**
  
  Updated the release matrix to add Windows AMA 1.45 alongside Linux 1.44 and refreshed the version highlights. Added release notes detailing security updates (including OpenSSL 3.6.3 and a newer Metrics Extension), improved on-disk buffering reliability, reduced token refresh activity, and fixes for early startup and logging initialization crashes. These changes improve security posture and operational stability.
  
  https://learn.microsoft.com/en-us/azure/azure-monitor/agents/azure-monitor-agent-extension-versions

- **Azure Monitor Logs overview**
  
  Renamed the “Auxiliary” table plan to “Auxiliary / Lake” and refined supported table type descriptions to align with Basic and Auxiliary/Lake plans. Clarified plan naming and applicability without changing capabilities or retention. This helps align terminology with current offerings and reduces confusion when selecting plans.
  
  https://learn.microsoft.com/en-us/azure/azure-monitor/logs/data-platform-logs

- **Monitor AKS applications with OTLP and Azure Monitor (Preview)**
  
  Expanded protocol support to include OTLP/gRPC with binary Protobuf in addition to OTLP/HTTP, while clarifying that JSON payloads aren’t supported. This enables broader interoperability for telemetry ingestion without relying on JSON.
  
  https://learn.microsoft.com/en-us/azure/azure-monitor/containers/kubernetes-open-protocol

- **Logs Ingestion API in Azure Monitor**
  
  Simplified the Supported tables guidance by removing the embedded exhaustive list and linking to the centralized “Azure Monitor Logs table feature support” reference. Clarified that the target table must exist before ingestion and that custom tables must use the _CL suffix. This streamlines setup and reduces maintenance overhead for documentation consumers.
  
  https://learn.microsoft.com/en-us/azure/azure-monitor/logs/logs-ingestion-api-overview