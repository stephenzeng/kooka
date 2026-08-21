# Microsoft Foundry
**Date created:** 2026-08-21 UTC  
**Tags:** Analytics, Best Practices, Configuration, Deprecation, Governance, Guidance, Monitoring, Performance, Security, Troubleshooting  

## New Articles

- **Evaluate model router for your workload**

  Introduced a new how-to that explains how to evaluate model router against a baseline for response quality, estimated cost, and latency. It guides you through prerequisites, defining acceptance criteria and a fair test plan, preparing datasets, and running comparisons with the Model Router Auto Evaluation toolkit. The article shows how to interpret results and tradeoffs, choose routing modes and model subsets, validate under production-like traffic, and set up ongoing monitoring and periodic reevaluation. Links to the toolkit quickstart, methodology, and related guidance are included.

  https://learn.microsoft.com/en-us/azure/foundry/openai/how-to/evaluate-model-router

## Major Changes

- **Add guardrails to a hosted agent**

  Set a hard cap of 480 rules per egress policy and added guidance on requesting quota increases through Azure support. Expanded monitoring instructions to trace egress decisions in the Foundry portal (Trajectories tab), clarified decision span fields, and noted that decisions are emitted to trace monitoring tools. Updated Application Insights navigation and preserved the Kusto query to streamline troubleshooting and governance.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/add-hosted-agent-guardrails

- **Manage automatic upgrades from Azure OpenAI to Microsoft Foundry**

  Substantially rewrote the guide to focus on managing automatic upgrades, including checking status, deferring or opting out, and rolling back. Added prerequisites, clarified preview API usage, and documented opt-out paths via Azure portal, Bicep, and Terraform with validation steps. Detailed eligibility and constraints (networking, CMK, integrations, DNS, regional limits), expanded rollback guidance, and added troubleshooting plus strengthened governance and security recommendations.

  https://learn.microsoft.com/en-us/azure/foundry/how-to/upgrade-azure-openai-auto

## Moderate Changes

- **Access on-premises resources from your Microsoft Foundry managed network**

  Updated Azure CLI guidance to use separate --destination and --subresource-target parameters, removed the deprecated sparkEnabled property, and aligned REST examples to api-version 2026-05-01. Added instructions for adding FQDN aliases (fqdns) to private endpoint outbound rules, including UserDefined category, and referenced the outboundRules resource. These updates improve compatibility with current APIs and make outbound rule management more flexible.

  https://learn.microsoft.com/en-us/azure/foundry/how-to/access-on-premises-resources

- **Deploy a hosted agent**

  Reworked the Responses protocol guidance to be language-agnostic with a new Python example and clarified that the library manages event sequencing and response lifecycle. Updated thread-safety guidance for per-request handler scoping and safe concurrency, refreshed sample links, and documented using force=True to cascade-delete active sessions during agent deletion.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/deploy-hosted-agent

- **Deploy Microsoft Foundry Models to managed compute with pay-as-you-go billing (classic) **

  Added new supported models: TabPFN-3-Plus-Thinking (Forecasting) and voyage-code-4 (Embeddings). This expands available options and helps teams plan deployments that match workload needs.

  https://learn.microsoft.com/en-us/azure/foundry-classic/how-to/deploy-models-managed-pay-go

- **Manage and increase quotas and limits for resources with Azure Machine Learning**

  Added a note that when an online endpoints quota increase affects a data-plane limit, you must re-create the impacted online deployments for the new limit to take effect. This ensures capacity changes are applied and avoids confusing behavior after quota approvals.

  https://learn.microsoft.com/en-us/azure/machine-learning/how-to-manage-quotas?view=azureml-api-2

- **Foundry Agent Service limits, quotas, and regional support**

  Expanded regional availability for the Responses API to Canada Central, Japan West, Norway East, Poland Central, Switzerland North, Switzerland West, and West Central US. This enables broader deployment planning and can reduce latency by using closer regions.

  https://learn.microsoft.com/en-us/azure/foundry/agents/concepts/limits-quotas-regions

- **Use model router for Microsoft Foundry**

  Clarified that model router can act as a drop-in deployment and as an optimization layer that handles per-request model selection, and advised evaluating against your current baseline. Replaced the in-page evaluation walkthrough with concise benchmarking guidance that links to a dedicated evaluation article for details. This streamlines how-to content while directing readers to comprehensive evaluation best practices.

  https://learn.microsoft.com/en-us/azure/foundry/openai/how-to/model-router

- **How model router works in Microsoft Foundry**

  Renamed and expanded the rationale section to frame model router as an optimization layer that reduces manual model comparison and custom routing logic. Clarified that routing depends on configured modes and eligible model subsets, and recommended baseline comparisons and reevaluation after changing routing configurations.

  https://learn.microsoft.com/en-us/azure/foundry/openai/concepts/model-router-how-it-works

- **Migrate from GitHub Models to Microsoft Foundry Models**

  Retitled the article to emphasize migration and noted that GitHub Models was retired on July 30, 2026. Directs customers to move to Microsoft Foundry Models while retaining the core how-to content via the existing include.

  https://learn.microsoft.com/en-us/azure/foundry/foundry-models/how-to/quickstart-github-models