# Microsoft Entra
**Date created:** 2026-08-02 UTC  
**Tags:** Administration, Automation, Governance  

## New Articles

- **Reference for extending attribute mappings with custom call-outs using LCW extensibility workflows**

  Introduced a new reference that shows how to extend provisioning attribute mappings by invoking an Azure Logic App through a Lifecycle Workflows custom extension, enabling custom business logic to compute target attribute values. Provides prerequisites, an overview of extensibility workflows (including pre-provisioning scenarios), and step-by-step setup: create a consumption-based Logic App, configure a Lifecycle Workflows custom extension, build a Real-time Provisioning extensibility workflow, and map it to a target attribute with inputs. Highlights key limitations: not supported for Cloud Sync, not usable for matching attributes, applies only to create events, and includes cautions for custom security attributes. This helps admins tailor attribute values to organizational policies while understanding supported scenarios and constraints.

  https://learn.microsoft.com/en-us/entra/identity/app-provisioning/extend-application-attributes

## Moderate Changes

- **Configure an automatic assignment policy for an access package in entitlement management**

  Updated guidance clarifies that multiple automatic assignment policies are supported per access package as long as their scopes do not overlap. It warns that users matching more than one policy are not supported and may encounter access issues when falling out of scope for one policy while remaining in another. This helps avoid misconfiguration and ensures predictable entitlement outcomes.

  https://learn.microsoft.com/en-us/entra/id-governance/entitlement-management-access-package-auto-assignment-policy