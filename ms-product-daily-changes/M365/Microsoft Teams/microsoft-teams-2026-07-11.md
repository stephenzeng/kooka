# Microsoft Teams
**Date created:** 2026-07-11 UTC  
**Tags:** Administration, Security  

## Major Changes

- **Manage updates for Teams android devices in Pro Management portal (PMP)**

  Expanded and clarified the transition of Teams Android device update management from Teams Admin Center (TAC) to Teams Rooms Pro Management portal (PMP), including timeline and key dates. Clarifies that TAC auto-updates stop as PMP becomes primary; admins must confirm PMP ring usage, the switch is irreversible, and TAC phases are mapped once to PMP default rings which may roll out faster. Adds operational specifics like a nightly 1–5 AM local maintenance window, non-disruptive updates, coordinated updates for paired devices, update states/visibility, ring management, migration of tenant-wide pause behavior, and admin role/post-migration responsibilities. Details Teams Phones requirements tied to Admin Agent version 830+ (agent updates via TAC until 830, other updates paused; after 830, PMP manages; limited historical update visibility). Provides GCC/GCCH/DoD guidance noting no TAC auto-update for AA 830+ and recommending manual updates and early PMP adoption, with possible accelerated agent deployment.

  https://learn.microsoft.com/en-us/microsoftteams/rooms/androidupdatemanagementinpmp

## Moderate Changes

- **Teams Rooms certified systems and peripherals**

  Added new certified options for Teams Rooms on Windows, including three Crestron Intelligent Audio AP-100 ceiling system configurations and two Crestron Collab Compute models (CCC-110-T and CCC-120-T). Also added Lenovo ThinkSmart One Pro kits with Core Controller and IP Controller configurations, expanding validated hardware choices for varied room sizes and performance needs.

  https://learn.microsoft.com/en-us/microsoftteams/rooms/certified-hardware

- **Meetings and events feature and capacity comparison**

  Added a comparison row for “Join verification for external presenters,” indicating it’s not applicable to standard meetings and is available for webinars and town halls. This helps organizers choose the right event type when identity verification for external presenters is required.

  https://learn.microsoft.com/en-us/microsoftteams/meetings-events-feature-comparison

- **Plan for Teams events**

  Added admin and organizer policy entries for “Join verification for external presenters,” enabling admins to require identity verification for anonymous or unverified presenters. Organizers can require verification in meeting options when admins do not mandate it, improving event security and governance.

  https://learn.microsoft.com/en-us/microsoftteams/plan-events