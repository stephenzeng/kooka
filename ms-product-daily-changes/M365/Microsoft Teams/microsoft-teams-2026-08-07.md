# Microsoft Teams
**Date created:** 2026-08-07 UTC  
**Tags:** Administration, Governance, Monitoring, Security  

## Major Changes

- **Transition to Password-less Teams Shared Space device Resource Accounts**
  Restructured the guide into clear steps with new security guidance, including a required post-migration password rotation for resource accounts. Added important limitations and support notes, such as lack of proxy support for Teams Rooms on Windows and the need to set up replacement devices with a password before migrating. Consolidated troubleshooting and known issues, with mitigations for proxy-related Pro Management problems and network delays (for example, STP/portfast) that can block automatic sign-in. Expanded guidance to revert to password authentication when needed, and added an extensive FAQ covering migration triggers, device eligibility, post-migration behavior, and recovery scenarios.
  https://learn.microsoft.com/en-us/microsoftteams/rooms/passwordlessentraresourceaccounts

- **PSTN connectivity options**
  Overhauled guidance to focus on Teams Phone scenarios, how to mix connectivity options in a tenant, and how to choose the right approach. Introduced a concise comparison chart and feature table, clarified supported phone number types across options, and added guidance on combining operators and regional flexibility. Added foundational explanations of the PSTN, licensing prerequisites, provider responsibilities, and secure tenant integration. Included a “What’s next?” section with actionable steps to license, select, and configure the solution.
  https://learn.microsoft.com/en-us/microsoftteams/pstn-connectivity

- **Set up and manage live chat**
  Announced Live chat retirement: new customer setup ends August 6, 2026, and service ends October 5, 2026. Added a comprehensive FAQ covering end-of-support behavior, data retention expectations, required admin actions (remove the website widget by deleting the chatbot script), and recommended alternatives (Dynamics 365 Contact Center Live Chat and Microsoft Copilot Studio Contact Center AI solutions). Included a support contact for transition assistance.
  https://learn.microsoft.com/en-us/microsoftteams/set-up-live-chat

## Moderate Changes

- **Country and region availability for Audio Conferencing and Calling Plans**
  Clarified that availability listings do not indicate Know Your Customer (KYC) requirements and directed admins to verify KYC for the target country or region. Noted that KYC is reviewed at the tenant level, typically within three business days, and should be completed early to avoid number acquisition or porting delays.
  https://learn.microsoft.com/en-us/microsoftteams/calling-plan-overview

- **Microsoft Teams Calling Plans**
  Rewrote the introduction and added a comparison table for Domestic, International, and Pay-As-You-Go plans to help customers select the right option. Added an overview diagram explaining PSTN connectivity and a KYC note advising completion of approval before acquiring or porting numbers. Streamlined references to PSTN connectivity for clarity.
  https://learn.microsoft.com/en-us/microsoftteams/calling-plans-for-office-365

- **Set up Microsoft Teams in your small or medium business**
  Added an important notice about Live chat retirement, including key dates and service impact. Advised admins to remove the live chat widget before October 5, 2026 and linked to the retirement FAQ for migration guidance.
  https://learn.microsoft.com/en-us/microsoftteams/deploy-small-business

- **Teams Rooms Pro Management Portal Incident Notification Webhook Integration**
  Updated device types in the Event Subscription table: standardized “Teams Rooms on Android,” added IP Phone, SIP, and SIP Analog, and removed Surface Hub (legacy). Simplified instructions for selecting device types.
  https://learn.microsoft.com/en-us/microsoftteams/rooms/pmp-incident-webhook-integration

- **Set up Microsoft Calling Plans**
  Emphasized verification of availability, KYC requirements, and licensing, and added a dedicated KYC step with who submits, acceptable domains, admin center path, submission steps, status tracking, and review timelines. Renumbered the remaining setup steps for clarity.
  https://learn.microsoft.com/en-us/microsoftteams/set-up-calling-plans

- **Certified Teams phones**
  Added the C456HD device entry for GCCH, including latest firmware (3.1.98 AOSP), app versions (Teams, Intune, Authenticator, Admin Agent), and an August 4, 2026 release date. Helps admins validate compatibility and target firmware/app baselines.
  https://learn.microsoft.com/en-us/microsoftteams/devices/teams-phones-certified-hardware