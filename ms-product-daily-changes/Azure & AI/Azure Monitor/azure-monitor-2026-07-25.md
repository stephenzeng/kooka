# Azure Monitor
**Date created:** 2026-07-25 UTC  
**Tags:** Agent, Monitoring, Security  

## Major Changes

- **Azure Monitor Agent extension versions**

  Added July 2026 release details for Linux agent version 1.43, improving CEF event detection after long prefixes, fixing disk-space checks to target actual volumes, correctly honoring "true" string values in public settings, and preventing crashes when rows contain null strings in Log Analytics. Updated the release table to include July 2026 and consolidated legacy entries under a new "Older versions (Unsupported)" section for clearer lifecycle guidance. Clarified the rollout model to a coordinated, region-by-region deployment across Azure VMs, VMSS, and Arc-enabled servers with a 4–6 week timeline, removing prior guidance about manual installs. These changes enhance reliability, reduce operational risk during upgrades, and set clearer expectations for version availability and support status.

  https://learn.microsoft.com/en-us/azure/azure-monitor/agents/azure-monitor-agent-extension-versions