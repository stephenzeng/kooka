# Microsoft Defender for Cloud Apps
**Date created:** 2026-08-09 UTC  
**Tags:** Automation, Security  

## Moderate Changes

- **Identity-managed devices with Conditional Access app control | Microsoft Defender for Cloud Apps**
  Updated guidance to configure Conditional Access app control using device-management signals, clearly separating Microsoft Entra (Intune-compliant or Entra hybrid joined) and non-Entra (client certificate) scenarios. Clarified certificate handling by requiring upload of root or intermediate CA certificates and aligned policy steps to reference these certificates. This improves setup accuracy and helps ensure device-based access policies are reliably enforced.
  https://learn.microsoft.com/en-us/defender-cloud-apps/conditional-access-app-control-identity

- **Discovered app filters and queries | Microsoft Defender for Cloud Apps**
  Expanded instructions for using basic and advanced filters to refine Discovered apps by risk, category, compliance, usage, and more. Added guidance on saving custom queries and using suggested queries to quickly surface risky or high-priority apps.
  https://learn.microsoft.com/en-us/defender-cloud-apps/discovered-app-queries

- **Configure automatic log upload using Docker in Azure**
  Added a prerequisite requiring root access to the log collector machine and clarified that Docker CE is installed later in the process. Refined the collector configuration command steps to reduce setup errors and streamline deployment.
  https://learn.microsoft.com/en-us/defender-cloud-apps/discovery-docker-ubuntu-azure

- **Configure automatic log upload using on-premises Podman on Linux | Microsoft Defender for Cloud Apps**
  Expanded the overview to explain continuous upload of firewall and proxy logs to Cloud Discovery and when to use Podman on RHEL 7.1+ instead of Docker. Outlined the key steps to set up a data source, deploy the collector container, and verify successful uploads for smoother implementation.
  https://learn.microsoft.com/en-us/defender-cloud-apps/discovery-linux-podman

- **Integrate with Microsoft Power Automate for custom alert automation**
  Added a prerequisite to create an API token in Defender for Cloud Apps and referenced it in authentication steps. Clarified the “Before you begin” requirements and highlighted use of Power Automate connectors to ensure reliable, authenticated automation flows.
  https://learn.microsoft.com/en-us/defender-cloud-apps/flow-integration

- **Protect your Atlassian environment | Microsoft Defender for Cloud Apps**
  Reworked onboarding guidance to explain how to connect Atlassian and what activities are monitored across Confluence, Jira, and Bitbucket, including required permissions. Strengthened security posture guidance by directing admins to connect via App Connector before using Microsoft Secure Score, and documented API key lifecycle best practices (1-year default validity, 6-month rotation, and clear revoke-and-replace steps). These updates help improve initial setup, governance, and key hygiene.
  https://learn.microsoft.com/en-us/defender-cloud-apps/protect-atlassian

- **Protect your Box environment | Microsoft Defender for Cloud Apps**
  Added prerequisites specifying a Box Admin or fully privileged Co-Admin and explained the impact on API testing and file scanning. Clarified that App Connector APIs are the supported integration method, updated the connection procedure naming with anchors for direct linking, and improved accessibility with updated alt text. These changes make connection steps clearer and more reliable.
  https://learn.microsoft.com/en-us/defender-cloud-apps/protect-box