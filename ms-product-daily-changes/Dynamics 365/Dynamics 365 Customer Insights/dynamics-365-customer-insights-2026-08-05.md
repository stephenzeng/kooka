# Dynamics 365 Customer Insights
**Date created:** 2026-08-05 UTC  
**Tags:** Governance, Programming  

## Moderate Changes

- **Consent management overview**

  Clarified how compliance profiles and purposes work, emphasizing that each profile has a single tracking purpose and that tracking purposes can’t be linked or unlinked after creation. Explained the impact of the “Use previously captured consent” option, including inherited purposes and default purpose creation when not used. Highlighted that enforcement is configured on the purpose and applies across all profiles sharing it, advising separate purposes (and avoiding the toggle for tracking) when different enforcement is required.

  https://learn.microsoft.com/en-us/dynamics365/customer-insights/journeys/real-time-marketing-compliance-settings

- **Manage consent for email, SMS (text), and custom channel messages**

  Expanded guidance on what tracking consent governs, including opens, link clicks, UTM parameters, website interactions via the tracking script, and form prefill. Clarified that website tracking relies on cookie acceptance and that tracking consent controls interaction recording, not cookie placement. Noted that the tracking purpose must be explicitly added to forms and preference centers because it isn’t included by default.

  https://learn.microsoft.com/en-us/dynamics365/customer-insights/journeys/real-time-marketing-email-text-consent

- **Extend Customer Insights - Journeys marketing forms using code**

  Updated examples to use a parameterized FormLoader URL pattern, ensuring scripts are loaded from the correct environment. Added instructions to obtain server and geo values from the published embed code to prevent misconfiguration across regions and environments.

  https://learn.microsoft.com/en-us/dynamics365/customer-insights/journeys/developer/realtime-marketing-form-client-side-extensibility

- **Create branded, customized preference centers to manage customer consent**

  Clarified that the default preference center includes only the Commercial purpose and excludes Tracking. Advised explicitly adding Tracking to enable users to manage tracking consent, especially when using a restrictive enforcement model.

  https://learn.microsoft.com/en-us/dynamics365/customer-insights/journeys/real-time-marketing-preference-centers