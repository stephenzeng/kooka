# Power Query
**Date created:** 2026-07-21 UTC  
**Tags:** Security  

## Moderate Changes

- **Handling Connector Signing**

  Added guidance for installing and running MakePQX via the Microsoft.PowerQuery.SdkTools NuGet package, including NuGet CLI steps and the requirement to execute from the tools directory to avoid path issues. Updated command help and refined descriptions for Pack, Sign, and Verify, with revised examples to improve accuracy and usability. Introduced notes on using Export-PfxCertificate and clarified how to trust signed connectors in Power BI Desktop to strengthen the signing workflow and reduce setup errors.

  https://learn.microsoft.com/en-us/power-query/handling-connector-signing