# Dynamics 365 Commerce
**Date created:** 2026-08-12 UTC  
**Tags:** Configuration, Deprecation, Guidance, Performance  

## Major Changes

- **Archive, delete, or compress credit card transaction data**

  Expanded guidance now covers archiving, deleting, and compressing credit card transaction data to improve performance and governance. From version 10.0.49, compression runs in a dedicated batch job (Compress credit card transaction data), and the Archive job now focuses on archiving or deletion, with the Use compression parameter deprecated. The article clarifies parameters such as Delete data without archiving, details in-scope entities (PaymentAuthorization, PaymentCaptureToken, PaymentCardToken, SigCapData), and adds instructions for compressing existing tokens via the Compress credit card transaction tokens feature (dependent on Compress payment tokens). It also consolidates document management dependencies, refines guidance on batch scheduling and PII handling, and removes outdated preview content.

  https://learn.microsoft.com/en-us/dynamics365/commerce/dev-itpro/archive-cc-data