# Microsoft Entra
**Date created:** 2026-08-15 UTC  
**Tags:** Best Practices, Configuration, Governance, Guidance, Identity, Security, Troubleshooting  

## Moderate Changes

- **Token claims reference for agents**

  Removed the 'tid' (tenant ID) claim from the documented token claims for agent identities. This helps developers avoid relying on tenant-specific values in tokens and adapt integrations to supported claims only.

  https://learn.microsoft.com/en-us/entra/agent-id/agent-token-claims

- **Best practices for Microsoft Entra Agent ID**

  Added guardrails for AI coding assistants recommending the use of agent identity blueprints instead of standard app registrations. Included repository instructions, required roles and permissions, and .NET implementation patterns using Microsoft.Identity.Web.AgentIdentities for app-only and on-behalf-of flows. This guidance streamlines secure setup and aligns implementations with supported provisioning paths.

  https://learn.microsoft.com/en-us/entra/agent-id/best-practices-agent-id

- **Call Azure services from your agent using .NET Azure SDK**

  Updated .NET samples to properly configure agent identities, pass TokenCredential to clients, and use clear scenarios for app-only and on-behalf-of-user calls. Clarified options such as WithAgentIdentity and RequestAppToken and standardized tenant ID placeholders. These fixes reduce authentication errors and make sample code production-ready.

  https://learn.microsoft.com/en-us/entra/agent-id/call-api-azure-services

- **Call custom APIs from an agent using .NET**

  Refined code examples by adding required using directives, removing redundant placeholders, and renaming helpers for clarity (UPN/OID variants). Clarified the on-behalf-of flow and simplified controller code without changing core concepts. These edits improve readability and reduce confusion when implementing agent-to-API calls.

  https://learn.microsoft.com/en-us/entra/agent-id/call-api-custom

- **Call a Microsoft Graph API from an agent using .NET**

  Enhanced samples and guidance with required using directives, least-privilege permission advice, and examples aligned to Users endpoints. Clarified how to reference an agent’s user identity via UPN or OID across app-only and on-behalf-of scenarios. This helps developers request the right scopes and implement consistent identity patterns.

  https://learn.microsoft.com/en-us/entra/agent-id/call-api-microsoft-graph

- **Risk-based access policies**

  Introduced the attacker-added device scenario and clarified adaptive remediation behavior: the Entra device object is disabled to block new token issuance, user sessions are revoked, and users are prompted to sign in again. Removed earlier wording about revoking existing device-bound refresh tokens to reflect current behavior. This update sharpens expectations for incident response and session control.

  https://learn.microsoft.com/en-us/entra/id-protection/concept-identity-protection-policies

- **Replica sets concepts and features for Microsoft Entra Domain Services**

  Added an important note detailing that all replica-set virtual networks must have direct, fully meshed connectivity within a single AD site for replication. The guidance explains that missing connectivity can cause authentication, domain controller communication, and Netlogon issues. This helps teams validate network design before cross-region deployments.

  https://learn.microsoft.com/en-us/entra/identity/domain-services/concepts-replica-sets

- **Create agent identities in agent identity platform**

  Standardized tenant ID placeholders and corrected the Program.cs sample by adding necessary using directives, reordering top-level statements, and fixing endpoint mapping syntax. These corrections improve accuracy and prevent compile-time errors in sample code.

  https://learn.microsoft.com/en-us/entra/agent-id/create-delete-agent-identities

- **Microsoft agent identity platform error codes**

  Reorganized the error code reference into clear categories (for example, quotas, blueprints, and identity creation) and added explanatory context before each section. Updated table headers for consistency without changing code meanings. This structure improves discoverability and speeds troubleshooting.

  https://learn.microsoft.com/en-us/entra/agent-id/error-codes

- **Plan your agent identity architecture**

  Added guidance to avoid standard app registrations for AI agents and use agent identity blueprints instead. Included a comparison mapping common app registration steps to blueprint-based processes and .NET guidance using Microsoft.Identity.Web.AgentIdentities. This ensures correct provisioning, clearer governance, and smoother implementation. 

  https://learn.microsoft.com/en-us/entra/agent-id/how-to-plan-agent-identity-architecture