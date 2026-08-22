# Microsoft Foundry
**Date created:** 2026-08-22 UTC  
**Tags:** Analytics, Best Practices, Billing, Configuration, Consumption, Get Started, Governance, Guidance, Monitoring, Performance, Security  

## Major Changes

- **Run agent evaluations with the azd CLI (preview)**

  Adopted the new azd ai eval extension and workflow, replacing older agent-specific commands. Introduces a streamlined lifecycle for initializing, generating, creating, and running evaluations, with support for dataset- and trace-based sources. Adds CI gating with failure thresholds, job management, summaries export, and evaluator discovery/configuration, and integrates evaluations into deployments with azd up. Deprecates prior hosted-agent flows and legacy commands to reduce confusion and align with the current toolchain.

  https://learn.microsoft.com/en-us/azure/foundry/observability/how-to/azure-developer-cli-evaluation

## Moderate Changes

- **Add Microsoft Foundry to a network security perimeter**

  Updated validation instructions to replace “Learning mode” with “Transition mode” in the Validate before enforcement steps, including the revert step. This aligns terminology with the current mode to avoid confusion during rollout.

  https://learn.microsoft.com/en-us/azure/foundry/how-to/add-foundry-to-network-security-perimeter

- **Train models with Azure Machine Learning**

  Clarified that Automated ML requires explicit job configuration and that pipelines support both Automated ML and command jobs. Documented that the Azure CLI can submit command, Automated ML, and pipeline jobs, and refined the training lifecycle guidance for script-based command jobs.

  https://learn.microsoft.com/en-us/azure/machine-learning/concept-train-machine-learning-model?view=azureml-api-2

- **Set up AutoML training for tabular data with the Azure Machine Learning CLI and Python SDK**

  Added Multinomial Naive Bayes and the spearman_correlation metric to supported options, and noted that the UI now shows a featurization summary alongside hyperparameters and training code. Updated examples to the sklearn-1.5 registry environment and flagged TabularTrainingMode as experimental.

  https://learn.microsoft.com/en-us/azure/machine-learning/how-to-configure-auto-train?view=azureml-api-2

- **Create and manage data assets**

  Updated example environments to use the azureml registry sklearn-1.5 latest label, replacing older image references. Simplified data asset examples by switching to direct relative paths for clarity.

  https://learn.microsoft.com/en-us/azure/machine-learning/how-to-create-data-assets?view=azureml-api-2

- **Run Jupyter notebooks in your workspace**

  Added a prerequisite to use a compute instance with sufficient regional quota, noting potential charges while it’s running. Clarified notebook execution behavior, including execution counts, output display, and kernel status.

  https://learn.microsoft.com/en-us/azure/machine-learning/how-to-run-jupyter-notebooks?view=azureml-api-2

- **Manage hosted agent sessions**

  Updated azd guidance for configuring hosted session idle timeouts via sessionConfiguration in azure.yaml and documented required extension version (1.0.0-beta.11+) with install/update commands. Removed older provisional guidance to consolidate instructions.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/manage-hosted-sessions

- **Tutorial: Create resources you need to get started**

  Expanded the tutorial with learning objectives, required permissions, and billing/region availability considerations. Added steps to wait for workspace and compute readiness, a brief studio orientation, and guidance on when to delete the resource group versus individual resources to control costs.

  https://learn.microsoft.com/en-us/azure/machine-learning/quickstart-create-resources?view=azureml-api-2

- **Azure AI Search regions list**

  Expanded preview regional availability for the Serverless pricing model to additional regions including Australia East, Central India, Central US, Japan East, North Central US, Sweden Central, Switzerland North, UK South, West Central US, West US, and West US 2. This broadens deployment options for evaluating Serverless.

  https://learn.microsoft.com/en-us/azure/search/search-region-support

- **Optimize costs for the Serverless pricing model in Azure AI Search**

  Clarified how compute, memory, and disk I/O translate to Compute Units (CUs) in Serverless and contrasted cost accounting with Dedicated. Detailed what Serverless CU charges cover versus external billable components (for example, semantic ranking and certain skill executions), helping teams plan and optimize spend.

  https://learn.microsoft.com/en-us/azure/search/serverless-cost-optimization

- **Eliminate optional vector instances from storage**

  Clarified that when a vector field is not stored (stored: false), partial updates must include the vector field or the existing vector will not be preserved. Recommended setting stored: true to avoid data loss during reindexing and partial updates.

  https://learn.microsoft.com/en-us/azure/search/vector-search-how-to-storage-options