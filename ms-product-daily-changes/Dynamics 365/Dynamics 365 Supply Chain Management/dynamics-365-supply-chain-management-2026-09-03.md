# Dynamics 365 Supply Chain Management
**Date created:** 2026-09-03 UTC  
**Tags:** Best Practices, Configuration, Guidance, Identity, Security, Troubleshooting  

## Major Changes

- **Install the Warehouse Management mobile app**
  
  Overhauled authentication and connection setup guidance to prioritize username/password authentication, with brokered authentication as an optional SSO enabler. Clarified AuthCloud options and when to use the global app versus a custom app registration, making tenant optional for Manual mode. Simplified the connection parameter table, removed certificate-based examples, and added realistic JSON samples for common connection scenarios. Streamlined configuration steps and aligned security guidance by de-emphasizing device code flow and certificate-based approaches.
  
  https://learn.microsoft.com/en-us/dynamics365/supply-chain/warehousing/install-configure-warehouse-management-app

- **User-based authentication for the Warehouse Management mobile app**
  
  Reframed authentication guidance to make username/password the primary method and brokered authentication optional for SSO and Conditional Access needs. Added Microsoft Entra QR code and PIN sign-in as a brokerless alternative that requires browser-based authentication and cannot be combined with a broker. Clarified device registration expectations, broker prerequisites, and when to use the global app or a custom app registration. Strengthened guidance around device code flow, session lifetimes, and migration steps to ensure secure, manageable sign-in experiences.
  
  https://learn.microsoft.com/en-us/dynamics365/supply-chain/warehousing/warehouse-app-authenticate-user-based

- **Brokered authentication and Conditional Access for the Warehouse Management mobile app**
  
  Expanded the article to cover brokered authentication alongside Conditional Access, explaining broker as an optional SSO choice within username/password authentication. Clarified division of responsibilities between app capabilities and IT policy design, and detailed device registration and broker requirements across platforms. Updated connection guidance, JSON format (ConnectionList), and default behaviors for AzureGlobal and custom app registrations. Enhanced Conditional Access examples and troubleshooting pointers to help admins configure and verify policies effectively.
  
  https://learn.microsoft.com/en-us/dynamics365/supply-chain/warehousing/warehouse-app-conditional-access-enable

- **Migrate the Warehouse Management mobile app from V3 to V4**
  
  Updated migration guidance to focus on a V3 support timeline and simplified reauthentication steps for cloud auth scenarios. Removed Windows-specific redirect URI setup and clarified that brokered auth is an option within username/password rather than a separate method. Eliminated the “New features in V4” section to keep the article focused on migration tasks and expectations. Minor text refinements improve clarity for rollout planning and authentication choices.
  
  https://learn.microsoft.com/en-us/dynamics365/supply-chain/warehousing/warehouse-app-migrating-from-v3-v4

## Moderate Changes

- **View, manage, and approve planned orders**
  
  Clarified that modified planned orders must be approved; otherwise, a subsequent planning run will ignore and overwrite edits. Added an exception for full regenerative runs where mid-run approvals or edits might not persist due to snapshot and reinsertion behavior, and advised scheduling planning outside business hours to avoid timing-related overwrites.
  
  https://learn.microsoft.com/en-us/dynamics365/supply-chain/master-planning/planning-optimization/approved-planned-order

- **Product receipt against purchase orders**
  
  Added guidance that canceling a product receipt posts a separate reversal transaction instead of modifying the original. The reversal may use a new number sequence value, so the original number might not appear in the product receipt report.
  
  https://learn.microsoft.com/en-us/dynamics365/supply-chain/procurement/product-receipt-against-purchase-orders

- **Warehouse Management mobile app release schedule**
  
  Updated the release table to add version 4.1.6.0 with dates and status set to Released, and changed 4.1.5.0 from Planned to Released. This keeps administrators aligned with current availability and rollout timelines.
  
  https://learn.microsoft.com/en-us/dynamics365/supply-chain/warehousing/warehouse-app-control-updates

- **Mass deploy the mobile app with user-based authentication**
  
  Updated MDM prerequisites to require app connection settings rather than authentication certificates. Removed the tip about setting IsDefaultConnection, simplifying managed configuration without changing core deployment steps.
  
  https://learn.microsoft.com/en-us/dynamics365/supply-chain/warehousing/warehouse-app-intune-user-based

- **Read connection settings from a QR code**
  
  Retitled to emphasize QR-based connection setup and removed obsolete properties (IsEditable, IsDefaultConnection) from all JSON examples. Guidance now aligns with current configuration requirements without changing supported connection types or procedure.
  
  https://learn.microsoft.com/en-us/dynamics365/supply-chain/warehousing/warehouse-app-qr-code

- **User-based authentication FAQ**
  
  Updated guidance to recommend username/password for all deployments, with brokered authentication optional for SSO and certain Conditional Access scenarios. Clarified QR code and PIN sign-in constraints, session persistence governed by token lifetimes and policy, device registration expectations, guest user host-tenant configuration, and deprecation of device code flow.
  
  https://learn.microsoft.com/en-us/dynamics365/supply-chain/warehousing/warehouse-app-user-based-auth-faq

- **What's new or changed in the Warehouse Management mobile app**
  
  Added release notes for version 4.1.6.0 (September 2, 2026), including a hotfix for a spinner control issue and support for external numeric keypads. This improves data entry reliability and usability for frontline workers.
  
  https://learn.microsoft.com/en-us/dynamics365/supply-chain/warehousing/warehouse-app-whats-new