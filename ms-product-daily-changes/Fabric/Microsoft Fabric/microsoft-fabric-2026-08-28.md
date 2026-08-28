# Microsoft Fabric
**Date created:** 2026-08-28 UTC  
**Tags:** Best Practices, Compliance, Configuration, Get Started, Governance, Guidance, Identity, Security  

## New Articles

- **Author and share Fabric Apps templates**

  Introduced a step-by-step guide to author, catalog, and distribute Fabric Apps templates using the Rayfin CLI. Explains template structure and scaffolding behaviors, including manifests, placeholders, and post-scaffold tasks. Provides instructions for building multi-template catalogs, registering template sources across registry tiers, and distributing via Git with ref pinning and private repo support. Includes a reference schema and links to related CLI topics to streamline template creation and sharing.

  https://learn.microsoft.com/en-us/fabric/apps/author-templates

- **Configure data source access for a Real-Time Dashboard**

  Added guidance to configure Real-Time Dashboard data sources to use the dashboard editor’s identity so viewers can access data without direct permissions. Covers prerequisites, creating cloud connections (for Azure Data Explorer/Kusto), and applying connections to data sources, with notes on default pass-through identity and per–data source connections. Helps teams simplify access management and ensure dashboards render consistently for viewers.

  https://learn.microsoft.com/en-us/fabric/real-time-intelligence/dashboard-data-source-access

- **Insert Checkbox Columns in a Planning Sheet**

  Added instructions to insert and configure checkbox columns in planning sheets for yes/no scenarios. Details how to add columns, select or clear values per row, and adjust properties over time. Highlights common use cases like filtering and using checks with Writeback to drive decisions.

  https://learn.microsoft.com/en-us/fabric/iq/plan/planning-how-to-insert-columns/how-to-insert-checkbox-columns

- **Insert Date Columns in a Planning Sheet**

  Added a how-to for inserting and configuring date columns, including picker-based entry and property management. Documents date formatting, min/max constraints, default values (static or measure-based), and general input properties like on-change formulas and totals behavior. Clarifies how invalid formats are handled and how defaults can be overridden to keep data clean.

  https://learn.microsoft.com/en-us/fabric/iq/plan/planning-how-to-insert-columns/how-to-insert-date-columns

- **Insert Text Columns in a Planning Sheet**

  Added guidance for creating text input columns with robust validation and configuration options. Explains shared input properties plus text-specific settings like word wrap, Prevent Null (for short text), and length and pattern validation (including email, URL, and custom regex). Helps modelers enforce data quality and streamline data entry with clear, reject-on-invalid rules.

  https://learn.microsoft.com/en-us/fabric/iq/plan/planning-how-to-insert-columns/how-to-insert-text-columns

## Major Changes

- **Create a OneDrive or SharePoint shortcut**

  Overhauled authentication and setup to use certificate-based service principals secured in Azure Key Vault, replacing key/secret methods. Unified configuration steps for workspace identity and service principals, including adding Sites.Selected permissions and granting admin consent in Azure. Expanded PowerShell examples and added guidance for creating certificate-based connections through Manage Connections and Gateways, with rollout notes and updated limitations.

  https://learn.microsoft.com/en-us/fabric/onelake/shortcuts/create-onedrive-sharepoint-shortcut

- **Real-Time Dashboard permissions**

  Reworked from a procedural how-to into a conceptual overview that separates dashboard permissions from data source permissions. Introduces pass-through identity versus dashboard editor’s identity models and explains their implications. Streamlines detailed setup into references and scenarios, with updated visuals to clarify permission layers and data source settings.

  https://learn.microsoft.com/en-us/fabric/real-time-intelligence/dashboard-permissions

- **Insert Data Input Columns in a Planning Sheet Introduction**

  Expanded input configuration with a new Simulate type and additional controls like default values, totals/subtotals entry, and on-change formulas. Consolidated immutability guidance and added instructions for modifying column properties via Manage Measures and the column gripper. Removed outdated sections and reorganized content to match current capabilities.

  https://learn.microsoft.com/en-us/fabric/iq/plan/planning-how-to-insert-columns/how-to-insert-data-input-columns

## Moderate Changes

- **Buy Fabric capacity in Azure**

  Enhanced prerequisites and purchasing guidance to clarify Azure subscription and tenant alignment, and that buying capacity provides compute resources. Added requirements to register the Microsoft.Fabric resource provider, select supported regions, and ensure sufficient CU quota with guidance on increase requests. Linked to enabling Fabric for the organization to complete setup.

  https://learn.microsoft.com/en-us/fabric/enterprise/buy-capacity

- **External data sharing in Microsoft Fabric**

  Clarified cross-tenant enforcement boundaries: data is shared in place, and provider-tenant governance (like labels and DLP) doesn’t run in the consumer tenant. Emphasized that providers can block external consumption at the source, and once access is allowed, the consumer tenant’s governance and compliance policies apply. Helps admins set appropriate controls on both sides of sharing.

  https://learn.microsoft.com/en-us/fabric/governance/external-data-sharing-overview

- **Enable Microsoft Fabric for your organization**

  Rewrote to explain that enabling Fabric requires both a tenant setting and capacity that supports Fabric workloads. Clarified supported capacity types and that per-user licenses don’t provide Fabric capacity, and updated prerequisites to require a Fabric administrator Microsoft Entra role. Renamed sections for tenant and capacity enablement and refreshed notes for current portal terminology and regions.

  https://learn.microsoft.com/en-us/fabric/admin/fabric-switch

- **Insert Dropdown List Columns in a Planning Sheet**

  Expanded configuration with a new Prevent Null option for single-select lists that requires a default value. Documented additional properties like input type, on-change formula, and allowing entries on totals/subtotals, with standardized terminology. Simplifies setup while enforcing required selections where appropriate.

  https://learn.microsoft.com/en-us/fabric/iq/plan/planning-how-to-insert-columns/how-to-insert-dropdown-columns

- **Insert formula columns in planning sheet**

  Removed an outdated note about weighted average behavior to align with current aggregation capabilities. Reduces confusion and ensures guidance reflects actual configuration options.

  https://learn.microsoft.com/en-us/fabric/iq/plan/planning-how-to-insert-columns/how-to-insert-formula-columns

- **Insert Number Columns in a Planning Sheet**

  Added a dedicated configuration section for number columns, including row/column aggregation methods, distributing parent values, and min/max constraints with error handling. Updated cross-links and reorganized insertion and modification guidance for clarity. Helps authors define precise numeric behaviors and guardrails.

  https://learn.microsoft.com/en-us/fabric/iq/plan/planning-how-to-insert-columns/how-to-insert-number-columns

- **Data science tutorial - get started**

  Updated the Models and experiments section to reference MLflow 3 in Fabric Data Science. Highlights new tracking features like LoggedModel and generative AI tracing to improve experiment management and observability.

  https://learn.microsoft.com/en-us/fabric/data-science/tutorial-data-science-introduction