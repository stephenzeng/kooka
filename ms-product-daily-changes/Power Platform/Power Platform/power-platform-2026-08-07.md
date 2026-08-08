# Power Platform
**Change date:** 2026-08-07 UTC  
**Tags:** Administration  

## New Articles

- **Understand agent counts across admin surfaces**

  Introduced guidance that explains why agent counts differ between Power Platform inventory and the Microsoft 365 admin center. Clarifies that Power Platform inventory shows agents built on Power Platform (including drafts), while Microsoft 365 admin center lists all agents available to users (Microsoft first‑party and ISV, published/shared only). Provides a comparison table for audience, scope, draft inclusion, and first‑party/ISV coverage, plus recommendations on which count to use in different reporting scenarios.

  https://learn.microsoft.com/en-us/power-platform/admin/inventory-agent-counts

## Major Changes

- **Power Platform inventory schema reference**

  Added connectors as a distinct inventory resource type with a full schema, including connector fields (ID, description, publisher, tier, release tag, deprecation) and operations metadata. Clarified the two ways connectors appear in inventory: as resources and as references used by other resources. Updated type tables and notes to reflect connectors as catalog entities and streamlined guidance by removing repeated notes about quarantined visibility. This improves accuracy for reporting, governance, and automation scenarios that depend on connector details.

  https://learn.microsoft.com/en-us/power-platform/admin/inventory-schema

- **Power Platform inventory**

  Reorganized and expanded documentation to detail inventory resource types and capabilities, adding Connectors (preview) as a tracked type. Enhanced discovery and operations with a new global search that scans the entire inventory, clarified navigation, and improved export guidance (full CSV and programmatic options via Admins V2 connector, Power Platform API, and Azure Resource Graph). Updated resource details with linked names and a multi-tab panel (Overview, Connectors, Usage), and added actions to delete or block published agents and canvas apps with clear blocking behavior. Restructured known limitations, including clarifications for model-driven apps ownership and capture scope, to set accurate expectations for admins.

  https://learn.microsoft.com/en-us/power-platform/admin/power-platform-inventory