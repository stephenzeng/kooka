# Microsoft Intune
**Date created:** 2026-07-20 UTC  
**Tags:** Administration  

## Major Changes

- **Introduction to software updates in Configuration Manager**

  Updated compliance scan guidance to clearly distinguish forced vs. non-forced and online vs. offline scans, clarifying WSUS connection behavior and TTL cache reuse. Added an explicit note that “online” indicates capability, not a guaranteed WSUS contact, and explained why forced offline scenarios are valid. Introduced a flowchart and summary table to visualize scan decision paths and WSUS contact conditions, improving troubleshooting and planning. Added sections clarifying that a single scan evaluates the entire synchronized catalog and that compliance refresh is separate from deployment policy retrieval, with guidance on which client actions to run for each.

  https://learn.microsoft.com/en-us/intune/configmgr/sum/understand/software-updates-introduction