# Power Apps
**Date created:** 2026-08-04 UTC  
**Tags:** Administration, Programming, Security  

## Major Changes

- **Use managed identities for Azure with your Azure data lake storage**

  Reworked setup to use Microsoft.PowerPlatform.EnterprisePolicies PowerShell cmdlets instead of cloned scripts and Azure CLI, streamlining deployment and reducing prerequisites. Provider registration is now integrated into the New-IdentityEnterprisePolicy step, simplifying subscription configuration. Operational steps were replaced with cmdlets for policy creation, role assignment, and enablement, and troubleshooting now uses corresponding cmdlets for consistent management. Guidance clarifies required Azure roles to ensure smoother approvals and fewer permission errors.

  https://learn.microsoft.com/en-us/power-apps/maker/data-platform/azure-synapse-link-msi

- **Toggle modern control in Power Apps**

  Added a Tooltip property and refined LabelPosition using typed Power Fx enums for more reliable configuration. Renamed FontColor to Color and FontSize to Size to align with other modern controls and improve consistency. Behavior updates include predictable full-bound sizing and a read-only appearance in DisplayMode.View, resulting in clearer design-time choices and fewer runtime surprises. Documentation now provides clearer guidance on when to use a toggle and how its properties behave.

  https://learn.microsoft.com/en-us/power-apps/maker/canvas-apps/controls/modern-controls/modern-control-toggle

## Moderate Changes

- **Create or edit filters in model-driven app views | MicrosoftDocs**

  Combined Apply and Close into a single action, clarifying that Close removes a condition without confirmation. Added instructions to save filters with options to Save or Save and publish, improving clarity on making changes available to users.

  https://learn.microsoft.com/en-us/power-apps/maker/model-driven-apps/create-edit-view-filters

- **Checkbox modern control in Power Apps**

  Added a Tooltip property and documented consistent event behavior, including OnCheck/OnUncheck firing within galleries. Clarified default Checked behavior on app load and introduced property renames (FontColor to Color, FontSize to Size) for alignment with other modern controls.

  https://learn.microsoft.com/en-us/power-apps/maker/canvas-apps/controls/modern-controls/modern-control-checkbox

- **Recent updates to modern controls in canvas apps**

  Expanded the updates log to cover Toggle and Checkbox changes, including property renames (FontColor to Color, FontSize to Size), a new Tooltip property, sizing improvements, and read-only behavior in View mode. Updated cross-control tables to reflect these changes for faster discovery and consistent adoption.

  https://learn.microsoft.com/en-us/power-apps/maker/canvas-apps/controls/modern-controls/modern-control-updates

- **Improve solution performance, stability and reliability**

  Removed several SDL-related Web Resources rules from the checker guidance (for example, no-inner-html and no-insecure-url), reducing noise from deprecated or superseded checks. This helps makers focus on current, actionable rules for solution quality and security.

  https://learn.microsoft.com/en-us/power-apps/maker/data-platform/use-powerapps-checker