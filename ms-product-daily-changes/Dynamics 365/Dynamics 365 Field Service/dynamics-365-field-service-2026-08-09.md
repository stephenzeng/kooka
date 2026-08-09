# Dynamics 365 Field Service
**Date created:** 2026-08-09 UTC  
**Tags:** Administration, Automation  

## Moderate Changes

- **Create work order templates with incident types**

  Updated end-to-end procedures and field labels to match the current UI, including using Incident type then Save and the renamed Rating Value field. Clarified how incident items copy to agreements and provided guidance for safely changing an incident type on a work order by removing related items and recreating the incident. Refined customer asset lookup configuration using Power Apps form properties and added concise tips to reduce setup errors.

  https://learn.microsoft.com/en-us/dynamics365/field-service/configure-incident-types

- **Enable push notifications**

  Streamlined setup steps in Power Apps and Power Automate, adding explicit actions like selecting Objects before creating a connection reference and signing in/selecting the environment. Clarified the sequence for creating the connection in a new window, refreshing, and configuring a Dataverse-triggered flow, improving reliability without changing feature scope.

  https://learn.microsoft.com/en-us/dynamics365/field-service/mobile/enable-push-notifications

- **Work order incident type overview**

  Added guidance on how incident types interact with agreements, including when to set Copy Incident Items to Agreement to Yes or No with practical examples. Clarified relationships and workflows across incident-related entities and how primary incidents drive business logic.

  https://learn.microsoft.com/en-us/dynamics365/field-service/incident-type-overview

- **Create entitlements for work orders**

  Clarified entitlement application behavior, noting that the entitlement’s Price List overrides the work order’s price list. Expanded scenario-based steps for creating entitlement applications (including selecting the appropriate asset category) and explained how they work with the primary customer requirement to ensure correct billing and coverage.

  https://learn.microsoft.com/en-us/dynamics365/field-service/work-order-entitlements