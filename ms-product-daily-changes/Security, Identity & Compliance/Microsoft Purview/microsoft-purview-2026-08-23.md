# Microsoft Purview
**Date created:** 2026-08-23 UTC  
**Tags:** Configuration, Guidance, Identity, Security, Troubleshooting  

## Moderate Changes

- **Assign permissions in eDiscovery**

  Updated guidance to add step-by-step instructions for configuring app-only (certificate-based) authentication for eDiscovery PowerShell, including creating a Microsoft Entra app, granting Exchange.ManageAsApp permissions with admin consent, registering the service principal, and assigning it to the eDiscovery Manager role group. The article also details how to connect using Connect-IPPSSession with EnableSearchOnlySession and ExchangeOnlineManagement 3.10.1+, and includes troubleshooting for common issues like HTTP 401 and missing eDiscovery cmdlets. These changes help teams securely automate eDiscovery tasks with least-privileged, service principal-based access.

  https://learn.microsoft.com/en-us/purview/edisc-permissions