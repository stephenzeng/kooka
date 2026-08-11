# Microsoft Defender XDR
**Date created:** 2026-08-04 UTC  
**Tags:** Administration, Analytics, Monitoring, Security  

## Major Changes

- **AADSignInEventsBeta table in the advanced hunting schema (deprecated)**

  Marked AADSignInEventsBeta as deprecated and updated the Important notice with an October 19, 2026 retirement date. Clarified that EntraIdSignInEvents will replace this table and that existing queries will be automatically migrated on the retirement date. This sets clear timelines and reduces migration effort for existing hunting content.

  https://learn.microsoft.com/en-us/defender-xdr/advanced-hunting-aadsignineventsbeta-table

- **EntraIdSignInEvents**

  Updated the migration notice: AADSignInEventsBeta will be replaced by EntraIdSignInEvents on October 19, 2026, with automatic query migration and no changes required for custom detections. Expanded the schema with new fields (for example, GatewayJA4, TenantId, Type, SourceSystem, TimeGenerated, UniqueTokenId, IsSignInThroughGlobalSecureAccess) and documented EndpointCall in the main field list. Adjusted field semantics (TokenIssuerType from int to string; RiskDetails replaced by RiskLevelDuringSignIn and RiskEventTypes; corrected IsGuestUser description) and removed IsConfidentialClient. These updates add coverage and clarity, and may require updates to parsing and enrichment logic.

  https://learn.microsoft.com/en-us/defender-xdr/advanced-hunting-entraidsigninevents-table

- **EntraIdSpnSignInEvents**

  Announced that EntraIdSpnSignInEvents will replace AADSpnSignInEventsBeta on October 19, 2026, with automatic migration of queries and no action required for custom detections. Expanded the schema with fields including IsConfidentialClient, GatewayJA4, SessionId, UserAgent, TenantId, Type, SourceSystem, TimeGenerated, and UniqueTokenId. The changes enhance service principal sign-in telemetry and may inform updated analytics.

  https://learn.microsoft.com/en-us/defender-xdr/advanced-hunting-entraidspnsigninevents-table

- **GraphAPIAuditEvents table in the advanced hunting schema**

  Standardized the table name to GraphAPIAuditEvents and replaced IPAddress with correctly cased IpAddress. Added ReportId, TenantId, Type, SourceSystem, and TimeGenerated, and changed data types (Timestamp to datetime, ResponseSize to long). Refined several field descriptions and reordered key columns. These schema changes are material and may require updates to queries, parsers, and data pipelines.

  https://learn.microsoft.com/en-us/defender-xdr/advanced-hunting-graphapiauditevents-table

- **Microsoft Defender XDR Advanced hunting API**

  Added a deprecation notice indicating the Defender XDR advanced hunting API is transitioning to the Microsoft Graph security API. Retirement begins January 2026, after which the API will stop functioning. Included migration guidance and reinforced using Microsoft Graph for advanced hunting. Customers should plan and execute migrations to avoid service disruption.

  https://learn.microsoft.com/en-us/defender-xdr/api-advanced-hunting

- **Investigate an identity**

  Expanded guidance for identity investigations with updated screenshots and a significantly enhanced Timeline tab that aggregates signals across on-premises AD, Microsoft Entra ID, IAM providers, SaaS apps, cloud, and endpoints. Documented deduplication behavior, correlated account coverage, and newly supported data types such as Entra ID risk signals and Conditional Access evaluations. Added a list of advanced hunting tables feeding the identity timeline and a detailed timeline schema with normalized columns and filterability. Introduced an Event details pane highlighting Conditional Access policy evaluation, improving visibility and triage workflows.

  https://learn.microsoft.com/en-us/defender-xdr/investigate-users

## Moderate Changes

- **AADSpnSignInEventsBeta table in the advanced hunting schema (deprecated)**

  Marked AADSpnSignInEventsBeta as deprecated with an October 19, 2026 retirement date. Clarified that queries will be automatically migrated to EntraIdSpnSignInEvents, minimizing required user action.

  https://learn.microsoft.com/en-us/defender-xdr/advanced-hunting-aadspnsignineventsbeta-table

- **CloudDnsEvents**

  Added three new columns: ImageDigest (container image digest), Region (cluster region), and HostName (node hostname). This enriches cloud DNS telemetry for better container and infrastructure context in investigations.

  https://learn.microsoft.com/en-us/defender-xdr/advanced-hunting-clouddnsevents-table

- **EmailEvents**

  Clarified Streaming API behavior: a new record is emitted when an email’s verdict or delivery location changes. Added SIEM guidance with a KQL example using summarize arg_max by NetworkMessageId and RecipientEmailAddress to return the latest record per message-recipient pair, helping avoid duplicate alerts.

  https://learn.microsoft.com/en-us/defender-xdr/advanced-hunting-emailevents-table

- **Take action on advanced hunting results in Microsoft Defender XDR**

  Expanded remediation to include identity actions (Disable user, Reset user authentication) with parameter requirements such as SID and AccountObjectId. Updated descriptions and references to identity and file actions to streamline response playbooks across identities, devices, files, and emails.

  https://learn.microsoft.com/en-us/defender-xdr/advanced-hunting-take-action

- **Map existing RBAC permissions to Microsoft Defender unified RBAC permissions**

  Added the SOC Identity Responder role with permissions to read security data basics and manage alerts and response. This update helps map existing responsibilities to unified RBAC for identity-focused operations.

  https://learn.microsoft.com/en-us/defender-xdr/compare-rbac-roles

- **What's new in Microsoft Defender XDR**

  Added a July 2026 entry announcing the October 19, 2026 deprecation of AADSignInEventsBeta and AADSpnSignInEventsBeta, replaced by EntraIdSignInEvents and EntraIdSpnSignInEvents. Noted automatic migration of queries and availability of the new Entra ID tables for early adoption.

  https://learn.microsoft.com/en-us/defender-xdr/whats-new