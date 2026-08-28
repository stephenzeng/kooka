# Dynamics 365 Commerce
**Date created:** 2026-08-28 UTC  
**Tags:** Configuration, Guidance  

## Moderate Changes

- **Enable pay by link in POS by using the Dynamics 365 Payment Connector for Adyen**

  Updated configuration guidance for passing Adyen store information per register or per store by embedding the Adyen store name within #...# in the register or store name, with register-level values taking precedence over store-level. Clarified availability: capability is backported to Commerce 10.0.46 (behind a flight) and enabled by default starting with 10.0.47.

  https://learn.microsoft.com/en-us/dynamics365/commerce/dev-itpro/pay-by-link-overview