# Microsoft Entra
**Date created:** 2026-07-24 UTC  
**Tags:** Administration, Automation, Security  

## New Articles

- **Configure Azure Databricks for automatic user provisioning with Microsoft Entra ID**

  Introduced a step-by-step tutorial for configuring SCIM-based automatic user and group provisioning from Microsoft Entra ID to Azure Databricks at the account level. The guidance covers prerequisites, connector setup, credential configuration, assignments, enabling sync, monitoring, and operational best practices. It documents limitations (for example, no service principals or nested groups via SCIM, immutable email constraint, connector not available in Azure China) and recommends disabling workspace-level SCIM when moving to account-level provisioning. It also includes troubleshooting tips, required IP ranges for the provisioning service, an option to automate via Microsoft Graph, and notes an alternative Databricks identity management approach that supports service principals and nested groups.

  https://learn.microsoft.com/en-us/entra/identity/saas-apps/azure-databricks-provisioning-tutorial

- **Global Secure Access egress IP ranges**

  Added a reference listing the egress IP ranges used by Global Secure Access to help administrators allowlist outbound traffic on downstream services. The page introduces two CIDR blocks (128.94.0.0/19 and 151.206.0.0/16) and links to related points of presence and IP address information. This helps ensure connectivity reliability and consistent enforcement of network policies for Global Secure Access traffic.

  https://learn.microsoft.com/en-us/entra/global-secure-access/reference-egress-ip-ranges

## Moderate Changes

- **Group Policy - Public Preview**

  Updated the title and content to mark Group Policy Backup as Public Preview and clarified that it enhances the service rather than being a new Domain Health Monitor feature. This sets accurate expectations for deployment planning and feature evaluation.

  https://learn.microsoft.com/en-us/entra/identity/domain-services/group-policy

- **Microsoft Entra Connect: Cloud authentication via Staged Rollout**

  Removed the prior 50,000-user group size limit and clarified support for up to 10 groups per feature (password hash sync, pass-through authentication, seamless SSO). Added guidance on using Temporary Access Pass to streamline sign-in for newly added users during migration, reducing extra federated authentication prompts.

  https://learn.microsoft.com/en-us/entra/identity/hybrid/connect/how-to-connect-staged-rollout

- **Configure optional claims**

  Added an “amr claim” section explaining how to request and receive authentication method references for SAML apps, including default behavior for Salesforce and how to enable granular AMR using the include_granular_amr property. Clarifies that “multipleauthn” and “mfa” are emitted only after MFA completes and links to SAML authnmethodreferences for deeper details.

  https://learn.microsoft.com/en-us/entra/identity-platform/optional-claims

- **Optional claims reference**

  Added the amr optional claim to the v2.0 set and introduced a reference section mapping Microsoft Entra authentication methods to OIDC amr values. Explains when AMR is included for SAML/OIDC apps, how to request granular AMR via include_granular_amr, and notes that AMR values from external MFA providers can be forwarded.

  https://learn.microsoft.com/en-us/entra/identity-platform/optional-claims-reference

- **Workload identity federation concepts**

  Updated AWS integration guidance to use AWS IAM Outbound Identity Federation instead of Amazon Cognito. The revised flow covers establishing trust with the AWS account, obtaining a JWT from IAM Outbound Identity Federation, exchanging it for a Microsoft access token, and accessing Microsoft Entra–protected resources, with links updated accordingly.

  https://learn.microsoft.com/en-us/entra/workload-id/workload-identity-federation