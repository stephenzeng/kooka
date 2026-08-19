# Dynamics 365 Industry Solutions
**Date created:** 2026-08-19 UTC  
**Tags:** Best Practices, Configuration, Guidance, Monitoring, Performance, Security  

## New Articles

- **Run Siemens NX using AMD Radeon PRO V710 GPUs on Azure Virtual Desktop**

  Introduced a reference architecture validating Siemens NX 2506 on Azure Virtual Desktop using AMD Radeon PRO V710 GPUs (NVads V710 v5). The article outlines prerequisites such as Windows 11 multi-session, AMD driver version 32.0.21017.2052, AVD setup, and a licensing server. It provides storage guidance for managed disks with alternatives like Azure Files and Azure NetApp Files. Comprehensive validation covers Standard_NV12ads_V710_v5 and Standard_NV24ads_V710_v5 VM sizes, single- and multi-host scenarios up to 30 users, with measured runtimes and analysis. Well-Architected guidance addresses reliability, security (including licensing port 28000), cost, operations, performance efficiency, and scaling with host pool load balancing and scaling plans.

  https://learn.microsoft.com/en-us/industry/manufacturing/architecture/siemens-azure-amd

## Moderate Changes

- **Overview of Microsoft for Manufacturing reference architectures**

  Added a link to new guidance for running Siemens NX on Azure Virtual Desktop with AMD Radeon PRO V710 GPUs and updated the NVIDIA Blackwell item to emphasize RTX PRO 6000 Blackwell GPUs. These updates clarify GPU options and improve discoverability of the latest validated configurations for design workloads.

  https://learn.microsoft.com/en-us/industry/manufacturing/architecture/ra-overview

- **Digital engineering**

  Added a reference architecture entry for Siemens NX on Azure Virtual Desktop using AMD Radeon PRO V710 GPUs and retitled the NVIDIA Blackwell entry for clarity and consistency. This improves navigation and helps readers choose the appropriate GPU-backed configuration for engineering scenarios.

  https://learn.microsoft.com/en-us/industry/manufacturing/unlock-innovation

- **What's new in Microsoft for Manufacturing**

  Highlighted a new feature entry covering proof-of-concept validation of Siemens NX 2506 on Azure Virtual Desktop with AMD Radeon PRO V710 GPUs (NVads V710 v5). This provides visibility into newly validated GPU options and their performance implications for engineering workloads.

  https://learn.microsoft.com/en-us/industry/manufacturing/whats-new