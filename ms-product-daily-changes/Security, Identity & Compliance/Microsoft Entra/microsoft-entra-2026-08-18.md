# Microsoft Entra
**Date created:** 2026-08-18 UTC  
**Tags:** Configuration, Guidance, Identity, Licensing, Security  

## Moderate Changes

- **Product names and service plan identifiers for licensing**

  Updated the licensing reference to include new service plans, such as Skills in Viva and Windows 10 ESU entries for specific Windows 365 SKUs. This improves accuracy for SKU-to-plan mapping used in compliance checks, provisioning, and automation; a note date was refreshed without changing guidance.

  https://learn.microsoft.com/en-us/entra/identity/users/licensing-service-plan-reference

- **Flexible federated identity credentials (preview)**

  Clarified GitHub requirements to match sub plus at least one immutable claim (repository_id or repository_owner_id) and updated examples and supported claim/operator lists accordingly. This strengthens credential binding to repositories or owners, improving supply chain security and reducing risks from repo moves or ownership changes.

  https://learn.microsoft.com/en-us/entra/workload-id/workload-identities-flexible-federated-identity-credentials

- **Set up a Flexible Federated identity credential (preview)**

  Updated setup guidance with issuer-specific requirements, emphasizing GitHub configurations that match sub and immutable claims (repository_id and optionally repository_owner_id). Added Azure portal and Graph request steps with claimsMatchingExpression examples and clarified issuer patterns for GitHub, GitLab, and Terraform Cloud to ensure secure, precise credential binding.

  https://learn.microsoft.com/en-us/entra/workload-id/workload-identities-set-up-flexible-federated-identity-credential