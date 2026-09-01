# Visual Studio
**Date created:** 2026-09-01 UTC  
**Tags:** Configuration, Guidance, Performance, Security  

## Major Changes

- **MSBuild Server**

  Updated guidance reflects that starting with the .NET 11 SDK, MSBuild Server is enabled by default for MSBuild-based .NET CLI commands, improving startup and build responsiveness. Multithreaded builds automatically use the server, while disabling node reuse (/nr:false or /node-reuse:false) turns it off and runs the build in-process. The server is not used for certain commands (for example, -help, -version, or replaying a binary log) and these scenarios fall back to in-process execution. Diagnostics to confirm server usage are available via -v:diag or binary logs (-bl), and opting out is now done with DOTNET_CLI_USE_MSBUILD_SERVER=false.

  https://learn.microsoft.com/en-us/visualstudio/msbuild/msbuild-server?view=visualstudio

## Moderate Changes

- **Change waves**

  Added change waves 18.10 and 18.9 with improvements to reliability, performance, and security: stable project paths on Unix via PWD under symlinks, faster evaluations for -getProperty/-getItem, and restore avoiding a second evaluation. GenerateResource now blocks typed ResX entries in Mark-of-the-Web files (MSB3821) with an opt-out via MSBUILDDISABLEFEATURESFROMVERSION=18.9, while ResXFileRef entries remain blocked for safety. Defaults were tuned for throughput, including a 1 MB TaskHost named-pipe buffer (configurable) and updated logging that surfaces log file paths at the end of builds.

  https://learn.microsoft.com/en-us/visualstudio/msbuild/change-waves?view=visualstudio