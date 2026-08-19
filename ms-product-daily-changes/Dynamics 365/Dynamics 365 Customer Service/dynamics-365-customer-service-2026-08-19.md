# Dynamics 365 Customer Service
**Date created:** 2026-08-19 UTC  
**Tags:** Configuration, Get Started, Guidance, Security  

## New Articles

- **Overview of Dynamics 365 Workforce Management MCP tools**

  Introduced an overview of Model Context Protocol (MCP) tools that connect Service Agent with Dynamics 365 Customer Service and Dataverse. Explains common scenarios such as viewing workforce requests, accessing request details and context, handling supervisor approvals and rejections for time-off, and providing role-aware responses. Outlines personas (customer service representatives, supervisors, and MCP app/agent developers) and clarifies security via Dynamics 365 and Dataverse RBAC, including reviewer permissions and non-overwrite behavior for already decided requests. Details available tools and capabilities: list_wem_requests for filtering requests, get_wem_request_details for full context, and decide_wem_time_off_request to approve or reject time-off with reviewer and reason recorded.

  https://learn.microsoft.com/en-us/dynamics365/customer-service/develop/workforce-mcp-tools-overview-service-agent

## Moderate Changes

- **Connect Dynamics 365 CX MCP Server - Service through Agent 365 Tooling Gateway**

  Updated configuration guidance to standardize on a single gateway host (agent365.svc.cloud.microsoft) and a unified Microsoft Entra app ID, replacing ring-specific hosts, app IDs, and URLs. Simplified OAuth scope and admin consent guidance and refreshed configuration samples for multiple MCP clients, reducing setup complexity and preventing environment-specific misconfigurations.

  https://learn.microsoft.com/en-us/dynamics365/customer-service/develop/connect-agent-model-context-protocol