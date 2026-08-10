# Dynamics 365 Customer Service
**Date created:** 2026-07-14 UTC  
**Tags:** Administration, Agent, Automation, Security  

## Moderate Changes

- **Assign roles, enable users**

  Expanded guidance to include Dynamics 365 Contact Center and clarified privilege inheritance via teams/personas (prvAgent, prvSupervisor, prvAdmin). Added step-by-step instructions to manage access with Microsoft Entra security groups, including team mapping, role assignment, and an optional Power Automate flow to sync group members. Improves clarity on required roles, such as Customer Service Representative for case work.

  https://learn.microsoft.com/en-us/dynamics365/customer-service/implement/add-users-assign-roles

- **Enable consult with representatives and transfer of conversations**

  Updated inbox configuration to explicitly support both consult and transfer scenarios, including wrap-up. Clarifies conditions to route and close sessions, specifying participant mode equals consult and session state equals wrap-up. Improves accuracy and consistency for conversation workflows.

  https://learn.microsoft.com/en-us/dynamics365/customer-service/administer/enable-transfer-consult

- **Manage personas and custom security roles in Customer Service**

  Clarified custom role guidance by requiring assignment of persona privileges (prvAgent, prvSupervisor, or prvAdmin) for mapping to work. Emphasizes that custom roles are optional while ensuring correct access alignment.

  https://learn.microsoft.com/en-us/dynamics365/customer-service/administer/role-persona-mapping