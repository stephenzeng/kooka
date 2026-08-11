# Dev and Admin for Dynamics 365 Business Central
**Date created:** 2026-08-11 UTC  
**Tags:** Automation, Configuration, Get Started, Governance, Guidance, Identity, Monitoring, Security, Troubleshooting  

## New Articles

- **approvalEntry Resource Type Reference**

  Introduced full API v2.0 reference for approvalEntry, defining its purpose and structure. Lists supported method availability and provides a complete property set with types and descriptions. Includes a full JSON representation and links to the related GET operation to streamline discovery and implementation.

  https://learn.microsoft.com/en-us/dynamics365/business-central/dev-itpro/api-reference/v2.0/resources/dynamics_approvalentry

- **Get Approval Entries with the Business Central API**

  Documented the GET operation for approvalEntry, including the endpoint for a single entry and guidance on omitting the ID to list all entries. Clarifies required authorization, response behavior (200 OK), and the payload shape to improve client implementation. Provides end-to-end request/response examples and links to related API guidance for faster onboarding.

  https://learn.microsoft.com/en-us/dynamics365/business-central/dev-itpro/api-reference/v2.0/api/dynamics_approvalentry_get

- **approvalUserSetup Resource Type**

  Added a comprehensive reference for approvalUserSetup in API v2.0, explaining its role in defining approval limits and relationships. Details all properties, including identifiers, approval limits and unlimited flags across sales, purchase, and request flows, plus admin and contact fields. Includes a complete JSON example and a related link to help teams model approval configuration programmatically.

  https://learn.microsoft.com/en-us/dynamics365/business-central/dev-itpro/api-reference/v2.0/resources/dynamics_approvalusersetup

- **Get Approval User Setups with the Business Central API**

  Introduced the GET endpoint documentation for approvalUserSetup, supporting retrieval of a single setup or listing all setups. Specifies authentication requirements, response structure, and provides full sample requests and responses for accuracy. Notes environment-specific endpoints and links to related resources to guide correct usage across tenants.

  https://learn.microsoft.com/en-us/dynamics365/business-central/dev-itpro/api-reference/v2.0/api/dynamics_approvalusersetup_get

- **postedApprovalEntry Resource Type**

  Published reference for postedApprovalEntry to expose finalized approval records via API v2.0. Enumerates identifiers, document context, approver details, statuses, timestamps, amounts, currency, workflow types, and iteration metadata. Includes a full JSON example and related link, enabling analytics and audit scenarios that depend on completed approvals.

  https://learn.microsoft.com/en-us/dynamics365/business-central/dev-itpro/api-reference/v2.0/resources/dynamics_postedapprovalentry

- **Get Posted Approval Entries with the Business Central API**

  Added GET operation documentation for postedApprovalEntry to retrieve individual items or list all posted approval entries. Clarifies authorization and response semantics and provides practical request/response samples. This helps developers automate reporting and auditing of completed approvals with confidence.

  https://learn.microsoft.com/en-us/dynamics365/business-central/dev-itpro/api-reference/v2.0/api/dynamics_postedapprovalentry_get

- **workflowApprover Resource Type**

  Introduced reference documentation for workflowApprover in API v2.0 to surface approver configuration for workflows. Details key properties such as workflow context, approver type and limits, user and sequence fields, and modification metadata. Includes a JSON example and related link to accelerate integration with approval routing logic.

  https://learn.microsoft.com/en-us/dynamics365/business-central/dev-itpro/api-reference/v2.0/resources/dynamics_workflowapprover

- **Get Workflow Approvers with the Business Central API**

  Documented the GET endpoint for workflowApprover, with support for fetching a single approver or enumerating all approvers. Outlines required headers, expected success responses, and example payloads to reduce implementation errors. Links to broader API guidance and the resource reference for end-to-end discoverability.

  https://learn.microsoft.com/en-us/dynamics365/business-central/dev-itpro/api-reference/v2.0/api/dynamics_workflowapprover_get

## Major Changes

- **Get Security Group Members with the Automation API**

  Updated the endpoint to use composite keys (securityGroupCode and userSecurityId) instead of a generic ID, aligning the route with the underlying data model. Request and response examples were revised accordingly and now include userName and userFullName for better identity context. The title and description were clarified to emphasize retrieving a specific security group member. These changes improve precision, reduce ambiguity in API calls, and make results more actionable for identity management.

  https://learn.microsoft.com/en-us/dynamics365/business-central/dev-itpro/administration/api/dynamics_securitygroupmember_get

## Moderate Changes

- **company resource type**

  Expanded the Navigation section with workflowApprovers, postedApprovalEntries, approvalEntries, and approvalUserSetups relationships. This enables straightforward traversal to approval configuration and history from a company, simplifying integrations and reporting.

  https://learn.microsoft.com/en-us/dynamics365/business-central/dev-itpro/api-reference/v2.0/resources/dynamics_company

- **Get a security group with the automation API**

  Corrected the HTTP request syntax by quoting the securityGroupId and expanded the sample response with additional properties for clarity. These fixes help ensure valid requests and more predictable parsing for automation scenarios.

  https://learn.microsoft.com/en-us/dynamics365/business-central/dev-itpro/administration/api/dynamics_securitygroup_get

- **Welcome to the API (v2.0) for Business Central**

  Clarified that APIs are enabled by default for online environments and provided steps for enabling them on-premises. Added an “Available APIs” section directing readers to the table of contents to quickly discover endpoints and operations.

  https://learn.microsoft.com/en-us/dynamics365/business-central/dev-itpro/api-reference/v2.0/

- **Introduction to automation APIs**

  Added an “Inspect security and permissions” section documenting read-only endpoints for tenant-wide insights: usersPermissions, userPermissionSets, accessControls, aggregatePermissionSets, and expandedPermissionSets. Guidance includes license coverage, exclusions, and an example GET request to accelerate adoption.

  https://learn.microsoft.com/en-us/dynamics365/business-central/dev-itpro/administration/itpro-introduction-to-automation-apis

- **Analyze API metadata validation telemetry**

  Documented telemetry event RT0037 for invalid API metadata pages, including general/custom dimensions and sample KQL. This helps teams quickly detect and investigate metadata issues impacting API surfaces.

  https://learn.microsoft.com/en-us/dynamics365/business-central/dev-itpro/administration/telemetry-api-metadata-validation-trace

- **Analyzing User Checklist Telemetry**

  Added two new events for checklist item status updates, with and without guided experience context. Detailed dimensions and status transition fields help administrators track user progress and diagnose onboarding friction.

  https://learn.microsoft.com/en-us/dynamics365/business-central/dev-itpro/administration/telemetry-user-checklist-trace

- **Delete and recover environments**

  Removed outdated limits on the count of recently deleted environments and related recovery instructions. This prevents reliance on deprecated constraints and aligns guidance with current recovery behavior.

  https://learn.microsoft.com/en-us/dynamics365/business-central/dev-itpro/administration/tenant-admin-center-environments-delete