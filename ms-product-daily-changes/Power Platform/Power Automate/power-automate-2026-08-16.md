# Power Automate
**Date created:** 2026-08-16 UTC  
**Tags:** Compliance, Configuration, Guidance, Licensing  

## New Articles

- **Assign a user license to a flow owned by a service principal**

  Introduced a step-by-step how-to for keeping service principal–owned cloud flows compliant by designating a licensed user instead of assigning a Process (capacity) license. Explains prerequisites and how licensing works, with UI guidance to set the Licensee and remediation steps for suspended flows. Provides programmatic options using the Microsoft Dataverse connector and Web API, including PATCH/GET/DELETE examples and relevant table and column details. Notes that the designation is environment-specific and must be reapplied after redeployments.

  https://learn.microsoft.com/en-us/power-automate/assign-user-license-service-principal-flow

## Moderate Changes

- **Support for service principal owned flows**

  Expanded licensing guidance by enumerating valid options for service principal–owned flows and clarified that sharing connections isn’t required for solution flows. Improved instructions for changing the owner and emphasized usage guidance and ownership limits, including no co-owner capability.

  https://learn.microsoft.com/en-us/power-automate/service-principal-support