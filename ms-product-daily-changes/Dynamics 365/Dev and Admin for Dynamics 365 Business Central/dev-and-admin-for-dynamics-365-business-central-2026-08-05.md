# Dev and Admin for Dynamics 365 Business Central
**Date created:** 2026-08-05 UTC  
**Tags:** Administration, Programming  

## Moderate Changes

- **Feature details for Business Central 2026 release wave 1 public preview**
  Updated terminology and guidance to use Marketplace instead of AppSource, clarifying how Quality Management features are installed and discovered, how custom cloud migration engines are packaged and reused, and how AI billing and monetization flow through Marketplace. These edits align documentation with current distribution and monetization paths without adding new sections.

  https://learn.microsoft.com/en-us/dynamics365/business-central/dev-itpro/whatsnew/preview-feature-details

- **Record.FindSet([Boolean]) Method**
  Clarified that FindSet(true) reads records using IsolationLevel::UpdLock (SQL UPDLOCK) rather than performing LockTable(), aligning guidance with actual update semantics. This helps developers apply the correct locking behavior when iterating and updating records.

  https://learn.microsoft.com/en-us/dynamics365/business-central/dev-itpro/developer/methods-auto/record/record-findset-boolean-method