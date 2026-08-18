# Dynamics 365 Supply Chain Management
**Date created:** 2026-08-18 UTC  
**Tags:** Configuration, Guidance, Identity  

## Moderate Changes

- **Supplier Engagement deployment overview, prerequisites, and licensing (preview)**

  Updated prerequisites to require a Dataverse environment with US English (LCID 1033) during public preview to avoid mixed-language experiences. Recommends using a US English base language for testing environments. Notes that more languages will be supported at general availability.

  https://learn.microsoft.com/en-us/dynamics365/supply-chain/supplier-engagement/deploy-overview

- **User-based authentication for the Warehouse Management mobile app**

  Clarifies that the Warehouse Management mobile app does not support shared device mode and recommends assigning one Microsoft Entra ID user account per device in shared scenarios. Updates device code flow guidance to state it cannot be combined with brokered authentication or with QR code plus PIN sign-in. These changes help ensure consistent, supported authentication configurations.

  https://learn.microsoft.com/en-us/dynamics365/supply-chain/warehousing/warehouse-app-authenticate-user-based