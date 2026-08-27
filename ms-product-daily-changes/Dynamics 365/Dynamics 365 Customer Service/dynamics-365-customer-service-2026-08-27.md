# Dynamics 365 Customer Service
**Date created:** 2026-08-27 UTC  
**Tags:** Best Practices, Configuration, Guidance  

## Moderate Changes

- **Automatically create or update records in Dynamics 365 Customer Service**

  Added guidance to use a single automatic record creation and update rule when monitoring multiple queues to avoid duplicate case creation. Outlines routing emails from multiple mailboxes to a dedicated queue using Exchange transport rules or Dynamics 365 processing (Power Automate or plug-ins), with an illustrative diagram. Updated terminology to Dataverse tables/records for clarity.

  https://learn.microsoft.com/en-us/dynamics365/customer-service/administer/automatically-create-update-records

- **Configure Service Agent Experiences**

  Reorganized configuration guidance around a clear maker mode flow—select scope, make changes, review/reset, and exit—to streamline setup within Service Agent. Consolidated steps by removing references to configuring in other locations, clarified timelines/picklists/lookups, and refined tool visibility guidance including customer-defined MCP tools. Renamed and expanded the namespace section to explain what a namespace is and how to manage tools per namespace.

  https://learn.microsoft.com/en-us/dynamics365/customer-service/administer/configure-service-agent-experiences