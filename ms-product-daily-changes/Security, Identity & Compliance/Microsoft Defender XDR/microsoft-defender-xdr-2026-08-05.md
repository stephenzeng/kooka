# Microsoft Defender XDR
**Date created:** 2026-08-05 UTC  
**Tags:** Administration, Analytics, Security  

## Major Changes

- **OAuthAppInfo (Preview)**

  Clarified coverage by replacing references to “apps without OAuth consents” with Entra managed identities, improving accuracy of guidance. Added RiskScore (integer) to expose the Defender-calculated application risk and AssignedRoles (dynamic) to list active roles on the service principal (currently Entra roles only). These additions help analysts assess app risk and understand role-based privileges directly in advanced hunting. The updates make investigations and query results more precise and actionable.

  https://learn.microsoft.com/en-us/defender-xdr/advanced-hunting-oauthappinfo-table

## Moderate Changes

- **Alert policies in the Microsoft Defender portal**

  Added an IMPORTANT note that some default alert policies include hidden filters not shown in the portal, which can affect alert matching. Provided guidance to use the Get-ProtectionAlert cmdlet with IncludeRuleXml to review full rule definitions, including an example command for listing policy properties. This helps admins troubleshoot unexpected alert behavior and validate policy logic.

  https://learn.microsoft.com/en-us/defender-xdr/alert-policies