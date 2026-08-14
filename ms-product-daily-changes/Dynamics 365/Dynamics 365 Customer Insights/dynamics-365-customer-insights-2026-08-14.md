# Dynamics 365 Customer Insights
**Date created:** 2026-08-14 UTC  
**Tags:** Compliance, Guidance  

## Moderate Changes

- **Consent management overview**

  Updated guidance to focus on configuring consent controls in Customer Insights – Journeys, emphasizing that organizations define requirements, profiles, and enforcement models. Clarified how purposes and contact point consent are configured, noted product default purposes should be reviewed, and defined purpose as a customer-set label mapped to a legal basis. Added a warning that the Disabled enforcement model bypasses consent checks and tracking controls, which may lead to unintended data processing.

  https://learn.microsoft.com/en-us/dynamics365/customer-insights/journeys/real-time-marketing-compliance-settings

- **Manage consent for email, SMS (text), and custom channel messages**

  Expanded send-time consent evaluation to show how purposes, optional topics, consent records, and enforcement models determine delivery. Clarified default enforcement models and reworked tracking consent to a single built-in Tracking purpose covering opens, clicks, UTM, website interactions, and form prefill, advising review or disablement as needed. Added a warning that the Disabled model skips consent evaluation, which can result in sending and tracking even for opted-out contact points.

  https://learn.microsoft.com/en-us/dynamics365/customer-insights/journeys/real-time-marketing-email-text-consent