# Microsoft Foundry
**Date created:** 2026-08-28 UTC  
**Tags:** Analytics, Best Practices, Billing, Configuration, Deprecation, Get Started, Governance, Guidance, Identity, Security  

## New Articles

- **Microsoft Foundry product and capability map**

  Introduced a concept guide that maps common goals to the right starting points across Foundry, helping readers quickly find relevant quickstarts and how-to content. Provides a comprehensive capability table explaining what each feature is, when to use it, and who it’s for. Adds related links to overviews and architecture to streamline onboarding and discovery.

  https://learn.microsoft.com/en-us/azure/foundry/concepts/capabilities

- **Microsoft Foundry capability reference**

  Published a catalog-style reference that organizes Foundry capabilities by area and links to canonical documentation. Highlights build surfaces, models, agents, tools, knowledge/RAG, observability, evaluation, trust and safety, governance, and APIs/SDKs, with preview items clearly marked. Serves as a navigational index to accelerate wayfinding across the product.

  https://learn.microsoft.com/en-us/azure/foundry/concepts/capability-reference

## Major Changes

- **Batch endpoints**

  Announced retirement of low-priority VMs for Azure Machine Learning batch endpoints as of March 31, 2026; configurations now use Spot VMs. Updated guidance explains pricing, eviction behavior, and how rescheduling handles deallocated nodes while retaining completed mini-batches. Clarifies that job-level checkpointing isn’t provided, informing reliability and cost planning.

  https://learn.microsoft.com/en-us/azure/machine-learning/concept-endpoints-batch?view=azureml-api-2

- **Enable incoming A2A on a Foundry agent**

  Restricted incoming A2A support to prompt agents and updated prerequisites to require a deployed prompt agent. Standardized authentication on Microsoft Entra ID and clarified least-privilege role options and scopes for endpoint access. Added strict version selection validation (conflicting header/query version returns HTTP 400) and a detailed access-grant workflow covering identity scenarios, CLI role assignment, and token scopes.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/enable-agent-to-agent-endpoint

- **Generate a synthetic evaluation dataset (preview)**

  Added two task types for synthetic data: Simple QnA (single-turn) and Simulation seed (multi-turn), with updated portal flow and SDK requirements (Python 2.5.0+). Introduced full SDK guidance for generating simulation seeds, clarified schema (test_case_description required; other fields optional), and how to use seeds to drive conversation simulations. Distinguished evaluation paths for single-turn vs. multi-turn datasets and added best practices for scenario-focused authoring.

  https://learn.microsoft.com/en-us/azure/foundry/observability/how-to/evaluation-dataset-synthetic

## Moderate Changes

- **Run cloud evaluations with the Microsoft Foundry SDK**

  Reorganized setup into language-specific tabs and expanded instructions for Python and JavaScript/TypeScript. Added install steps and examples for authenticating with DefaultAzureCredential, creating AIProjectClient, and obtaining an OpenAI client, with clearer environment variable guidance.

  https://learn.microsoft.com/en-us/azure/foundry/observability/how-to/cloud-evaluation

- **Evaluate datasets in the cloud**

  Added multi-language, tabbed examples for uploading JSONL datasets, providing inline content, and defining data sources and testing criteria. Included JavaScript examples for coherence, violence, and F1 evaluators, plus guidance on creating evaluations/runs and using dataset IDs with cURL.

  https://learn.microsoft.com/en-us/azure/foundry/observability/how-to/cloud-evaluation-datasets

- **Evaluate deployed agent and model interactions**

  Introduced a JavaScript/TypeScript example that creates and runs evaluations against Azure AI responses, including evaluator setup and data mapping. Demonstrates configuration of data sources and criteria, and logs the evaluation run ID for tracking.

  https://learn.microsoft.com/en-us/azure/foundry/observability/how-to/cloud-evaluation-deployed-interactions

- **Get cloud evaluation results**

  Added JavaScript/TypeScript and cURL tabs to complement the Python example, enabling polling for run status and retrieving output via the Evals API. Provided REST guidance for using evaluation and run IDs and a direct link to the report URL.

  https://learn.microsoft.com/en-us/azure/foundry/observability/how-to/cloud-evaluation-results

- **Generate synthetic data (preview)**

  Added JavaScript/TypeScript tabs clarifying current SDK limitations for synthetic data evaluation and pointing to Python or cURL for runnable samples. Simplified the scenario schema by making only test_case_description required and added tips to use “Simulation seed (multi-turn)” to auto-generate dataset IDs.

  https://learn.microsoft.com/en-us/azure/foundry/observability/how-to/cloud-evaluation-synthetic-data

- **Evaluate models and agents in the cloud**

  Expanded with JavaScript/TypeScript examples for configuring inputs, targets, and evaluators (coherence, violence, task_adherence), alongside Python and cURL. Clarified hosted agent evaluation via the invocations protocol and noted current JS/TS SDK gaps for hosted-agent invocation.

  https://learn.microsoft.com/en-us/azure/foundry/observability/how-to/cloud-evaluation-targets

- **Use admin-connected models in cloud evaluations**

  Added Python and JavaScript/TypeScript samples showing how to set admin-connected models for evaluators and as targets, including sampling parameters. Linked to relevant evaluator and API references to streamline configuration.

  https://learn.microsoft.com/en-us/azure/foundry/observability/how-to/evaluate-admin-connected-models

- **Deploy models for scoring in batch endpoints**

  Noted that azureml-core (SDK v1) was deprecated on March 31, 2025 with support ending June 30, 2026, yet remains required at runtime for batch scoring scripts. Updated the recommended container image to Ubuntu 22.04, corrected logging level values, revised API references, and clarified error_threshold semantics.

  https://learn.microsoft.com/en-us/azure/machine-learning/how-to-use-batch-model-deployments?view=azureml-api-2

- **Use a screen reader with Microsoft Foundry**

  Updated for the new Foundry experience with clearer navigation (including Manage) and screen reader announcements for key transitions. Improved descriptions of Operate and Docs and refined headings and wording for accessibility.

  https://learn.microsoft.com/en-us/azure/foundry/tutorials/screen-reader

- **Tutorial: Upload, access, and explore your data in Azure Machine Learning**

  Clarified that the tutorial uses an Azure ML notebook to upload a CSV, register it as a versioned data asset, and explore it with Python. Distinguished cost implications for assets created from existing cloud storage versus uploads to the workspace datastore.

  https://learn.microsoft.com/en-us/azure/machine-learning/tutorial-explore-data?view=azureml-api-2