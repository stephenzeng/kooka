# Azure Monitor
**Date created:** 2026-07-28 UTC  
**Tags:** Administration, Agent, Governance, Monitoring, Programming, Security  

## Major Changes

- **Add or Delete Tables and Columns in Azure Monitor Logs**
  
  Substantially expanded guidance for creating and managing custom tables and columns across Analytics, Basic, and Auxiliary/Lake plans with end-to-end examples for Azure CLI, REST, PowerShell, ARM, and Bicep. Clarified plan selection, required _CL suffix, and billing implications for table names, plus prerequisites including ISO 8601 with microsecond precision for Auxiliary/Lake TimeGenerated. Reworked portal workflow, clarified transformation editor behavior, and linked to sample data. Enhanced deletion and schema operations with concrete payloads, including full PUT semantics and actions to add, replace, or remove columns.
  
  https://learn.microsoft.com/en-us/azure/azure-monitor/logs/create-custom-table

- **Send virtual machine client data to Event Hubs and Storage (Preview)**
  
  Overhauled and then clarified retirement and alternatives guidance for sending VM client data to Event Hubs and Storage. Documented that creating new data collection rules stops in February 2026 and the feature retires July 31, 2026; recommended using Azure Monitor Logs with data export to Event Hubs and updating AMA configurations to write to custom tables on the Auxiliary plan for Storage scenarios. Removed earlier guidance on VM Watch and direct routes to ADX/Fabric, and corrected an ARM template parameter type from String to string to prevent deployment errors. These changes set clear paths for migration and ensure configurations align with supported options.
  
  https://learn.microsoft.com/en-us/azure/azure-monitor/vm/send-event-hubs-storage

- **Dependency Agent in Azure Monitor VM insights**
  
  Refocused the article on deprecation and uninstallation instead of installation or upgrades. Clarified requirements, supported OSes, and data ingestion behavior, and discouraged new installations. Strengthened Linux-specific notes, including kernel taint behavior and installation restrictions, and linked to guidance for identifying VMs still using the Dependency Agent.
  
  https://learn.microsoft.com/en-us/azure/azure-monitor/vm/vminsights-dependency-agent

## Moderate Changes

- **Azure Monitor Agent extension versions**
  
  Updated July 2026 release details, adding Windows agent version 1.44 and Metrics Extension 2.2026.617.1755. Highlighted CEF parsing improvements, OpenSSL 3.6.3, and expanded guidance with a Windows-specific subsection; the versions summary now covers both Linux and Windows for clearer parity and security awareness.
  
  https://learn.microsoft.com/en-us/azure/azure-monitor/agents/azure-monitor-agent-extension-versions

- **Azure Monitor Logs**
  
  Added a table-based feature comparison across Analytics, Basic, and Auxiliary plans, including new rows for Resource query scope, Customer lockbox, and Workspace replication. Consolidated prior Auxiliary limitations into the comparison and simplified export guidance by removing on-demand export job (preview), helping readers choose the right plan and export approach.
  
  https://learn.microsoft.com/en-us/azure/azure-monitor/logs/data-platform-logs

- **Log query scope in Azure Monitor Log Analytics**
  
  Introduced a new restriction: queries are blocked when the scope includes tables in the Basic or Auxiliary plans because they only support workspace-scope queries. This clarifies expected behavior and helps avoid failed cross-scope queries.
  
  https://learn.microsoft.com/en-us/azure/azure-monitor/logs/scope

- **Remove Dependency Agent from Azure Virtual Machines and Virtual Machine Scale Sets**
  
  Clarified that manually installed Dependency Agents don’t appear as VM extensions and provided a Log Analytics query method to find them. Added instructions for manually removing standalone installations with links to Windows and Linux uninstall procedures, streamlining cleanup.
  
  https://learn.microsoft.com/en-us/azure/azure-monitor/vm/vminsights-dependency-agent-uninstall

- **VM Insights Map and Dependency Agent retirement guidance**
  
  Expanded retirement guidance with steps to identify affected resources via Azure Advisor and included applicable resource types. Added migration guidance for policy/initiative assignments, a FAQ covering monitoring impact and retention, and a Support section to direct customers to personalized recommendations and help channels.
  
  https://learn.microsoft.com/en-us/azure/azure-monitor/vm/vminsights-maps-retirement