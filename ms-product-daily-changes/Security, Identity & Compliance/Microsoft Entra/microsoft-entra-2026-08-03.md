# Microsoft Entra
**Date created:** 2026-08-03 UTC  
**Tags:** AI, Administration, Security  

## Major Changes

- **How to manage the Internet Access profile**

  Expanded Internet Access profile capabilities to support routing through remote networks and refined include/exclude traffic configuration. Introduced new policy types—Microsoft Traffic Bypass, Custom Acquire with selective acquisition (by protocol and ports), and Agentic Acquire for local AI agents like GitHub Copilot CLI and Claude CLI—with updated rule evaluation so Default Acquire is considered after bypass and custom acquire. Enhanced Custom Bypass to specify protocols and ports, and added guided procedures for creating Custom Bypass/Acquire rules, including when to disable Default Acquire. Added setup steps and platform/minimum client version details for Agentic Acquire, and clarified traffic evaluation order and coexistence with third-party SWG solutions.

  https://learn.microsoft.com/en-us/entra/global-secure-access/how-to-manage-internet-access-profile