# Dynamics 365 Contact Center
**Date created:** 2026-08-27 UTC  
**Tags:** Automation, Configuration, Guidance  

## Moderate Changes

- **Use CCaaS_CreateProactiveBulkDelivery API**

  Corrected the V2 API name and endpoint to CCaaS_CreateProactiveDeliveryBulkV2 and aligned the request URL and headings accordingly. This removes naming inconsistencies and helps prevent integration errors; no API behavior changes were introduced.

  https://learn.microsoft.com/en-us/dynamics365/contact-center/extend/api/ccaas_createproactivebulkdelivery

- **Manage Customer Intent Agent**

  Expanded setup guidance to fine-tune intent discovery (granularity, count, mapping heuristics) and optionally auto-promote high-confidence intents with thresholds. Added instructions for reviewing and promoting updates to existing intents, including job details, change reasons, and patching titles, descriptions, and attributes; aligned terminology with AI agent and clarified using custom connectors for specific intents by exposing and mapping actions as tools.

  https://learn.microsoft.com/en-us/dynamics365/contact-center/administer/manage-customer-intent-agent