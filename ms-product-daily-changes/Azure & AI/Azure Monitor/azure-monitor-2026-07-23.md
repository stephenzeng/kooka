# Azure Monitor
**Date created:** 2026-07-23 UTC  
**Tags:** Monitoring  

## Major Changes

- **Legacy authentication for Container Insights**

  Announced a deprecation timeline: legacy authentication will be retired after September 30, 2026, requiring migration to managed identity. Updated migration guidance highlights advantages of managed identity, including support for syslog collection and high-scale logs mode. Clarified that Arc-enabled Azure Red Hat OpenShift supports managed identity, enabling customers to migrate now. Added detailed migration impact notes and post-migration validation steps to help confirm data flow, dashboards, alerts, and custom configurations continue to work.

  https://learn.microsoft.com/en-us/azure/azure-monitor/containers/container-insights-authentication