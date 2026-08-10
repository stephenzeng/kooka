# Power Automate
**Date created:** 2026-07-19 UTC  
**Tags:** Administration, Automation, Governance  

## New Articles

- **Create and manage a flow group**

  Introduced a step-by-step how-to for creating and managing flow groups to share a single Process license’s daily capacity across up to 25 solution-aware cloud flows. Covers identifying candidate flows using daily action usage and admin reports, assigning a Process license to a group, and adding or removing flows from the group. Provides guidance on monitoring capacity, handling cases where one flow dominates usage, and warnings related to license changes. Includes deployment considerations across environments, rollout timeline notes, error handling when no capacity is available, and related links, including importing an existing group definition.

  https://learn.microsoft.com/en-us/power-automate/create-flow-group

- **Share Process license capacity with flow groups**

  Introduces the flow groups concept that allows up to 25 solution-aware cloud flows (including child runs) to share a single Process license’s daily capacity of 250,000 actions. Clarifies that capacity pools at the group level, license stacking isn’t supported for groups, and high-usage workloads should assign licenses directly to individual flows. Details prerequisites, eligibility (solution-aware cloud flows only), and limits such as single-environment scope and one group membership per flow, with links to setup and licensing guidance.

  https://learn.microsoft.com/en-us/power-automate/flow-groups

## Moderate Changes

- **How to use process capacity**

  Updated licensing guidance to enable assigning a Process license directly to an individual flow or to a flow group. Clarifies that a single Process license can be shared across up to 25 flows within a group and that child flows must be explicitly added to the group to consume shared capacity.

  https://learn.microsoft.com/en-us/power-automate/desktop-flows/capacity-process

- **Limits of automated, scheduled, and instant flows**

  Added licensing guidance for cloud flows enabling a single Process license to be shared across up to 25 flows via flow groups. Clarifies that license stacking isn’t supported for groups and that workloads exceeding 250,000 actions per day should license individual flows directly.

  https://learn.microsoft.com/en-us/power-automate/limits-and-config

- **Support for service principal owned flows**

  Clarified that premium service principal application user–owned flows can be licensed via a Process license, a per-flow license, or through membership in a flow group with a Process license. Retains existing exemptions for flows without premium connectors or those running solely within Dynamics 365 contexts.

  https://learn.microsoft.com/en-us/power-automate/service-principal-support