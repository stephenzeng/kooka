# Dynamics 365 Supply Chain Management
**Date created:** 2026-08-15 UTC  
**Tags:** Best Practices, Configuration, Deprecation, Guidance, Identity, Security  

## Major Changes

- **User-based authentication for the Warehouse Management mobile app**
  Updated guidance now prioritizes username/password with brokered authentication (SSO) and treats device code flow as legacy for backward compatibility only. A new legacy section explains security risks (notably phishing), default blocking in new Microsoft Entra tenants starting July 1, 2026, platform gaps (no iOS support and Android limits for on-prem), and lack of SSO. The article adds a detailed migration path to move from device code flow to username/password with broker using ConnectionType and UseBroker settings, plus rollout recommendations. Minor clarifications improve revocation steps for device or worker accounts.
  https://learn.microsoft.com/en-us/dynamics365/supply-chain/warehousing/warehouse-app-authenticate-user-based

- **User-based authentication FAQ**
  The FAQ now recommends username/password with brokered authentication (SSO) for all deployments and moves device code flow into a dedicated legacy explanation. It details why device code is discouraged (phishing exposure, default blocking in new tenants, no iOS support, no SSO) and notes it remains only for backward compatibility. Guidance includes how admins could temporarily unblock device code (with security caveats) and provides migration steps to update ConnectionType/UseBroker and redistribute configurations. On-premises guidance is aligned to username/password instead of device code.
  https://learn.microsoft.com/en-us/dynamics365/supply-chain/warehousing/warehouse-app-user-based-auth-faq

## Moderate Changes

- **Install the Warehouse Management mobile app**
  Guidance now favors username/password authentication with optional brokered SSO and clearly marks device code flow as legacy for backward compatibility only. ConnectionType and UseBroker are documented with defaults and valid values, and examples were updated to use UsernamePassword with UseBroker instead of DeviceCode. Additional notes explain phishing risks, default blocking in new tenants, lack of SSO, and iOS limitations, with advice to reconfigure devices accordingly.
  https://learn.microsoft.com/en-us/dynamics365/supply-chain/warehousing/install-configure-warehouse-management-app

- **Mass deploy the mobile app with user-based authentication**
  Device code flow is flagged as legacy and not recommended for MDM scenarios due to phishing risk and no SSO support. The article advises using username/password with a broker for SSO and clarifies that without SSO, each device requires manual sign-in.
  https://learn.microsoft.com/en-us/dynamics365/supply-chain/warehousing/warehouse-app-intune-user-based

- **Migrate the Warehouse Management mobile app from V3 to V4**
  The authentication methods table was reordered and clarified, adding a footnote that device code flow is still available but discouraged. The note explains phishing risks, default blocking in new tenants, lack of SSO/broker support, and recommends migrating to username/password.
  https://learn.microsoft.com/en-us/dynamics365/supply-chain/warehousing/warehouse-app-migrating-from-v3-v4

- **Use a QR code to connect the mobile app to Supply Chain Management**
  Recommendations now focus on UsernamePassword with UseBroker=true for SSO, and mark DeviceCode as not recommended. An IMPORTANT note highlights device code flow risks, default blocking in new tenants, and lack of iOS support, and all JSON examples were updated to use UsernamePassword with UseBroker.
  https://learn.microsoft.com/en-us/dynamics365/supply-chain/warehousing/warehouse-app-qr-code