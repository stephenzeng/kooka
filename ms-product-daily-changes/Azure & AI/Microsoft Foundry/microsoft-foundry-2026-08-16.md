# Microsoft Foundry
**Date created:** 2026-08-16 UTC  
**Tags:** Best Practices, Billing, Configuration, Consumption, Guidance, Monitoring, Security  

## New Articles

- **Network isolation for a toolbox in Microsoft Foundry**
  
  Introduced a how-to guide explaining how toolbox tool traffic flows when a project uses network isolation. Clarifies that a toolbox inherits the project’s networking and details connectivity patterns by tool type, including private endpoints, VNet subnet integration, and Microsoft backbone/public endpoints. Highlights unsupported or partially supported tools and includes a support matrix to set expectations. Provides step-by-step guidance and infrastructure-as-code templates for securing projects, including options for private endpoints and no public egress. Links to the authoritative tool-by-tool matrix and related networking documentation to aid planning and deployment.
  
  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/tools/toolbox-network-isolation

## Moderate Changes

- **Claude Consumption Units (CCU) billing in Microsoft Foundry**
  
  Reorganized guidance on where to view pricing, usage, and costs across Azure Cost Management, the Foundry portal Pricing tab, the Foundry Monitor tab, and Azure Marketplace private offers. Clarifies that the Monitor tab is for operational per-model usage, estimated-cost charts apply only to CCU-based deployments, private-offer discounts aren’t reflected in estimates, and invoices/Azure Cost Management remain the source of truth for billed cost.
  
  https://learn.microsoft.com/en-us/azure/foundry/foundry-models/concepts/claude-models-billing

- **How to configure network isolation for Microsoft Foundry**
  
  Updated the Agent tools support table to show Code Interpreter as fully supported over the Microsoft backbone network. This reduces ambiguity for secure deployments and planning.
  
  https://learn.microsoft.com/en-us/azure/foundry/how-to/configure-private-link

- **Create and manage a toolbox in Foundry**
  
  Streamlined the tools support table by removing the VNet support column and directing readers to a dedicated page for network isolation details. The table now focuses on SDK/tooling support and whether tools can attach directly to an agent, with network guidance consolidated in one place for clarity.
  
  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/tools/toolbox