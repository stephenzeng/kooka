# Microsoft Entra
**Date created:** 2026-08-07 UTC  
**Tags:** Administration, Security  

## New Articles

- **Configure Global Secure Access MCP firewall to secure Model Context Protocol traffic**

  Introduced a new how-to that explains how to use the Global Secure Access MCP firewall (preview) to inspect, audit, and enforce Allow/Block policies on Model Context Protocol traffic. The article details supported scenarios, prerequisites, and initial setup, then walks through creating and linking MCP policies that control protocol versions, transports, primitives (tools/resources/prompts), and server allow/deny lists. It also shows how to scope and enforce policies via security profiles and Conditional Access, with test examples for blocking specific tools and allowing only approved servers. Monitoring guidance covers Traffic logs and Generative AI Insights, and known limitations are documented to set expectations.

  https://learn.microsoft.com/en-us/entra/global-secure-access/how-to-configure-mcp-firewall

## Major Changes

- **Scoping users or groups to be provisioned with scoping filters in Microsoft Entra ID**

  Reworked scoping filters to a dedicated experience with Users and Groups tabs and a guided Configure Scoping Filters wizard, replacing the prior mapping-based flow. The new flow clarifies scope settings, assignment-based scoping, user/group selection, attribute-based rules, and review/save steps, with tightened operator descriptions. Saving a new filter now explicitly triggers a full sync and can deprovision users that fall out of scope, helping admins plan changes and avoid unintended impact.

  https://learn.microsoft.com/en-us/entra/identity/app-provisioning/define-conditional-rules-for-provisioning-user-accounts

## Moderate Changes

- **Configure cross-tenant synchronization**

  Updated navigation and workflow to align with the latest UI, including creating configurations via New configuration > Create and moving scope, notifications, and accidental deletion settings to Overview > Properties > Basics with an Apply action. Clarified attribute mapping using the Attribute mapping page, highlighted the AltSecIdFromNetId (alternativeSecurityIds) matching attribute, and renamed Constant Value to Constant attribute (default Member). Guidance now recommends syncing only assigned users and streamlines test provisioning and start steps with revised button labels.

  https://learn.microsoft.com/en-us/entra/identity/multi-tenant-organizations/cross-tenant-synchronization-configure

- **Tutorial - Customize Microsoft Entra attribute mappings in Application Provisioning**

  Aligned instructions with the Attribute Mapping page, describing mapping table columns and new edit/delete actions while noting required attributes. Moved custom attribute edits to Advanced Options and updated SCIM custom attribute steps, including the URN pattern. Restoring default mappings is now done from Attribute mapping and restarts synchronization.

  https://learn.microsoft.com/en-us/entra/identity/app-provisioning/customize-application-attributes

- **Understand how expression builder works with Application Provisioning in Microsoft Entra ID**

  Updated access steps to open Expression Builder from the left navigation menu instead of the attribute-mapping page’s advanced options. Removed outdated screenshots to match the current UI.

  https://learn.microsoft.com/en-us/entra/identity/app-provisioning/expression-builder

- **Target agent identities in Conditional Access policies**

  Revised licensing prerequisites to list supported options: Microsoft 365 E7 (including Agent 365 and Microsoft Entra Suite), or Microsoft Agent 365 with either Microsoft Entra P1 or Microsoft 365 E3. This clarifies eligibility and helps organizations select compliant licensing paths.

  https://learn.microsoft.com/en-us/entra/identity/conditional-access/howto-target-agent-identities