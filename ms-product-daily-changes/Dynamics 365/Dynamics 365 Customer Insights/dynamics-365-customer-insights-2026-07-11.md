# Dynamics 365 Customer Insights
**Date created:** 2026-07-11 UTC  
**Tags:** Administration, Analytics, Governance, Other, Programming, Security  

## New Articles

- **Resolve Email Delivery Issues in Customer Insights - Journeys**

  Introduced a comprehensive troubleshooting guide to improve email deliverability, especially for internal recipients blocked by spam filters. Provides steps to add the service to SPF and allowlists across common security tools and major email platforms, and references public sending IPs. Explains why forwarded emails can break or render poorly, with design and process recommendations to mitigate. Clarifies that automatic responses ignore the Reply-To header per RFC 3834 and outlines how to prevent internal emails being incorrectly labeled as external through admin settings.

  https://learn.microsoft.com/en-us/troubleshoot/dynamics-365/customer-insights/journeys/email/email-troubleshoot-delivery

- **Troubleshoot email engagement drops in Customer Insights - Journeys**

  Added guidance to diagnose sudden declines in opens and clicks, including the impact of privacy protections and policy changes on tracking. Outlines a structured investigation: confirm authentication (SPF/DKIM/DMARC), use DMARC and reputation tools, review recent content or list changes, validate list hygiene, and run inbox placement tests. Provides direction on when to contact the deliverability team, what evidence to include, and notes 30-day log retention for timely analysis.

  https://learn.microsoft.com/en-us/troubleshoot/dynamics-365/customer-insights/journeys/email/email-troubleshoot-engagement

- **Troubleshoot Email Rendering in Customer Insights - Journeys**

  Published best practices and client-specific fixes for common rendering issues across major email clients. Covers dark mode behavior, large-message truncation in Gmail, and numerous Outlook (Classic) workarounds for layout, background images, spacing, line-height, and custom fonts. Details limitations of custom HTML, guidance for dynamic content and images, and handling quirks in Outlook mobile and regional providers. Includes techniques to prevent rendering breaks when emails are forwarded and links to related email authoring and previewing topics.

  https://learn.microsoft.com/en-us/troubleshoot/dynamics-365/customer-insights/journeys/email/email-troubleshoot-rendering

- **Fix Segment Member Count Issues in Customer Insights - Journeys**

  Introduced diagnostics for segments reporting too few or too many members. Provides steps to isolate problematic rules, verify set operations and business unit scoping, check data availability and consent filters, and align conditions with underlying data. Explains differences from Advanced Find results and highlights unsupported virtual fields. Includes guidance on when to open a support ticket and the information to provide.

  https://learn.microsoft.com/en-us/troubleshoot/dynamics-365/customer-insights/journeys/segments/segment-member-count

- **Troubleshoot Custom Channels in Customer Insights - Journeys**

  Added targeted guidance to resolve setup and message submission issues for custom channels and SMS providers. Explains required configuration entities, relationships, and naming conventions, and how to debug InternalChannelFailure errors using plugin trace logs. Recommends enriching “Not sent” statuses via plugin responses, handling retry/idempotency to avoid duplicates, and improving performance to prevent timeouts. Details how to enable delivery analytics by configuring the delivery report custom API and references sample solutions and best practices.

  https://learn.microsoft.com/en-us/troubleshoot/dynamics-365/customer-insights/journeys/channels/troubleshoot-custom-channels

- **Fix Domain Authentication in Customer Insights - Journeys**

  Published a step-by-step guide to resolve DKIM and domain ownership issues. Clarifies required DNS records, propagation timing, and how to construct and validate TXT and CNAME hostnames for subdomains and root domains. Provides instructions to verify the Envelope-from domain and confirm DNS status in the product, including using the Confirm action. Includes examples, screenshots, and links to best practices and BIMI setup.

  https://learn.microsoft.com/en-us/troubleshoot/dynamics-365/customer-insights/journeys/email/troubleshoot-domain-authentication

- **Troubleshoot Event Management in Customer Insights - Journeys**

  Introduced troubleshooting for session registrations, form errors, and waitlist behavior to ensure reliable event operations. Details causes of missing confirmation emails and how to trace their source, and explains check-in mechanics for Teams events, including required URL patterns and data substitutions. Highlights scenarios where check-ins are not recorded and provides references to optimize the check-in flow and diagnose Teams integration issues.

  https://learn.microsoft.com/en-us/troubleshoot/dynamics-365/customer-insights/journeys/event-management/troubleshoot-event-management

- **Troubleshoot Forms in Customer Insights - Journeys**

  Added guidance to fix embedded forms that fail to render by enabling external domain hosting and using default table-less layouts for better accessibility. Explains handling publication retries, defaulting hidden field values, and managing custom JavaScript placement across versions to avoid removal or misplacement. Covers resolving duplicate or failed submissions through matching strategy tuning, permissions for lookups, and using plug-in trace logs to identify and disable conflicting customizations.

  https://learn.microsoft.com/en-us/troubleshoot/dynamics-365/customer-insights/journeys/forms/troubleshooting-forms

- **Troubleshoot with Solution Health Hub in Customer Insights - Journeys**

  Published a walkthrough for using Solution Health Hub to proactively detect and fix environment issues. Lists included rules that check plug-in steps, disabled-owner processes, inactive workflows, missing configuration, and missing application user roles. Explains how to run analyses, interpret results and return statuses, use Resolve actions to remediate, and opt out of automatic rule execution. Provides prerequisites and related references to streamline governance and maintenance.

  https://learn.microsoft.com/en-us/troubleshoot/dynamics-365/customer-insights/journeys/general/troubleshoot-marketing-solution-health

- **Troubleshoot Push Notifications in Customer Insights - Journeys**

  Added end-to-end troubleshooting for push notification registration, delivery, and duplication across Android and iOS. Explains the asynchronous registration flow, common misconfigurations (tokens, app IDs, environment), and how to use IDs and logs to verify status. Details Android-specific issues with Firebase configuration, APIs, and handling data payloads, plus iOS-specific APNS token requirements and error interpretation. Includes guidance to avoid duplicate sends via journey design and idempotency.

  https://learn.microsoft.com/en-us/troubleshoot/dynamics-365/customer-insights/journeys/channels/troubleshoot-push-notifications

- **Troubleshoot Teams Event Integration in Customer Insights - Journeys**

  Introduced a guide to configure and troubleshoot Teams Webinar v2 and event integration. Covers required Graph permissions, admin consent, issuer formats for federated credentials, and setting Application Access Policies with correct scoping and precedence. Addresses registrations appearing in CRM but not in Teams, unpublished sessions, unexpected cancellation emails, and attendance data delays or gaps. Provides PowerShell commands and links to ensure reliable publishing and data synchronization.

  https://learn.microsoft.com/en-us/troubleshoot/dynamics-365/customer-insights/journeys/event-management/troubleshoot-teams-integration

## Moderate Changes

- **Schedule measures**

  Updated navigation to Insights > Measures, clarified how the Schedule column reflects current schedules, and refined descriptions of manual versus cadence-based refresh. Improved the caution note and confirmation step to emphasize that measures refresh on the scheduled date, reducing ambiguity for administrators.

  https://learn.microsoft.com/en-us/dynamics365/customer-insights/data/measures-schedule