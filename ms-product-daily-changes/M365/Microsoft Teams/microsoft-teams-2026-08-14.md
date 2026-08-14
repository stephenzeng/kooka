# Microsoft Teams
**Date created:** 2026-08-14 UTC  
**Tags:** Analytics, Automation, Compliance, Configuration, Deprecation, Get Started, Guidance, Identity, Security, Troubleshooting  

## New Articles

- **Introduction to Microsoft 365 Plugins**

  Introduced new documentation for using Microsoft 365 plugins to integrate Moodle with Teams, covering SSO, user sync, permissions, and SharePoint configuration. Explains how to use OneDrive/SharePoint as repositories, create Teams meetings from Moodle, and apply a Teams-themed UI. Details OneNote integration, the Microsoft block for quick access to Microsoft 365 apps, and the oEmbed filter for rich content. Includes plugin references with GitHub labels, examples, and related links.

  https://learn.microsoft.com/en-us/microsoftteams/m365-plugins-overview

- **Moodle frequently asked questions**

  Added a comprehensive FAQ for Moodle–Teams integration. Covers prerequisites for course team creation, enforcing Microsoft 365 SSO, and controlling which users sync. Provides troubleshooting for sync and sign-in issues, renewing expired app secrets, changing the Teams instance linked to a course, restoring the Atto Teams meeting icon, and understanding calendar behavior. Includes pointers to support and feedback resources.

  https://learn.microsoft.com/en-us/microsoftteams/moodle-faqs

- **Introduction to Moodle LMS**

  Published an overview of Moodle LMS integration scenarios in Teams, including calls, chat, courses, and badges. Highlights access via Microsoft 365 plugins and partner apps, plus scenarios like hybrid meetings, personalized panels via Graph API, and automated institution setup using Adaptive Cards and custom connectors. Describes partner solutions (including mConnect), availability, and admin requirements, with links to setup and SSO guidance.

  https://learn.microsoft.com/en-us/microsoftteams/moodle-overview

## Major Changes

- **Setup - Teams Phone Agent**

  Expanded setup guidance with three new capabilities: spam detection, AI disclaimer customization, and configurable call length. Admins can define spam handling (including allow/deny lists), tailor AI disclaimers via PowerShell, and set custom call timeouts and disconnect prompts. The updates streamline policy control and improve compliance and call experience. The What's new section reflects these additions.

  https://learn.microsoft.com/en-us/microsoftteams/aa-cq-setup-teams-phone-agent

- **Languages for voicemail greetings and messages in Microsoft Teams**

  Updated voicemail transcription guidance to reference Azure Speech Fast Transcription and the need to enable transcription via Voicemail policies. The languages table was extensively refreshed, moving many languages to supported status and noting fallback dialects where applicable. This broadens coverage and sets expectations that supported languages evolve with Azure Speech.

  https://learn.microsoft.com/en-us/microsoftteams/languages-for-voicemail-greetings-and-messages

- **Plan Operator Connect for India**

  Added an IMPORTANT section on Location-Based Routing for India wireline numbers requiring automatically detected OS location. If Windows uses a manual default location, Teams removes coordinates and disables PSTN calling, which can hide the dial pad. The guidance lists common causes (VPN/proxies, VMs, disabled location services/permissions) and recommends admin actions to restore compliant detection. This behavior aligns with India regulations to prevent spoofing.

  https://learn.microsoft.com/en-us/microsoftteams/operator-connect-india-plan

- **Plan for Operator Connect**

  Significantly restructured planning guidance with an onboarding flow, clearer benefits, and explicit requirements for licensing, regions, and networking. Added quick links to related configuration and number management resources. Clarified support boundaries between Microsoft and operators to direct PSTN issues appropriately. The result is a more actionable planning and deployment guide.

  https://learn.microsoft.com/en-us/microsoftteams/operator-connect-plan

- **Certified Teams displays**

  Replaced detailed certification and firmware content with a deprecation notice for the Teams displays device category. Announced end of support for the Teams displays app on September 3, 2025. Guidance now directs customers to bookable desk solutions using Teams desktop with certified peripherals and analytics via Teams Rooms Pro Management and Microsoft Places.

  https://learn.microsoft.com/en-us/microsoftteams/devices/teams-displays-certified-hardware

## Moderate Changes

- **Setup - Spam Detection template for Teams Phone Agent**

  Removed the preview PowerShell module prerequisite and consolidated scattered examples into a shared include. This simplifies setup and keeps command guidance consistent in one place.

  https://learn.microsoft.com/en-us/microsoftteams/aa-cq-setup-teams-phone-agent-template-spam-detection

- **Transition to Password-less Teams Shared Space device Resource Accounts**

  Expanded benefits to emphasize removing or scrambling passwords while maintaining Microsoft 365 access, and raised the required Teams Admin Agent version across Android-based devices. Clarified migration requirements (Teams Administrator role for portal sign-in) and updated password cleanup guidance to align with password-less practices.

  https://learn.microsoft.com/en-us/microsoftteams/rooms/passwordlessentraresourceaccounts

- **Teams Bot Identification Program**

  Clarified program terminology and added a process overview. Expanded Next steps to cover intake, NDA and agreement requirements, detailed registration steps and validation scope, and the outcome of bots appearing as registered in Teams meetings.

  https://learn.microsoft.com/en-us/microsoftteams/teams-bot-identification

- **Microsoft Teams analytics and reporting**

  Added two security-focused reports to the reference: User reported security submissions (for calls, chats/channels, and external users) and Security detections. Each entry lists key fields to help admins investigate reported content and detections efficiently.

  https://learn.microsoft.com/en-us/microsoftteams/teams-analytics-and-reports/teams-reporting-reference

- **Personal peripherals certified for Microsoft Teams**

  Added newly certified devices: Jabra Evolve3 65 Stereo/Mono, Evolve3 45 Stereo/Mono, Evolve3 65 Flex (USB), and Yealink BH78 (native Bluetooth), with 2026 qualification dates. This expands approved options for reliable audio peripherals.

  https://learn.microsoft.com/en-us/microsoftteams/devices/usb-devices

- **How to use Microsoft Teams panels**

  Updated ad hoc meeting rules: start time can be current or in the future, and meetings now end by midnight or the next scheduled meeting (not up to 24 hours). Extension rules now allow 15-minute increments up to the next meeting start or midnight.

  https://learn.microsoft.com/en-us/microsoftteams/devices/use-teams-panels