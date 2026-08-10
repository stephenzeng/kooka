# Microsoft Foundry
**Date created:** 2026-07-21 UTC  
**Tags:** Administration, Agent, AI, Analytics, Automation, Governance, Monitoring, Programming, Security  

## Major Changes

- **Azure Open Datasets**

  Removed the Health and genomics section from the catalog, including the COVID-19 Data Lake entry and its description. This streamlines the catalog to reflect current availability and support. Users should adjust references and pipelines that relied on these listings and consult remaining datasets for alternatives.

  https://learn.microsoft.com/en-us/azure/open-datasets/dataset-catalog

- **Deploy a hosted agent from source code**

  Promoted guidance from preview to GA and overhauled samples to use stable APIs across Python, .NET, and REST. Python examples now use stable SDK surfaces and updated method signatures; REST calls moved from preview to v1 and removed preview headers; and .NET includes a note to use the prerelease Azure.AI.Projects.Agents package. These changes align docs with GA behavior, reduce reliance on preview flags, and provide clearer versioning and cleanup patterns for agent deployments.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/deploy-hosted-agent-code

- **What is Microsoft Foundry?**

  Restructured the overview for clarity and faster onboarding. Removed lengthy code samples and exhaustive model tables, and introduced concise Get started guidance with clear next steps. Added focused sections on what you can build (Agents, Models, Tools/knowledge) and enterprise-ready capabilities (observability, governance/security, unified management), while consolidating and simplifying prior content.

  https://learn.microsoft.com/en-us/azure/foundry/what-is-foundry

## Moderate Changes

- **Featured models of Foundry model catalog**

  Expanded the Azure OpenAI model list with o3, o4-mini, and the gpt-4.1 family, and documented key capabilities like modalities, token limits, and tool calling. Updated gpt-4o-realtime-preview to a newer version and removed o1-preview, helping teams choose supported models and versions confidently.

  https://learn.microsoft.com/en-us/azure/machine-learning/concept-models-featured?view=azureml-api-2

- **COVID-19 Data Lake**

  Replaced the detailed in-page dataset table with a pointer to the centralized Open Datasets catalog. This reduces duplication and keeps dataset references current in one authoritative location.

  https://learn.microsoft.com/en-us/azure/open-datasets/dataset-covid-19-data-lake

- **What are hosted agents?**

  Expanded and reorganized the list of regions where hosted agents are available, adding multiple new regions including Japan West, UAE North, UK West, West Europe, and more. This provides clearer planning guidance for deploying agents near your users and data.

  https://learn.microsoft.com/en-us/azure/foundry/agents/concepts/hosted-agents

- **Bring Your Own Model (BYOM) with Voice Live API**

  Updated Azure CLI examples to use a new role definition ID when assigning the Foundry User role to a system identity. This ensures role assignments succeed with the correct GUID for Foundry resources.

  https://learn.microsoft.com/en-us/azure/ai-services/speech-service/how-to-bring-your-own-model

- **Integrate prompt flow with DevOps for LLM-based applications**

  Fixed code to pass flow_inputs to pf_client.test and added the missing import for Run in Python examples. These corrections prevent runtime errors and enable reliable testing for both standard and evaluation flows.

  https://learn.microsoft.com/en-us/azure/machine-learning/prompt-flow/how-to-integrate-with-llm-app-devops?view=azureml-api-2

- **Create and manage instance types for efficient use of compute resources**

  Corrected default resource limits (memory from 8 GB to 2 GiB), added $schema references to CLI and Kubernetes YAML examples, and updated Python SDK samples to use Environment(image="python:3.12-slim") and gpu settings. These updates improve configuration accuracy and align examples with current APIs.

  https://learn.microsoft.com/en-us/azure/machine-learning/how-to-manage-kubernetes-instance-types?view=azureml-api-2

- **Foundry Agent Service limits, quotas, and regional support**

  Updated Responses API regional support: added Japan West, and made Korea Central and Southeast Asia fully supported. This clarifies where you can deploy and operate responses-dependent workloads.

  https://learn.microsoft.com/en-us/azure/foundry/agents/concepts/limits-quotas-regions