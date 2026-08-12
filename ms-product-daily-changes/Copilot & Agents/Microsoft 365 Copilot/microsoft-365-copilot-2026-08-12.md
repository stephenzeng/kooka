# Microsoft 365 Copilot
**Date created:** 2026-08-12 UTC  
**Tags:** Best Practices, Configuration, Guidance, Identity, Security  

## Major Changes

- **Integrate ServiceNow with your Employee Self-Service deployment**
  
  Updated integration guidance to require Microsoft Entra user sign-in with OAuth 2.0, replacing prior Basic and app-token-only approaches. Deployment guidance now emphasizes least-privileged roles and streamlines admin actions to configuring and authorizing the connector in the Microsoft 365 admin center. Clarified that the ACL role is used by the Scripted REST API for advanced user-criteria evaluation rather than Basic auth. These changes improve security posture, align with delegated user context, and simplify setup.
  
  https://learn.microsoft.com/en-us/microsoft-365/copilot/employee-self-service/servicenow

- **Integrate ServiceNow HRSD and ITSM with your Employee Self-Service deployment**
  
  Overhauled configuration to standardize on Microsoft Entra ID user sign-in with delegated tokens and removed legacy methods (Basic, certificate-based app-token OAuth, and OAuth2 app registry). Consolidated steps for adding the ServiceNow connector app to permissions, clarified claim mapping (UPN or equivalent), and updated extension pack parameters to only reflect user sign-in. Prior coexistence workarounds were replaced with a pointer to the ServiceNow Knowledge documentation, and obsolete parameters were eliminated. The result is a more secure, consistent, and easier-to-administer deployment.
  
  https://learn.microsoft.com/en-us/microsoft-365/copilot/employee-self-service/servicenow-hrsd-itsm

## Moderate Changes

- **Choose a model for Copilot Cowork**
  
  Expanded model selection guidance with two new options—GPT 5.6 Sol for complex tasks and GPT 5.6 Terra for high-volume work—and refined descriptions of existing models to clarify best-fit use cases. Added clarifications on data retention, hosted models, and admin controls to support informed selection and governance.
  
  https://learn.microsoft.com/en-us/microsoft-365/copilot/cowork/cowork-models

- **Manage Microsoft 365 Copilot scenarios in the Microsoft 365 admin center**
  
  Added guidance on Vision in Microsoft 365 Copilot, including where to configure it in the admin center (Copilot > Settings > Copilot actions > Screen and camera sharing). Documented that Vision is enabled by default, how to disable it, and that turning off Vision does not impact voice features.
  
  https://learn.microsoft.com/en-us/microsoft-365/copilot/microsoft-365-copilot-page