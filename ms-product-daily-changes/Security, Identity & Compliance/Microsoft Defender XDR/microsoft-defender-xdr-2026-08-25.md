# Microsoft Defender XDR
**Date created:** 2026-08-25 UTC  
**Tags:** Analytics, Guidance, Security  

## Moderate Changes

- **DeviceLogonEvents table in the advanced hunting schema**

  Updated guidance to document access-token privilege context available in AdditionalFields for token creation events initiated by lsass.exe, including flags indicating high-privilege group SIDs and counts that reflect logon-time group membership. Added a sample Kusto query to help analysts hunt for and parse privileged token creation activity. Refined several column descriptions for greater precision and consistency, including UAC terminology and SHA-256 guidance.

  https://learn.microsoft.com/en-us/defender-xdr/advanced-hunting-devicelogonevents-table