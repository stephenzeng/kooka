# Power Automate
**Date created:** 2026-08-02 UTC  
**Tags:** Administration, Automation  

## Moderate Changes

- **Create child flows**

  Clarified licensing and capacity behavior for Process licenses: child flows don’t inherit capacity from a parent flow’s flow group, and both must be explicitly added to the same group to share capacity. Reinforced that each parent and child flow counts separately toward the 25-flow limit.

  https://learn.microsoft.com/en-us/power-automate/create-child-flows

- **Create and manage a flow group**

  Updated guidance to state that adding a parent flow to a group doesn’t automatically include its child flows; each child must be added individually and each counts toward the 25-flow limit. Instructions and deployment steps now explicitly require adding every parent and child flow to the group.

  https://learn.microsoft.com/en-us/power-automate/create-flow-group

- **Share Process license capacity with flow groups**

  Clarified that only flows explicitly added to a group consume its shared Process license capacity, and that parent and child flows are separate members. Updated eligibility and limits to reflect explicit inclusion of both and that each counts toward the 25-flow cap.

  https://learn.microsoft.com/en-us/power-automate/flow-groups