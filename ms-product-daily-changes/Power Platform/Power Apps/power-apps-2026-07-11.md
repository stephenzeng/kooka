# Power Apps
**Date created:** 2026-07-11 UTC  
**Tags:** AI, Administration, Automation, Programming  

## New Articles

- **Configure structured content in the rich text editor (preview)**
  
  Introduced step-by-step guidance to enable and use structured content in the rich text editor for model-driven apps with Copilot-powered templates. Covers prerequisites such as Copilot control, pay-as-you-go billing, and cross-geo settings, plus how to turn on the feature in admin settings. Explains creating and managing templates (name, description, structuring prompt), the user flow to generate structured content, and billing considerations for preview and GA. Includes troubleshooting for common errors like disabled Copilot, exhausted credits, or missing prerequisites.
  
  https://learn.microsoft.com/en-us/power-apps/maker/model-driven-apps/rte-structured-notes

## Major Changes

- **Supported customizations for Microsoft Dataverse**
  
  Expanded and clarified platform targets for custom code, including support for web service clients on .NET Framework 4.6.2+ with a recommendation to target 4.8 or later. Added guidance that web service clients targeting .NET Core 8 or higher are supported. Explicitly disallowed registering or running plug-ins and custom workflow activities from assemblies targeting any version of .NET Core. This helps teams align their build targets with supported platforms and avoid unsupported deployments.
  
  https://learn.microsoft.com/en-us/power-apps/developer/data-platform/supported-customizations

## Moderate Changes

- **Build and package plug-in code**
  
  Updated guidance to target supported .NET Framework versions rather than a fixed 4.6.2 requirement, with a link to the supported versions page. Expanded NuGet guidance to include Microsoft.PowerPlatform.Dataverse.Client alongside Microsoft.CrmSdk.CoreAssemblies to ensure correct Dataverse references.
  
  https://learn.microsoft.com/en-us/power-apps/developer/data-platform/build-and-package

- **Transition client applications to Dataverse ServiceClient**
  
  Noted Event Framework (sandbox) support for .NET Framework 4.8 and recommended rebuilding plug-ins and custom workflow activities to target 4.8, while keeping earlier 4.6.2–4.7.x targets supported. Reaffirmed using Microsoft.CrmSdk.CoreAssemblies for these components to maintain compatibility.
  
  https://learn.microsoft.com/en-us/power-apps/developer/data-platform/sdk-client-transition

- **Tutorial: Create workflow extension (Microsoft Dataverse) | Microsoft Docs**
  
  Revised setup instructions to require a supported .NET Framework version instead of a hardcoded 4.6.2, linking to authoritative supported frameworks guidance. This prevents pinning to an outdated version and improves forward compatibility.
  
  https://learn.microsoft.com/en-us/power-apps/developer/data-platform/workflow/tutorial-create-workflow-extension

- **Tutorial: Write and register a plug-in (Microsoft Dataverse) | Microsoft Docs**
  
  Updated project setup to target a supported .NET Framework version and referenced the supported versions guidance. This streamlines upgrades and ensures compliance with current platform support.
  
  https://learn.microsoft.com/en-us/power-apps/developer/data-platform/tutorial-write-plug-in

- **Visual Studio and the .NET platform**
  
  Clarified that Dataverse SDK assemblies support both .NET Framework and .NET Core and that development can use Visual Studio, Visual Studio Code, or other tools. Removed outdated version-specific and TLS notes, and refined setup steps to install the .NET Framework Developer Pack and, for .NET Core, the SDK; also clarified Visual Studio Express limitations.
  
  https://learn.microsoft.com/en-us/power-apps/developer/data-platform/org-service/visual-studio-dot-net-framework

- **Create Workflow Extensions for Microsoft Dataverse**
  
  Aligned custom workflow activity guidance to target supported .NET Framework versions instead of a fixed 4.6.2 and adjusted related instructions. Clarified how parameters appear in the process designer to reduce configuration errors.
  
  https://learn.microsoft.com/en-us/power-apps/developer/data-platform/workflow/workflow-extensions

- **Write a plug-in (Microsoft Dataverse) | Microsoft Docs**
  
  Simplified plug-in targeting guidance to use supported .NET Framework versions and linked to official support details. This reduces maintenance risk and keeps projects aligned with platform updates.
  
  https://learn.microsoft.com/en-us/power-apps/developer/data-platform/write-plug-in