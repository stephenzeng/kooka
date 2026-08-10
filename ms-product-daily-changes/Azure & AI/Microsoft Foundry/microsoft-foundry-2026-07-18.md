# Microsoft Foundry
**Date created:** 2026-07-18 UTC  
**Tags:** AI, Administration, Agent, Programming, Security  

## Moderate Changes

- **Build with agents, conversations, and responses**
  
  Updated code samples to use newer SDK versions (JavaScript @azure/ai-projects 2.3.0; Java azure-ai-agents 2.2.0 and azure-identity 1.18.4). The Java memory store example now uses the beta client (BetaMemoryStoresClient) and corresponding beta() builder to reflect current APIs and improve alignment with preview features.
  
  https://learn.microsoft.com/en-us/azure/foundry/agents/concepts/runtime-components

- **Configure Customer-Managed Keys for Azure AI Search**
  
  Clarified how to manage service-level versus object-level CMK, including using PUT to set object-level keys, defaulting to service-level inheritance on create, and switching back via isServiceLevelKey = true. Documented 2026-05-01-preview validation rules and explained that when isServiceLevelKey is true, provided key fields are ignored for selection; examples and guidance now recommend including service-level fields and verifying the effective key via GET.
  
  https://learn.microsoft.com/en-us/azure/search/search-security-manage-encryption-keys

- **Create and use memory in Foundry Agent Service (preview)**
  
  Updated Java samples to use the beta Memory Stores client (BetaMemoryStoresClient) with the beta() builder and buildBetaMemoryStoresClient(). This aligns the guidance with current preview APIs and helps developers avoid compile-time mismatches.
  
  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/memory-usage

- **File search tool for agents**
  
  Bumped the Java Maven dependency for com.azure:azure-ai-agents from 2.0.0 to 2.2.0. This ensures developers use the latest SDK features and fixes in code examples.
  
  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/tools/file-search

- **Foundry Agent Service limits, quotas, and regional support**
  
  Expanded the Responses API regional support table to include Switzerland West and West Central US. This helps teams plan deployments in newly supported regions.
  
  https://learn.microsoft.com/en-us/azure/foundry/agents/concepts/limits-quotas-regions

- **Hosted agent permissions reference**
  
  Clarified that the UserIdentityImpersonation data action is not included in built-in roles and now requires a custom role. Added a ready-to-use custom role JSON and Azure CLI steps to create and assign it to the middle-tier identity; calls lacking this permission return 403, ensuring correct role configuration is enforced.
  
  https://learn.microsoft.com/en-us/azure/foundry/agents/concepts/hosted-agent-permissions

- **How to configure network isolation for Microsoft Foundry**
  
  Updated firewall allowlisting guidance to support service tags alongside FQDNs. For Agents, use the AAD service tag; for Evaluations & Traces with Application Insights, added required endpoints and the AzureMachineLearning service tag and removed the blob storage FQDN, clarifying how results flow to Application Insights and the Evaluators Catalog.
  
  https://learn.microsoft.com/en-us/azure/foundry/how-to/configure-private-link

- **Isolate hosted agent sessions per user**
  
  Clarified that the UserIdentityImpersonation data action is not granted by built-in roles or broad wildcards and must be explicitly included in a custom role assigned to the calling service. Troubleshooting now directs resolving 403 errors (with x-ms-user-identity) by creating and assigning the custom role that includes the required data action.
  
  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/isolate-sessions-per-user

- **Migrate to the new agents developer experience**
  
  Updated SDK versions and guidance: JavaScript @azure/ai-projects to 2.3.0, Java azure-ai-agents to 2.2.0, and azure-identity to 1.18.4. Troubleshooting now recommends these minimum versions and provides streamlined install instructions, helping developers avoid compatibility issues during migration.
  
  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/migrate

- **Microsoft Foundry SDKs and Endpoints**
  
  Simplified JavaScript installation instructions by removing @azure/identity from the required packages. Projects now list @azure/ai-projects and dotenv only, reducing unnecessary dependencies.
  
  https://learn.microsoft.com/en-us/azure/foundry/how-to/develop/sdk-overview

- **Publish your agent as an Agent Application**
  
  Removed the Foundry portal publishing section, deprecating the portal-based flow and related steps (RBAC configuration, tool permissions, and sharing). Guidance now focuses on the REST API publishing approach to streamline and standardize deployment.
  
  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/agent-applications