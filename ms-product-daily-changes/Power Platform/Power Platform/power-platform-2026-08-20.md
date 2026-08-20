# Power Platform
**Date created:** 2026-08-20 UTC  
**Tags:** Configuration, Licensing, Security  

## Moderate Changes

- **Power Platform URLs and IP address ranges**

  Clarified network allow-list guidance to avoid using resolved environment IPs and instead rely on the published Azure service tag IP ranges, refreshed regularly. Updated the Ports section to state that Dataverse TDS connectivity requires ports 1433 and 5558 to be allowed along with the applicable IP ranges, improving setup reliability and compliance.

  https://learn.microsoft.com/en-us/power-platform/admin/online-requirements

- **Power Platform licensing FAQs**

  Refined wording in AI Builder licensing and capacity sections and standardized the capitalization of “Copilot Credits.” Removed prescriptive guidance about consumption precedence (AI Builder credits first, then Copilot credits) and the rule that Copilot Studio agents always consume Copilot credits, reducing potential confusion and aligning with current licensing descriptions.

  https://learn.microsoft.com/en-us/power-platform/admin/powerapps-flow-licensing-faq