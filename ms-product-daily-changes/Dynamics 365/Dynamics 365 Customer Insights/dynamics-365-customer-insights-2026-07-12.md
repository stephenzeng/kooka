# Dynamics 365 Customer Insights
**Date created:** 2026-07-12 UTC  
**Tags:** Agent  

## Major Changes

- **Customer Insights MCP server tools reference (preview)**

  Updated the msdynci_getclusterinformation tool to report only cluster membership, replacing references to enrichment datasets with the unified customer profile source. Clarified the definition of clusters as post-unification rules (for example, households) and aligned related workflow references and tool lists accordingly. This change removes ambiguity between enrichment data and cluster membership. The result is clearer guidance and more consistent outputs for scenarios that depend on cluster logic.

  https://learn.microsoft.com/en-us/dynamics365/customer-insights/data/mcp-server-tools-reference

## Moderate Changes

- **Use tools in the Customer Insights MCP Server (preview)**

  Expanded the Scenario section into a structured, multi-step walkthrough with named personas to illustrate how an agent gains access to the MCP server. The narrative now demonstrates lead-contact matching, unified profiles across Dynamics 365 and external sources, and how prompts surface insights like webinar interests, contract details, CLV, churn risk, and segment membership. This improves practical understanding of the end-to-end flow and how to use the server’s unified insights in real conversations.

  https://learn.microsoft.com/en-us/dynamics365/customer-insights/data/mcp-server-tools