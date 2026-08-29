# SharePoint
**Date created:** 2026-08-29 UTC  
**Tags:** Deprecation, Governance, Guidance, Security  

## New Articles

- **Deprecation of Classic SharePoint Pages**

  Announced a phased deprecation of classic SharePoint publishing sites and user-created classic pages, alongside strengthened custom scripting restrictions. Phase 1 (Mar 1, 2027) blocks creation and activation of classic publishing features, enforces tenant settings to prevent classic publishing site creation, and for new tenants disables creating/editing classic pages with DenyAddAndCustomizePages=True. Phase 2 (Oct 1, 2028) extends these restrictions to all tenants, makes classic user-created pages read-only, and applies custom script limitations across environments including GCC, GCC High, DoD, air-gapped, and 21Vianet. Provides migration guidance to discover and assess usage (Purview Audit, Microsoft 365 Assessment Tool), modernize with recommended tools (PnP PowerShell, optional Page Migration Agent), and run wave-based migrations; classic list and library views/forms remain unaffected.

  https://learn.microsoft.com/en-us/sharepoint/classic-user-created-page-deprecation