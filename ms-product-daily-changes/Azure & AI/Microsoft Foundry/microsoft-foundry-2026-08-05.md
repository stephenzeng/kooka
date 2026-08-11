# Microsoft Foundry
**Date created:** 2026-08-05 UTC  
**Tags:** Administration, Agent, AI, Automation, Governance, Programming, Security  

## New Articles

- **Create a private skill catalog in Foundry Agent Service**

  Introduced a new how-to for creating a private skill catalog (preview) with Azure API Center to govern which tools and skills agents can use. The article outlines admin and developer roles, step-by-step skill registration with allowed tools, and optional AI assessment of submissions. It also covers RBAC setup so developers can discover approved skills, verification steps in Foundry, and troubleshooting for common visibility and access delays. This guidance helps organizations enforce boundaries, improve discoverability, and streamline approval workflows for agent skills.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/private-skill-catalog

## Major Changes

- **Add guardrails to a hosted agent**

  Updated guidance to require azd ai agent extension version 1.0.0-beta.1 and clarified how azd maps policies to the Foundry rai_config at deployment. The configuration model now uses a policies list with type: rai_policy and raiPolicyName (full ARM ID) instead of setting rai_config.rai_policy_name directly. YAML examples and CLI steps were reworked to reflect the new policy-based approach, reducing configuration errors and aligning with current deployment practices.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/add-hosted-agent-guardrails

- **Foundry Agent Service limits, quotas, and regional support**

  Updated the model tool support matrix by removing several Claude models, indicating changes in supported capabilities. This affects planning for tool integration and model availability, and teams should review their dependencies to avoid using unsupported entries.

  https://learn.microsoft.com/en-us/azure/foundry/agents/concepts/limits-quotas-regions

- **How to configure Azure OpenAI in Microsoft Foundry Models with Microsoft Entra ID authentication (classic)**

  Substantially expanded guidance from basic managed identity setup to a comprehensive Microsoft Entra ID authentication workflow. The update compares Entra ID options (developer accounts, system-assigned, user-assigned, service principals), adds end-to-end local development with DefaultAzureCredential and token provider usage, and includes a verification flow using az and curl. It also introduces control plane authentication audience differences, role requirements, and detailed troubleshooting for common 401/403 and configuration issues. These changes help teams choose the right identity approach, validate tokens, and reliably secure both inference and control plane operations.

  https://learn.microsoft.com/en-us/azure/foundry-classic/openai/how-to/managed-identity

- **Automate agents with routines (preview)**

  Expanded routines to support event-based triggers alongside schedules and timers, adding a new custom trigger with Microsoft Teams channel message events. Guidance now spans the Foundry portal, REST, Python, .NET, JavaScript SDKs, and Azure Developer CLI with detailed steps for creating and authorizing the Teams connector and defining routines. Documentation clarifies trigger and action types, updates SDK requirements, and consolidates identity prerequisites for unattended runs. These updates enable richer automation scenarios and simplify cross-tool configuration.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/use-routines

## Moderate Changes

- **Evaluate your AI agents**

  Raised the SDK requirement to azure-ai-projects>=2.4.0 and switched evaluation jobs to the long-running operation pattern with a poller (begin_create_generation_job). Optional periodic status output and streamlined result retrieval improve reliability and simplify code.

  https://learn.microsoft.com/en-us/azure/foundry/observability/how-to/evaluate-agent

- **Generate a synthetic evaluation dataset (preview)**

  Updated to azure-ai-projects>=2.4.0 and reworked examples to use a long-running operation poller instead of manual status checks. The changes include periodic status printing, adjusted imports, and simplified result handling via poller.result() for clearer, more robust workflows.

  https://learn.microsoft.com/en-us/azure/foundry/observability/how-to/evaluation-dataset-synthetic

- **Manage compliance and security in Microsoft Foundry**

  Expanded Microsoft Purview billing guidance to include support for an Agent 365 subscription in addition to pay-as-you-go, clarifying that otherwise only Purview Audit is supported. Replaced an image-based instruction with an explicit step to select the Data security and governance tab, improving clarity.

  https://learn.microsoft.com/en-us/azure/foundry/control-plane/how-to-manage-compliance-security

- **Quickstart: Optimize a hosted agent (preview)**

  Increased the Python package requirement to azure-ai-projects>=2.4.0 and adopted a poller-based long-running operation (begin_create_optimization_job). Removed manual JobStatus checks and simplified result handling with poller.result() for cleaner, more maintainable samples.

  https://learn.microsoft.com/en-us/azure/foundry/agents/quickstarts/quickstart-optimize-hosted-agent

- **Convert agent traces into evaluation datasets (preview)**

  Updated the SDK to version 2.4.0 and migrated to a long-running operation pattern for generation jobs. The sample removes manual terminal state logic, adds a configurable poll interval, and streamlines output handling for more reliable dataset creation.

  https://learn.microsoft.com/en-us/azure/foundry/observability/how-to/traces-to-dataset

- **What is Foundry Local?**

  Refreshed the overview to second-person language, clarified on-device benefits, and emphasized device-local operations. Added a “Choose your next step” section with quick-start links to help readers quickly proceed to getting started, architecture, and tutorials.

  https://learn.microsoft.com/en-us/azure/foundry-local/what-is-foundry-local