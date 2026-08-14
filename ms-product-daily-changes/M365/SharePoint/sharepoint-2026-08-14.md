# SharePoint
**Date created:** 2026-08-14 UTC  
**Tags:** Best Practices, Configuration, Governance, Guidance  

## Major Changes

- **Generate structured documents in a SharePoint document library**

  Added support for Managed metadata fields, enabling selection from governed term sets in structured document generation. Expanded guidance on conditional field visibility, including adding rules from the Conditional logic pivot, using AND/OR conditions, default-hidden behavior until conditions are met, and visual indicators for conditional fields. Clarified interactions with branching and how read-only conditions can be created from Word template conditional sections. Documented supported master field types and operators, noted that Date and time fields can’t be used as master fields yet, and clarified validation for required fields when hidden. Highlighted that Power Automate doesn’t apply conditional visibility, with a tip to mark such fields optional when using flows.

  https://learn.microsoft.com/en-us/sharepoint/copilot-in-sharepoint-structured-document-generation

## Moderate Changes

- **How shareable links work in OneDrive and SharePoint in Microsoft 365**

  Updated guidance on expiration policies for “People in your organization” links, covering how new links receive expiration dates and how existing links are evaluated based on their original creation date. Clarified that only the link expires (not the content or other permissions) and refined wording about automatic redemption behavior when sending links from SharePoint/OneDrive, Outlook, or Teams chat.

  https://learn.microsoft.com/en-us/sharepoint/shareable-links-anyone-specific-people-organization