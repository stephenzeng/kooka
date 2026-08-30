# Microsoft Entra
**Date created:** 2026-08-30 UTC  
**Tags:** Automation, Best Practices, Configuration, Guidance, Identity, Troubleshooting  

## New Articles

- **Troubleshoot user provisioning validation for Microsoft Entra App Gallery (preview)**

  New troubleshooting guidance helps ISV developers diagnose and fix failures in the Logic Apps–based SCIM validation for App Gallery integrations. It details how to trace runs using Logic Apps outputs and provisioningErrorDetails, and provides fixes for common issues like incorrect endpoint URLs, token expiration, missing managed identity permissions, and schema mismatches. It also clarifies expected SCIM behaviors (for example, handling 409 conflicts, empty-result queries, and filtered GET support), group provisioning requirements, and rate limiting expectations of at least 25 RPS per tenant. Links to validation overview, onboarding requirements, and known issues streamline follow-up actions.

  https://learn.microsoft.com/en-us/entra/identity/enterprise-apps/troubleshoot-user-provisioning-validation

- **Validate user provisioning for Microsoft Entra App Gallery (preview)**

  Introduces a step-by-step how-to for validating SCIM-based user and group provisioning using either an Azure Logic Apps template or an AI-driven onboarding agent. It covers prerequisites, choosing the setup path, running a 25-test workflow across users, groups, and SCIM compliance, and interpreting pass conditions and exceptions. The article explains how to capture the Logic App run ID, submit results in the Microsoft Entra admin center, and clean up resources, with links to related requirements and troubleshooting.

  https://learn.microsoft.com/en-us/entra/identity/enterprise-apps/validate-user-provisioning-app-gallery

- **Set up the validation Logic App in the Azure portal (preview)**

  Provides a detailed guide to deploy and run the Azure Logic Apps validation template for SCIM provisioning tests. It walks through creating required resources, importing workflows from the SCIMReferenceCode repository, enabling a managed identity, assigning roles, and configuring parameters such as servicePrincipalId, SCIM endpoint/auth, test domain, and default user properties. The article explains the orchestrator and nested workflows, how to execute runs and review outputs, optional script-based validation, and how to clean up test resources.

  https://learn.microsoft.com/en-us/entra/identity/enterprise-apps/validate-user-provisioning-logic-app

## Moderate Changes

- **User provisioning requirements for Microsoft Entra App Gallery**

  Added a “Validate your integration” requirement directing ISVs to test their SCIM endpoint with the Microsoft Entra provisioning validation and include results in App Gallery submissions. This clarifies the prerequisites and ensures higher-quality, standards-compliant integrations.

  https://learn.microsoft.com/en-us/entra/identity/enterprise-apps/app-gallery-user-provisioning-requirements

- **Tutorial - Develop a SCIM endpoint for user provisioning to apps from Microsoft Entra ID**

  Reworked publishing guidance to a self-service model, replacing onboarding narrative with links to centralized prerequisites and validation steps. Clarified OAuth 2.0 client credentials expectations—customers provide Tenant URL, Token Endpoint, Client ID, and Client Secret—and advised ISVs to surface these in their admin experience. Removed the note that Microsoft would enable Workload Identity Federation, aligning with the new self-service approach.

  https://learn.microsoft.com/en-us/entra/identity/app-provisioning/use-scim-to-provision-users-and-groups