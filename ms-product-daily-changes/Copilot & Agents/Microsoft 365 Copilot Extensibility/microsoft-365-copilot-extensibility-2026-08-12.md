# Microsoft 365 Copilot Extensibility
**Date created:** 2026-08-12 UTC  
**Tags:** Automation, Best Practices, Billing, Configuration, Consumption, Get Started, Guidance, Troubleshooting  

## New Articles

- **Add custom evaluators to your agent evaluations**

  Introduced a how-to guide for creating and using custom evaluators with the Agent Evaluations CLI, covering LLM-judge (.py + .prompty) and code-only (.py) approaches with required folder structure and naming rules. Provides guidance for authoring prompty files, implementing Python evaluator contracts, handling parameters and model_config, and returning standardized scores. Explains threshold behaviors, graded vs. boolean scoring patterns, and how to reference custom evaluators in evaluation documents with evaluators_mode. Includes security considerations and a troubleshooting section to help diagnose common errors.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/extensibility/evaluations-cli-custom-evaluators

## Major Changes

- **Get values for Agent Evaluations CLI environment variables**

  Overhauled configuration to use Microsoft Foundry projects with Microsoft Entra authentication instead of Azure OpenAI keys. Added steps to deploy a GPT-5 mini model, set AZURE_AI_PROJECT_ENDPOINT and AZURE_AI_MODEL_NAME, and sign in via az login. Updated prerequisites to require the Azure AI Developer role and revised troubleshooting to address Foundry role and tenant sign-in issues.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/extensibility/evaluations-cli-get-env-values

- **Agent Evaluations CLI overview**

  Removed preview status and shifted guidance to Microsoft Foundry cloud evaluation with built-in metrics. Replaced Azure OpenAI variables with Foundry equivalents (AZURE_AI_PROJECT_ENDPOINT and AZURE_AI_MODEL_NAME) and set gpt-5-mini as the default model. Updated descriptions and workflows to align with Foundry-based authentication and scoring.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/extensibility/evaluations-cli-overview

- **Quickstart: Use the Agent Evaluations CLI**

  Removed preview status and updated prerequisites to require Copilot credits with usage-based billing enabled. Moved setup to a Microsoft Foundry project using a GPT-5 model, replaced Azure OpenAI variables with AZURE_AI_PROJECT_ENDPOINT and gpt-5-mini, and retained TENANT_ID. Clarified that scoring uses Foundry cloud evaluation authenticated via Microsoft Entra and requires az login; updated admin consent references to Work IQ.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/extensibility/evaluations-cli-quickstart

- **Agent Evaluations CLI reference**

  Removed preview status and updated evaluation architecture to use Microsoft Foundry cloud evaluation and built-in metrics. Refreshed the sample CLI version to 1.15.0 and replaced Azure OpenAI configuration with AZURE_AI_PROJECT_ENDPOINT, updating model examples to gpt-5-mini. Streamlined optional settings by removing API version requirements.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/extensibility/evaluations-cli-reference

- **Troubleshoot the Agent Evaluations CLI**

  Reworked authentication guidance to use Microsoft Foundry access with Microsoft Entra sign-in instead of Azure OpenAI keys. Added steps to sign in to the correct tenant via Azure CLI, confirm Azure AI Developer role on the Foundry project, verify AZURE_AI_PROJECT_ENDPOINT, and ensure the model (gpt-5-mini) is deployed. Removed preview markers and updated error handling for 401/403 scenarios tied to Foundry permissions and tenant issues.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/extensibility/evaluations-cli-troubleshooting

## Moderate Changes

- **Choose the right tool to build your declarative agent**

  Added guidance on using Work IQ Dev Tools (wiqd) as a CLI layer over the declarative agent lifecycle. Highlights that it leverages Agents Toolkit while enabling validate, package, and publish from terminal or CI.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/extensibility/declarative-agent-tool-comparison

- **Evaluators reference for Agent Evaluations CLI**

  Removed the preview designation to indicate general availability. Clarified that LLM-based evaluators run using an Azure OpenAI model within a Microsoft Foundry project, refining environment setup guidance.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/extensibility/evaluations-cli-evaluators

- **Microsoft 365 Copilot extensibility planning guide**

  Added a TIP introducing the wiqd CLI for a consistent command surface across local, CI, and VS Code. Describes using named environments (local, dev, staging, prod) aligned to rollout plans.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/extensibility/planning-guide

- **Publish agents for Microsoft 365 Copilot**

  Added a TIP on publishing declarative agents via wiqd, including validate, package, and publish commands to the organizational catalog. Notes that admin approval remains required before agents are available.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/extensibility/publish