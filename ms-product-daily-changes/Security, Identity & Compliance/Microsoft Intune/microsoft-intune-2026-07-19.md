# Microsoft Intune
**Date created:** 2026-07-19 UTC  
**Tags:** Administration  

## Moderate Changes

- **Packages and programs in Configuration Manager**

  Updated guidance to explain that on 64-bit clients, package and program command lines run as 32-bit processes under WOW64, and advised using %windir%\Sysnative to invoke 64-bit binaries when needed. Clarified which user sees package and task sequence deployments in Software Center when multiple users are signed in, and how to identify session IDs and types using Task Manager.

  https://learn.microsoft.com/en-us/intune/configmgr/apps/deploy-use/packages-and-programs