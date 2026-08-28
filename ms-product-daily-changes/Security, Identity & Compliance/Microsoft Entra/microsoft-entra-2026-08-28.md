# Microsoft Entra
**Date created:** 2026-08-28 UTC  
**Tags:** Configuration, Guidance, Identity  

## Major Changes

- **Microsoft Entra ID SCIM API reference**
  
  Updated SCIM guidance to make enterprise and Microsoft Entra schemaExtensions optional, reducing implementation requirements for user provisioning. Clarified that mailNickname is optional at user creation and will be derived from userName if not provided, with updated examples that use only the core User schema. Added guidance that mailNickname cannot be removed via PATCH after a user is created, preventing unintended attribute removals and aligning expectations for lifecycle operations. These changes simplify integrations and improve consistency across provisioning scenarios.
  
  https://learn.microsoft.com/en-us/entra/identity/app-provisioning/entra-id-scim-api-reference

## Moderate Changes

- **Exchange hybrid writeback with cloud sync**
  
  Expanded attribute synchronization guidance with a new section on Entra2ADExchangeOnlineAttributeWriteback (LES Writeback), enabling Exchange Online to serve as the source of truth for specific Exchange attributes that are written back to on-premises AD via cloud sync. Clarifies how LES Writeback differs from the preview Exchange hybrid writeback template and lists the supported attributes and mappings to streamline hybrid configuration decisions.
  
  https://learn.microsoft.com/en-us/entra/identity/hybrid/cloud-sync/exchange-hybrid