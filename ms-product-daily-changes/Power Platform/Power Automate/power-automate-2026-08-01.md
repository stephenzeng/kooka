# Power Automate
**Date created:** 2026-08-01 UTC  
**Tags:** Administration, Automation, Security  

## Moderate Changes

- **Secure data used in cloud flows**

  Updated security guidance by removing the recommendation to use IP pinning for HTTP request triggers and emphasizing Microsoft Entra ID token authentication as the primary control. This clarifies best practices and reduces reliance on brittle IP allowlists, improving overall security posture. Minor wording and formatting clean-up were also made.

  https://learn.microsoft.com/en-us/power-automate/guidance/coding-guidelines/use-secure-inputs-outputs-triggers

- **Troubleshoot Browser Extension Errors in Desktop Flows**

  Reworked the article to clarify which errors are covered and retitled it to improve discoverability for desktop flow web automation. Added a new troubleshooting step for failures caused by coexisting MSI and MSIX installations of Power Automate for desktop, with a link to detailed guidance.

  https://learn.microsoft.com/en-us/troubleshoot/power-platform/power-automate/desktop-flows/browser-automation/web-extensions-policies