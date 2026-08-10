# Power Platform
**Date created:** 2026-07-17 UTC  
**Tags:** Administration, Governance  

## New Articles

- **Manage advanced connector policies programmatically**

  Introduced a comprehensive tutorial for managing Advanced Connector Policies (ACP) via the Power Platform API and Admin SDKs (PowerShell, C#, Python). Covers prerequisites and authentication, ACP policy structure and ConnectorManagement rules, and discovery of connector/action IDs via the Connector Catalog API. Provides end-to-end examples to create, assign, update, copy, and remove ACP policies across environment groups and single environments, including enabling specific connector actions and patching policies. Includes REST and SDK code samples, API version guidance (2024-10-01), and RBAC/service principal considerations to help automate governance at scale.

  https://learn.microsoft.com/en-us/power-platform/admin/programmability-tutorial-manage-advanced-connector-policies

## Major Changes

- **Power Platform and Dynamics 365 macro region geography**

  Expanded macro region geography to include Canada, Norway, Switzerland, and France, and clarified how macro regions are defined and selected. Updated eligibility to require Advanced Data Residency (ADR) for selecting datacenter regions across all Microsoft 365 seats in a tenant. Significantly expanded data residency and compliance guidance, including relationships between EU/EFTA, EUDB, and ADR, plus considerations for Australia and India. Added detailed provisioning flows for tenants with and without ADR, continuity expectations for existing environments, and a new FAQ covering cross-region connectivity and the capacity/availability-based placement algorithm to inform planning decisions.

  https://learn.microsoft.com/en-us/power-platform/admin/macro-regions

## Moderate Changes

- **Advanced connector policies**

  Added clear guidance on Enforcement modes (Mixed mode and ACP-only), how ACP works alongside classic data policies, and how to configure policies at environment group or single-environment scope. Highlighted immediate strict-allowlist enforcement on save/publish and recommended starting in mixed mode during migrations. Clarified inheritance and removal behavior and reorganized content for easier discovery, including where mixed-mode guidance appears and how runtime uses the most restrictive settings.

  https://learn.microsoft.com/en-us/power-platform/admin/advanced-connector-policies

- **Create users**

  Added guidance on non-licensed users in Microsoft Entra ID who are created in Dataverse (for example, via activities) with Disabled status and no access to Dataverse apps or admin portals. Explained that these users can be converted to regular users once a license is assigned.

  https://learn.microsoft.com/en-us/power-platform/admin/create-users