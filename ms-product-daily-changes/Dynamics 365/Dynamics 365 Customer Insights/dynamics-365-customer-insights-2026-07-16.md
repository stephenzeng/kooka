# Dynamics 365 Customer Insights
**Date created:** 2026-07-16 UTC  
**Tags:** Analytics, Automation, Governance, Security  

## Moderate Changes

- **Add an action in a journey**

  Clarified a 90-day maximum wait duration for condition branches that depend on message interactions/triggers or segment membership. This helps prevent indefinite waits and ensures journey logic completes within predictable time windows.

  https://learn.microsoft.com/en-us/dynamics365/customer-insights/journeys/add-action

- **Create lead scoring models for Customer Insights - Journeys**

  Updated the article title and guidance to focus on lead scoring, with clearer instructions for using demographic attributes and interactions. Added an Important note that fields with field-level security (FLS) cannot be used in lead scoring model conditions, helping teams avoid configuration errors.

  https://learn.microsoft.com/en-us/dynamics365/customer-insights/journeys/real-time-marketing-create-lead-scoring-model

- **Prefill values for forms and event registration**

  Expanded guidance on consent prefill, detailing the two-stage calculation, consent enforcement models (Restrictive, Non-restrictive, Disabled), and how OR logic applies across linked channels. Clarified how the “When checked” setting (opt in vs. opt out), required Tracking consent, and a 15-minute cache affect send decisions, improving compliance and predictable behavior.

  https://learn.microsoft.com/en-us/dynamics365/customer-insights/journeys/real-time-marketing-form-prefill

- **Known issues in Customer Insights - Journeys with mitigations**

  Added a known issue noting that fields with field-level security (FLS) enabled can’t be used in lead scoring model conditions. This helps users quickly identify and avoid unsupported configurations.

  https://learn.microsoft.com/en-us/dynamics365/customer-insights/journeys/real-time-marketing-known-issues

- **Security roles for lead scoring and qualification in Dynamics 365 Customer Insights - Journeys**

  Added an Important note clarifying that fields with field-level security (FLS) cannot be used in lead scoring model conditions, regardless of a user’s security role. This prevents misconfiguration and sets clear expectations for model design.

  https://learn.microsoft.com/en-us/dynamics365/customer-insights/journeys/real-time-marketing-security-roles-lead-scoring