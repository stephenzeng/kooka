# Microsoft Intune
**Date created:** 2026-07-30 UTC  
**Tags:** Administration, Security  

## New Articles

- **Supported configurations for SQL Server**

  Introduced a dedicated article that consolidates required and optional SQL Server settings for Configuration Manager, making setup expectations clear and easier to follow. It specifies mandatory instance and database configurations, recommended memory reservations, and clarifies when to use Windows authentication. It adds optional guidance for SQL service accounts and SPN management, plus new security options available from version 2603, including extended protection and enforced SQL encryption. It also documents required ports and the need for static ports on named instances to simplify firewall planning and intersite communications.

  https://learn.microsoft.com/en-us/intune/configmgr/core/plan-design/configs/supported-configurations-for-sql-server

## Major Changes

- **Supported SQL Server versions**

  Restructured the page to focus on version and edition support while moving detailed configuration requirements to a new, dedicated article. Added guidance on using Database Engine only, supported instance patterns, 64-bit architecture requirements, and considerations for the data warehouse service point. Updated compatibility to note SQL Server 2025 support starting with version 2603, and streamlined optional topics while retaining SSRS prerequisites. This improves clarity, separates “what is supported” from “how to configure,” and reduces duplication.

  https://learn.microsoft.com/en-us/intune/configmgr/core/plan-design/configs/support-for-sql-server-versions

## Moderate Changes

- **Supported configurations for Configuration Manager**

  Expanded SQL Server guidance by refining the “Supported SQL Server versions” entry and adding a new “Supported configurations for SQL Server” reference. This improves discoverability of version support and directs admins to a single source for required and optional SQL settings.

  https://learn.microsoft.com/en-us/intune/configmgr/core/plan-design/configs/supported-configurations