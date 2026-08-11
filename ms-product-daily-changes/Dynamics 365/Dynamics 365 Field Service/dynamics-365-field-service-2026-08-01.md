# Dynamics 365 Field Service
**Date created:** 2026-08-01 UTC  
**Tags:** Administration, Monitoring, Other, Programming, Security  

## New Articles

- **Post a work order and generate an invoice**

  Introduced a step-by-step guide to post completed work orders and automatically generate invoices, including prerequisites and required roles. Clarifies system actions during posting (invoice creation, actuals generation, and Closed By/On updates) and how work order products and services map to invoice lines, including billing basis and handling of Used vs. Estimated lines. Explains pricing dependencies such as price lists and entitlements, how to review/confirm invoices, and options to integrate with Project Operations, Business Central, or third-party ERPs via Power Automate and Dataverse APIs. Includes a troubleshooting section covering posting, pricing, inventory, and actuals configuration issues.

  https://learn.microsoft.com/en-us/dynamics365/field-service/post-work-order-invoice

- **View scheduling warnings in the mobile app**

  Added guidance for technicians to view scheduling warnings on work orders opened from Project Operations tasks when there are date or dependency conflicts. Shows how to use the Notifications section to review predecessor and successor tasks and explains that work orders can’t be completed until predecessors are finished. Includes illustrative visuals to help users quickly identify and resolve scheduling blockers.

  https://learn.microsoft.com/en-us/dynamics365/field-service/project-operations-integration-view-warnings

- **Troubleshoot Slow or Unnecessary Mobile App Network Calls**

  Published a troubleshooting playbook to capture and analyze mobile network traces and pinpoint long-running, pending, or failed requests. Explains how to distinguish local vs. remote responses (ServiceWorker on Android, localhost on iOS) and separate customization-driven from platform-driven traffic. Provides procedures to reproduce issues under degraded or offline conditions, a decision table and quick checklist, and recommended next steps for remediation or escalation.

  https://learn.microsoft.com/en-us/troubleshoot/dynamics-365/field-service/mobile-app/unnecessary-network-calls

## Major Changes

- **Search for resource availability and create bookings for requirement groups**

  Updated the API to make the Version parameter optional with clear rules for version resolution. If omitted, the latest version is used; specifying a major version selects the highest minor and patch; specifying major and minor selects the highest patch; specifying all three targets the exact version. This streamlines requests while preserving control for precise version targeting and compatibility management.

  https://learn.microsoft.com/en-us/dynamics365/field-service/search-resource-availability-requirement-groups-api

## Moderate Changes

- **Best practices and limitations for the offline profile**

  Added an important note clarifying that tables filtered with “Related rows only” inherit the parent table’s filter. For example, restricting work orders to Scheduled limits related accounts and contacts accordingly. Administrators should review related-row filters to ensure technicians have the data they need offline.

  https://learn.microsoft.com/en-us/dynamics365/field-service/mobile/best-practices-limitations-offline-profile

- **Create products or services for work orders**

  Added a comparison table to distinguish work order products (parts/materials) from work order services (labor), including tracking method, inventory impact, and billing approach. This helps teams choose the right line type for accurate pricing, inventory control, and reporting.

  https://learn.microsoft.com/en-us/dynamics365/field-service/create-product-or-service

- **Search resource availability API**

  Updated the Version parameter to be optional and default to the current version, with clearer behavior when specifying major, minor, and patch numbers. This reduces required inputs for typical scenarios while preserving explicit version control when needed.

  https://learn.microsoft.com/en-us/dynamics365/field-service/search-resource-availability-api

- **Security roles and column-level security profiles**

  Added minimum privilege requirements for schedule board access, including specific Read/Create/Write permissions per table. Highlights that missing privileges can cause errors or a blank schedule board and advises assigning access via built-in or custom Field Service roles, with a link to setup guidance.

  https://learn.microsoft.com/en-us/dynamics365/field-service/security-permissions