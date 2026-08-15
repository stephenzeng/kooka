# Visual Studio
**Date created:** 2026-08-15 UTC  
**Tags:** Configuration, Guidance  

## Moderate Changes

- **Change waves**

  Updated guidance explaining that persistent MSBuild processes keep the MSBuildDisableFeaturesFromVersion environment variable value from when they started. After changing this variable, shut down build processes to apply the new value—use 'dotnet build-server shutdown' for .NET CLI builds, and close Visual Studio and terminate any MSBuild.exe processes for Visual Studio/MSBuild builds. This prevents reused or parallel processes from using inconsistent or outdated settings.

  https://learn.microsoft.com/en-us/visualstudio/msbuild/change-waves?view=visualstudio