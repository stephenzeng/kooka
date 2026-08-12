# Visual Studio
**Date created:** 2026-08-12 UTC  
**Tags:** Configuration  

## Moderate Changes

- **Common MSBuild Project Properties**

  Updated guidance on the Deterministic property to clarify that it governs whether supported tasks and tools produce deterministic outputs and that compiled assemblies map to the /deterministic compiler switch. Added a new DeterministicTimestamp property with support for RFC 3339 date/time or Unix timestamps, enabling consistent timestamps in outputs (e.g., archive/package entries) and compatibility with SOURCE_DATE_EPOCH. These changes improve reproducible build configurations and documentation clarity.

  https://learn.microsoft.com/en-us/visualstudio/msbuild/common-msbuild-project-properties?view=visualstudio