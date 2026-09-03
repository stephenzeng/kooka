# Dynamics 365 Customer Service
**Date created:** 2026-09-03 UTC  
**Tags:** Guidance, Performance, Troubleshooting  

## Major Changes

- **FAQ on managing cases**

  Expanded troubleshooting guidance for case creation and form issues to help admins resolve errors faster and improve reliability. Added steps to diagnose “Expected non-empty Guid” errors by validating lookup GUIDs, integrations, and @odata.bind references. Introduced performance recommendations for slow Web API case creation, including handling service protection limits, moving synchronous operations to async, and adding retry logic. Added a new case forms FAQ to address missing fields, hidden command buttons, HTTP 500 errors on save, missing referenced components, and slow form loads, with actionable checks and optimization tips.

  https://learn.microsoft.com/en-us/dynamics365/customer-service/administer/faq-case-mgmt

- **Supported languages and locale codes for voice channel**

  Streamlined the language support table to focus on Voice channel, IVR, Sentiment, and UI coverage, making it easier to identify supported locales. Updated and reduced the locale list with revised Yes/No availability to set accurate expectations for deployments. Clarified that transcription uses speech-to-text only for languages supported by the voice channel, improving planning for multilingual scenarios.

  https://learn.microsoft.com/en-us/dynamics365/customer-service/administer/voice-channel-supported-languages