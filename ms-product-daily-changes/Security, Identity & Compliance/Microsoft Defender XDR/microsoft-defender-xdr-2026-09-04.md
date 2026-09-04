# Microsoft Defender XDR
**Date created:** 2026-09-04 UTC  
**Tags:** Compliance, Configuration, Governance, Guidance, Monitoring, Security  

## Major Changes

- **View your identity coverage and maturity (Preview)**
  Expanded guidance helps teams interpret identity coverage by clarifying the Observed column and adding a global Show Only Observed Applications toggle in side panels. A new On-premises identities panel explains onboarding, activation, and migration metrics, with action names aligned to sensor version transitions. The SaaS identities panel was refined to emphasize observed SaaS apps and how to connect other supported applications, improving visibility and next steps for coverage maturation.
  https://learn.microsoft.com/en-us/defender-xdr/identity-security/coverage-maturity

## Moderate Changes

- **Map existing RBAC permissions to Microsoft Defender unified RBAC permissions**
  Updated mappings expand Email & collaboration roles and role groups, clarify import behavior (only actively assigned source roles/role groups are imported), and explain how role-group permissions derive from the union of mapped roles. Added links to Microsoft Purview documentation, an example for the Preview role with prerequisite permissions auto-selected, and a note on Exchange Online permissions activation for clearer setup and governance.
  https://learn.microsoft.com/en-us/defender-xdr/compare-rbac-roles

- **Detect and investigate threats to AI agents using Microsoft Defender (Preview)**
  Clarified that threat detection currently applies only to published Microsoft Foundry agents; unpublished or playground-only agents aren’t supported. Included pointers to publishing steps for Microsoft 365 Copilot and Microsoft Teams so teams can enable protection.
  https://learn.microsoft.com/en-us/defender-xdr/security-for-ai/ai-agent-detection-protection