# Dev and Admin for Dynamics 365 Business Central
**Date created:** 2026-08-04 UTC  
**Tags:** Agent, AI, Monitoring  

## Moderate Changes

- **ALTool**

  Updated the profiling tool to automatically estimate session memory usage during scheduled runs and embed the data in each .alcpuprofile. The stop-and-retrieve flow now includes session-level totals such as totalMemoryUsed (bytes) and totalObjectCount when memory estimation is enabled. Clarified that detailed per-type memory breakdown is emitted to server-side telemetry, improving analysis without bloating downloaded profiles.

  https://learn.microsoft.com/en-us/dynamics365/business-central/dev-itpro/developer/devenv-al-tool

- **Scheduled performance profiler overview**

  Expanded the profiler to capture and summarize session memory usage and object counts with every collected profile. Added guidance and a new Session memory usage section explaining how the data is automatically collected, stored with results, and presented for assessing memory impact.

  https://learn.microsoft.com/en-us/dynamics365/business-central/dev-itpro/administration/scheduled-performance-profiler-overview