# Microsoft Purview
**Date created:** 2026-07-21 UTC  
**Tags:** Governance  

## New Articles

- **Disaster Recovery for Microsoft Purview Data Map**

  Introduces a comprehensive manual BCDR guide for Microsoft Purview Data Map, covering prerequisites such as an Enterprise primary account, enabling Classic provisioning in a secondary region, and capturing identities and Key Vault details. Provides step-by-step setup to mirror the primary environment, including collection RBAC, integration runtimes (managed VNet, Azure IR, SHIR), managed private endpoints, and private endpoints/DNS. Clarifies configuration of data source access for the secondary identity, registration of Key Vault connections, and alignment of firewall and network rules. Details replication of scan configurations (data sources, credentials, classification rules, rulesets, scans, schedules) and validation of parity between accounts. Outlines the failover process via support ticket and offers troubleshooting for common authentication, network, credential, configuration drift, and provisioning issues.

  https://learn.microsoft.com/en-us/purview/data-map-disaster-recovery