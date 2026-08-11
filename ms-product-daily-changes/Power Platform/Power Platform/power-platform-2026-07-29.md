# Power Platform
**Date created:** 2026-07-29 UTC  
**Tags:** Administration, Analytics, Governance, Programming  

## Major Changes

- **pac model**

  Expanded the PAC CLI reference for model-driven app generated pages with new commands to discover connector tables and operations and retrieve schemas. Documented parameters for these commands to improve automation and repeatability across environments. Added a new --connectors option to pac model genpage upload to persist connector bindings in config.json, helping teams keep generated pages consistently wired to required connectors.

  https://learn.microsoft.com/en-us/power-platform/developer/cli/reference/model

## Moderate Changes

- **Dataverse capacity-based storage details**

  Added a preview Dataverse storage advisor in the Licensing > Dataverse capacity view that highlights cleanup opportunities with a recommendation banner, a Clean up column, and a detailed advisor panel. The guidance helps admins reclaim space by setting archival policies, running bulk deletes, and managing capacity based on table-level insights.

  https://learn.microsoft.com/en-us/power-platform/admin/capacity-storage