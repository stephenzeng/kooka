# Microsoft Purview
**Date created:** 2026-07-30 UTC  
**Tags:** AI, Security  

## Moderate Changes

- **Collection policy reference**

  Added a consolidated “Considerations for unmanaged cloud apps policies” section to improve configuration and troubleshooting. Clarified that detection is based on destination app traffic, advised including all catalog entries for apps with multiple names, and noted some AI apps send encoded content to dynamic endpoints affecting enforcement. Added a note that unmanaged cloud app features apply only to the consumer version of Microsoft 365 Copilot, with links to enterprise protections.

  https://learn.microsoft.com/en-us/purview/collection-policies-policy-reference

- **Learn about Data Loss Prevention for Cloud Apps in Edge for Business**

  Added a limitation that browser and network data security policies don’t apply to B2B guest users. Expanded guidance for unmanaged cloud apps, including consumer versions of Microsoft 365 Copilot and ChatGPT, and introduced a consolidated considerations section covering catalog entry inclusion, destination-based detection, shared URLs across consumer/enterprise instances, and handling encoded traffic.

  https://learn.microsoft.com/en-us/purview/dlp-browser-dlp-learn

- **Help prevent sharing via Microsoft Edge for Business to unmanaged AI apps from managed devices**

  Removed an outdated note about Intune multi-admin approval not being supported for inline protection, reducing confusion. Updated prerequisites to reference the new considerations for unmanaged cloud apps policies for more accurate setup guidance.

  https://learn.microsoft.com/en-us/purview/dlp-create-policy-block-to-ai-via-edge

- **Learn about Microsoft Purview Network Data Security**

  Introduced a “Considerations for unmanaged cloud apps policies” subsection to streamline deployment and troubleshooting. Guidance clarifies including all relevant catalog entries, destination-based detection behavior, potential enforcement limits with encoded traffic, and how shared URLs can capture both consumer and enterprise interactions. Added a note that unmanaged cloud app features apply only to the consumer version of Microsoft 365 Copilot with a link to enterprise protections.

  https://learn.microsoft.com/en-us/purview/dlp-network-data-security-learn