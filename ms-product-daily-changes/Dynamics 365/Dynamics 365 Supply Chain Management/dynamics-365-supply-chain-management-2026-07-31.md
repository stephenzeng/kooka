# Dynamics 365 Supply Chain Management
**Date created:** 2026-07-31 UTC  
**Tags:** Administration, Security  

## Major Changes

- **User-based authentication for the Warehouse Management mobile app**
  
  Updated guidance to prioritize username/password with brokered authentication over device code flow to reduce phishing risk. Added details on brokered options (shared device mode, Windows Web Account Manager, and QR code + PIN) and expanded SSO coverage for Android and iOS. Introduced prominent warnings that device code flow is vulnerable and will be blocked by default for new Microsoft Entra tenants starting July 1, 2026, with temporary unblocking guidance and associated risks. Refreshed authentication scenarios and expanded requirements/restrictions for device code to support informed decision-making.
  
  https://learn.microsoft.com/en-us/dynamics365/supply-chain/warehousing/warehouse-app-authenticate-user-based

- **User-based authentication FAQ**
  
  Expanded the FAQ to explain why device code flow is no longer recommended, the phishing risks involved, and that it will be blocked by default in new tenants starting July 1, 2026. Recommends migrating to username/password with brokered authentication, including shared device mode and QR/PIN sign-in, and outlines how admins could temporarily unblock device code by disabling security defaults—while strongly advising against it. Helps admins plan a secure transition away from device code flow.
  
  https://learn.microsoft.com/en-us/dynamics365/supply-chain/warehousing/warehouse-app-user-based-auth-faq

## Moderate Changes

- **Install the Warehouse Management mobile app**
  
  Updated authentication guidance to favor username/password with brokered authentication, and changed the default JSON ConnectionType from DeviceCode to UsernamePassword. Added security notes about device code phishing risks and default blocking in new tenants, clarified brokered sign-in options (shared device mode, QR code + PIN), and consolidated device access revocation guidance under user-based authentication.
  
  https://learn.microsoft.com/en-us/dynamics365/supply-chain/warehousing/install-configure-warehouse-management-app