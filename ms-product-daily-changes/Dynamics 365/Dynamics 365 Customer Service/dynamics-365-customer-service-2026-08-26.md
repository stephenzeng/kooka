# Dynamics 365 Customer Service
**Date created:** 2026-08-26 UTC  
**Tags:** Configuration, Guidance  

## Major Changes

- **Add a timer control for SLA-enabled tables**
  
  Updated guidance to use table-based terminology and the modern Power Apps form designer. Provides streamlined steps to add an SLA timer via a subgrid on the Case table, including configuring the data source, default view, update frequency, negative countdown, and label bindings. Retired legacy Web Client and classic customization instructions to reduce confusion and align with current experiences. Consolidated runtime behavior notes and preserved troubleshooting resources to improve setup and support.

  https://learn.microsoft.com/en-us/dynamics365/customer-service/administer/add-timer-control-case-form-track-time-against-sla

## Moderate Changes

- **Understand how unified routing affects queue items and live work items for routed records**
  
  Expanded guidance for moving records between advanced queues and clarified the resulting system actions. When a record is moved, the live work item shifts to the target queue, the agent is unassigned, capacity is released, the item returns to routing as unassigned, and subsequent handling depends on the workstream type with references to workstream configuration.

  https://learn.microsoft.com/en-us/dynamics365/customer-service/develop/unified-routing-impact-on-APIs