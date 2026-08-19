# Power Query
**Date created:** 2026-08-19 UTC  
**Tags:** Configuration, Identity  

## Moderate Changes

- **Denodo**

  Marked Microsoft Entra ID SSO as generally available and updated guidance to remove preview references. Viewers of DirectQuery semantic models now use their own Entra ID identity to query Denodo, reducing reliance on on-premises Active Directory and Kerberos constrained delegation. This simplifies deployment and supports cloud-first authentication.

  https://learn.microsoft.com/en-us/power-query/connectors/denodo

- **Starburst**

  Moved Microsoft Entra ID authentication and DirectQuery SSO to general availability for the “Starburst secured by Entra ID” connector, removing preview labels across capabilities, authentication types, and descriptions. Viewers now authenticate with their own Entra ID identity, streamlining SSO and reducing configuration ambiguity.

  https://learn.microsoft.com/en-us/power-query/connectors/starburst