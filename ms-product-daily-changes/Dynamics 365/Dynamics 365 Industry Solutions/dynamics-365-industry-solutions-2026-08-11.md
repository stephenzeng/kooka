# Dynamics 365 Industry Solutions
**Date created:** 2026-08-11 UTC  
**Tags:** Configuration, Guidance, Performance  

## New Articles

- **Run Autodesk Maya on AMD-based V710 GPU on an Azure VM**

  Introduced a reference architecture for running Autodesk Maya 2025 on Azure NVads V710 v5 VMs with AMD Radeon PRO V710 GPUs. Provides end-to-end setup and validation guidance, including prerequisites, architecture and workflow, Azure components, and detailed Autodesk Hardware Certification Test Suite outcomes (all applicable tests passed; Arnold GPU marked not applicable due to CUDA requirement). Outlines scenarios and use cases and maps Well-Architected considerations across reliability, security, cost optimization, performance efficiency, scalability, and operational excellence. This helps teams confidently plan, configure, and validate Maya workloads on AMD-based Azure GPU VMs.

  https://learn.microsoft.com/en-us/industry/manufacturing/architecture/autodesk-maya-amd

## Major Changes

- **What's new in Microsoft for Manufacturing**

  Expanded the “What’s new” page with multiple updates across 2025–2026 to consolidate the latest guidance and validated results. Added August 2026 entries for running Autodesk Maya 2025 on AMD Radeon PRO V710 GPU–enabled Azure VMs and Autodesk AutoCAD 2027 on Azure NVads V710 v5. Extended July 2026 with Siemens NX performance validation on NVIDIA RTX PRO 6000 Blackwell GPUs and guidance for Ansys Discovery on Azure GPU VMs. Updated February 2026 with instructions to run Azure AI models on Siemens Industrial Edge with centralized monitoring, and added August 2025 content for PLM migration to Azure and using Icertis Contract Intelligence. These updates help manufacturers plan deployments with current, validated patterns and performance data.

  https://learn.microsoft.com/en-us/industry/manufacturing/whats-new

## Moderate Changes

- **Run Autodesk AutoCAD on AMD-powered Azure NVads V710 v5**

  Added a “How to interpret the results” section to guide proper use of benchmark data, focusing on per-scenario runtimes, avoiding cross-scenario comparisons, and limiting conclusions to the tested Standard_NV24ads_V710_v5 configuration. Clarified validation methodology to emphasize consistent iterations and the non-comparative scope, with minor refinements across Overview, Architecture, Workflow, Components, and Validation to better describe the environment and purpose.

  https://learn.microsoft.com/en-us/industry/manufacturing/architecture/autodesk-autocad-amd