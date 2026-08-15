# Dynamics 365 Customer Insights
**Date created:** 2026-08-15 UTC  
**Tags:** Configuration, Governance, Guidance, Security, Troubleshooting  

## New Articles

- **How record ownership and business units affect personalization**

  Introduced guidance on how Dataverse record ownership and business units determine what data is available to personalization in Customer Insights - Journeys. Clarifies identity differences between preview (signed-in user) and live execution (service user with Service Reader) and how each uses platform security vs. business unit scoping. Explains exact-match scoping for owner or owning business unit across user-, team-, business unit–, and organization-owned records, and how multi-hop personalization can fail when any record falls outside scope. Provides diagnostic steps to trace ownership along placeholder paths and mitigation approaches such as aligning record and journey ownership, adjusting scoping, and setting defaults—helping teams resolve missing or unexpected personalization outcomes.

  https://learn.microsoft.com/en-us/dynamics365/customer-insights/journeys/personalization-ownership-business-units