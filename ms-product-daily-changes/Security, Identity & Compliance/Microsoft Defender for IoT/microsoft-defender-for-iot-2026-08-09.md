# Microsoft Defender for IoT
**Date created:** 2026-08-09 UTC  
**Tags:** Administration, Security  

## Moderate Changes

- **Maintain OT network sensors from the sensor console**

  Added clear prerequisites to ensure admins prepare correctly before starting procedures. Introduced a critical warning that resetting sensor data permanently removes learned data, allowlists, policies, and configurations. Expanded guidance on Horizon Plugins to explain their DPI-based protocol analysis and what data they expose, helping teams use plugins more effectively.

  https://learn.microsoft.com/en-us/azure/defender-for-iot/organizations/how-to-manage-individual-sensors

- **Manage EIoT monitoring support | Microsoft Defender for IoT**

  Added a warning that disabling Enterprise IoT security halts purpose-built alerts, vulnerabilities, and recommendations, ensuring admins understand the operational impact. Clarified that the Cancel plan page is only available to legacy Enterprise IoT plan customers.

  https://learn.microsoft.com/en-us/azure/defender-for-iot/organizations/manage-subscriptions-enterprise

- **Create and Manage Users on an On-premises Management Console**

  Clarified the article’s scope with a complete list of user management tasks and the permissions required for each. Corrected the session timeout procedure to use terminal access to the on-premises management console, preventing misconfiguration.

  https://learn.microsoft.com/en-us/azure/defender-for-iot/organizations/legacy-central-management/manage-users-on-premises-management-console

- **Create and manage Users on an OT Network Sensor**

  Expanded coverage to include creating, editing, and removing on-premises users, plus configuring Active Directory integration and recovering privileged access. Clarified role and prerequisite requirements to help administrators complete tasks successfully.

  https://learn.microsoft.com/en-us/azure/defender-for-iot/organizations/manage-users-sensor

- **Set up Single Sign-on for Microsoft Defender for IoT Sensor Console**

  Clarified permission setup by renaming the section to “Grant API permissions,” specifying the Microsoft Graph User.Read requirement, and directing admins to grant tenant-wide consent. These changes help ensure SSO works for all users without individual approval prompts.

  https://learn.microsoft.com/en-us/azure/defender-for-iot/organizations/set-up-sso