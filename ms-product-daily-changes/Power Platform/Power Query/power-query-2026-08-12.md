# Power Query
**Date created:** 2026-08-12 UTC  
**Tags:** Configuration, Deprecation, Guidance, Performance, Troubleshooting  

## Major Changes

- **Power Query Oracle database connector**

  Added a comprehensive Known issues section for the built-in Oracle driver, including TNS alias resolution failures on network shares, ignored NLS_LANG leading to parsing errors, and FetchSize registry overrides not being honored—along with actionable workarounds such as moving tnsnames.ora locally, aligning regional settings, using Easy Connect, or disabling the built-in driver to revert to the unmanaged driver. Clarified that Oracle proxy-user authentication isn’t supported on the on-premises data gateway (June 2026+), with guidance to disable the built-in driver for Import, contact Microsoft Support for DirectQuery, or use non-proxy accounts; also noted how to update Oracle credentials in the Power BI service via semantic model settings. Updated guidance to reflect Power BI Desktop terminology, removed outdated gateway configuration steps, and clarified that the updated Oracle connector doesn’t support personal on-premises data gateways for Import or DirectQuery—recommending enterprise or VNET gateways or direct cloud connections. These changes streamline setup, reduce connectivity and locale-related errors, and direct users toward supported gateway configurations.

  https://learn.microsoft.com/en-us/power-query/connectors/oracle-database