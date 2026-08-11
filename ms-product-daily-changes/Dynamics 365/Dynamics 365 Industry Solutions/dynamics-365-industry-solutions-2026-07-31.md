# Dynamics 365 Industry Solutions
**Date created:** 2026-07-31 UTC  
**Tags:** Administration, Azure, Governance, Monitoring, Security  

## Moderate Changes

- **Azure landing zone for Nonprofits architecture**

  Clarified the foundation networking posture: the application subnet is private with NSG rules that deny internet ingress and egress, and default outbound connectivity isn’t provided. Documented that the baseline omits NAT Gateway, Azure Firewall, centralized egress, paid DDoS protection, and public IPs, helping teams plan explicit, approved outbound paths.

  https://learn.microsoft.com/en-us/industry/nonprofit/azure-landing-zone-architecture

- **Deploy Azure landing zone for Nonprofits with the Azure CLI**

  Expanded parameter guidance for foundation and platform profiles, detailing NSG deny-by-default behavior and how Key Vault access should use private endpoints for durable data-plane operations. Clarified that when private endpoints are disabled, the Key Vault public endpoint remains behind a deny-by-default firewall, and added checklist steps to verify NSG rules and explicit outbound designs align with workload needs.

  https://learn.microsoft.com/en-us/industry/nonprofit/azure-landing-zone-cli

- **Considerations and limitations for Azure landing zone for Nonprofits**

  Added definitive guidance that Key Vault’s public endpoint is enabled but blocked by a deny-by-default firewall, recommending private connectivity for sustained access. Elaborated the foundation baseline by disabling default outbound access and enforcing NSG internet deny rules, requiring explicit outbound design; confirmed that NAT Gateway isn’t created in this profile.

  https://learn.microsoft.com/en-us/industry/nonprofit/azure-landing-zone-considerations

- **Deploy and configure Azure landing zone for Nonprofits**

  Updated deployment options to spell out NSG deny-by-default behavior in the foundation profile and to recommend enabling Key Vault private endpoints when DNS and network prerequisites are ready. Refined post-deployment results to clearly indicate which resources were created or deferred, emphasize setting up platform admin operational access, and highlight Key Vault firewall and networking status.

  https://learn.microsoft.com/en-us/industry/nonprofit/azure-landing-zone-deploy

- **Azure landing zone for Nonprofits overview**

  Strengthened the security overview by noting the shared platform Key Vault uses Azure RBAC with a deny-by-default firewall, with optional private endpoint and Defender coverage. Clarified that the public endpoint remains enabled but blocked and that simple foundation networking includes an application-subnet NSG, guiding secure-by-default operations.

  https://learn.microsoft.com/en-us/industry/nonprofit/azure-landing-zone-overview

- **Post-deployment tasks for Azure landing zone for Nonprofits**

  Added explicit security checks for Key Vault public endpoint mode (default deny, no bypass, empty allowlists) and reinforced using private endpoints for durable access. Expanded networking checks to verify application-subnet NSG association, confirm internet deny rules, review any higher-priority workload allows, and validate approved outbound connectivity.

  https://learn.microsoft.com/en-us/industry/nonprofit/azure-landing-zone-post-deployment

- **Plan and prepare to deploy Azure landing zone for Nonprofits**

  Expanded cost and readiness guidance for Key Vault network firewalls and private endpoints, stressing operational preparedness (DNS/network) and ownership of any allowlists. Detailed the foundation baseline’s lack of default outbound access and outbound components, requiring explicit egress design with minimal, scoped allow rules; reiterated when to enable the simple network baseline for private endpoints.

  https://learn.microsoft.com/en-us/industry/nonprofit/azure-landing-zone-prerequisites

- **Troubleshoot Azure landing zone for Nonprofits**

  Introduced troubleshooting for Key Vault public endpoint scenarios where data-plane operations fail due to deny-by-default firewalls, recommending private endpoints and private DNS. Added guidance for workloads lacking internet access in the foundation baseline, outlining steps to add necessary NSG allow rules and approved outbound options such as NAT Gateway.

  https://learn.microsoft.com/en-us/industry/nonprofit/azure-landing-zone-troubleshooting