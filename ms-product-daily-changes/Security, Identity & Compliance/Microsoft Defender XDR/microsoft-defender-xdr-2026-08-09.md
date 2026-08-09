# Microsoft Defender XDR
**Date created:** 2026-08-09 UTC  
**Tags:** Security  

## Moderate Changes

- **Configure Azure Event Hubs to export Microsoft Defender XDR data**

  Updated guidance provides an end-to-end configuration flow, clarifies Azure resource provider and Microsoft Entra app registration (including service principal context and one-time client secret visibility), and specifies required roles. It refines Event Hubs setup with pricing/throughput/auto-inflate recommendations, partition guidance, resource ID usage, and when to use a single hub versus one per event type, including cases where Defender XDR auto-creates hubs. Verification steps were enhanced with an Advanced Hunting query explanation to confirm successful export, and scenarios were reorganized to cover email table export and Splunk via Event Hubs.

  https://learn.microsoft.com/en-us/defender-xdr/configure-event-hub