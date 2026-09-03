# Microsoft 365 Copilot
**Date created:** 2026-09-03 UTC  
**Tags:** Best Practices, Billing, Compliance, Configuration, Governance, Guidance, Monitoring, Security  

## New Articles

- **Determine access controls for Copilot Cowork**

  Introduced consolidated guidance that establishes spending policies as the definitive access control for Copilot Cowork—any policy selecting Cowork grants access, regardless of low credit limits. Clarifies that discovery settings only control feature visibility and model settings only manage which models are available, not who can use Cowork. Explains policy precedence for users in multiple policies and notes that credit limit enforcement can be asynchronous. Includes a worked example and related links to governance, model selection, and usage-based billing guidance.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/cowork/cowork-access

- **Manage content sharing for Microsoft Copilot**

  Added an admin how-to for managing session and response sharing without expanding access to underlying Microsoft 365 content. Defines the primary control “Allow users to share Copilot responses,” provides step-by-step enable/disable instructions in the admin center, and notes that sharing is on by default. Provides prerequisites and monitoring guidance using Microsoft Purview audit logs to track sharing events, link access, and blocked attempts, with related resources for deeper learning.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/microsoft-copilot-manage-content-sharing

## Major Changes

- **Anthropic models in Microsoft Online Services**

  Restructured content to clearly separate scenarios where Anthropic acts as a Microsoft subprocessor under the Product Terms and DPA from those where Anthropic is an independent processor. Introduced a new section on Anthropic “Fable-class” models and clarified that “Anthropic models with Data Retention” are off by default, require explicit tenant opt-in, and are covered by Anthropic’s commercial terms and DPA. Replaced legacy “Preview models with Data Retention” terminology, added detailed admin controls and user scoping guidance, and moved general preview guidance to a new “Allow the use of Preview models” section. Removed outdated preview-specific content and updated instructions to reflect the new model categories and controls.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/connect-to-ai-subprocessor

- **Manage Copilot Cowork for your organization**

  Updated governance guidance to make clear that spending policies grant access to Copilot Cowork and are not merely budgeting tools. Deprecated agent-based access control from Frontier/Preview; access is now governed solely by spending policies. Added a migration path to translate previous allow lists into spending policies using Microsoft Entra security groups, and clarified that model settings affect model visibility only while Auto continues choosing among available models. Expanded related content with a link explaining how access to Copilot Cowork is determined.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/cowork/cowork-admin-governance

- **Available plugins for Copilot Cowork**

  Significantly expanded the partner plugins catalog with dozens of new third-party integrations across analytics, development, finance, HR, legal, marketing, and productivity. Refined plugin names and descriptions and improved catalog guidance for administrators evaluating integrations. Core Microsoft plugin details remain functionally unchanged.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/cowork/cowork-available-plugins

## Moderate Changes

- **Choose a model for Copilot Cowork**

  Clarified that the Anthropic model family toggle is a tenant-wide setting that controls model availability, not access, and cannot be scoped to subsets of users. When disabled, users continue with permitted models and Auto selects from those; also added a reference on how Cowork access is determined and refined wording on data retention and Claude Fable 5 behavior.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/cowork/cowork-models

- **Deployment overview for the Microsoft Copilot app**

  Expanded installation restrictions to note that deploying the Microsoft 365 Copilot app on devices with Microsoft 365 Apps is not enabled for customers in the European Economic Area and government clouds (GCC, GCC High, DoD).

  https://learn.microsoft.com/en-us/microsoft-365/copilot/deploy-microsoft-365-copilot-app