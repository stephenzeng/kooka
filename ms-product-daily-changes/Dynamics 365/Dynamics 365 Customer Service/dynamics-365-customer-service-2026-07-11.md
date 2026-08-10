# Dynamics 365 Customer Service
**Date created:** 2026-07-11 UTC  
**Tags:** Agent, Administration  

## Moderate Changes

- **Configure automated messages**
  
  Added guidance for Messaging API channel instances to send queue wait time notifications using the Estimate Wait Time Notification trigger. You can include the {QueuePosition} variable, set the notification interval, and optionally repeat notifications until an agent is assigned. This helps set clear expectations for customers while they wait.
  
  https://learn.microsoft.com/en-us/dynamics365/customer-service/administer/configure-automated-message

- **Overview of productivity pane Dynamics 365 Copilot Service workspace**
  
  Clarified that screen recording captures the entire screen and shows a red border during recording. Added instructions for multi-monitor setups to select which monitors to capture when the multi-screen setting is enabled; otherwise, all monitors are recorded. This helps agents control what is recorded and align with privacy requirements.
  
  https://learn.microsoft.com/en-us/dynamics365/customer-service/use/csw-productivity-pane

- **Configure call recording, transcription, and real-time translation**
  
  Introduced a prerequisite to enable audio recording at the tenant level in the Copilot Service admin center; if disabled, audio recording is blocked regardless of workstream configuration. The requirement to allow audio and mpeg MIME types in the Power Platform admin center remains. This ensures administrators configure recording capabilities consistently and avoid unexpected recording failures.
  
  https://learn.microsoft.com/en-us/dynamics365/customer-service/administer/voice-channel-configure-transcripts