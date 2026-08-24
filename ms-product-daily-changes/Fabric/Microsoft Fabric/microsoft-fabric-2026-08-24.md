# Microsoft Fabric
**Date created:** 2026-08-24 UTC  
**Tags:** Analytics, Best Practices, Governance, Guidance, Security  

## New Articles

- **Microsoft OneLake patterns and foundational capabilities**

  Introduced a comprehensive concept article that defines core OneLake architectural patterns and how foundational capabilities bring them to life. Explains when and how to use patterns such as unified data access, medallion layers, domain-oriented data mesh, platform consolidation for analytics/AI, and external data sharing. Details enabling features including shortcuts, database and metadata mirroring, OneLake security and catalog, open table formats, Direct Lake, and interoperability with Fabric workloads and partner engines. Provides step-by-step guidance, decision points, and governance considerations to help teams build a unified, governed analytics foundation.

  https://learn.microsoft.com/en-us/fabric/onelake/architecture-patterns

## Moderate Changes

- **Understand medallion architecture for Fabric with OneLake**

  Added planning guidance for implementing the medallion pattern, covering layer design, deployment approaches, storage formats, materialized lake views, and Delta optimization. Cross-references the new OneLake patterns article for broader context, and slightly refined the title for clarity.

  https://learn.microsoft.com/en-us/fabric/onelake/onelake-medallion-lakehouse-architecture

- **What is OneLake?**

  Updated the Mirroring section to clarify zero-ETL options and distinguish database mirroring (replicates into Delta tables) from metadata mirroring (accesses data in place via shortcuts). Added guidance on when to use shortcuts versus mirroring and refreshed related resources, replacing older items with more current guidance and an improved quickstart.

  https://learn.microsoft.com/en-us/fabric/onelake/onelake-overview