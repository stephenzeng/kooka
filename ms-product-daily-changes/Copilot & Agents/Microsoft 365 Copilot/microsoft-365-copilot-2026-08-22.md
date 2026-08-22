# Microsoft 365 Copilot
**Date created:** 2026-08-22 UTC  
**Tags:** Best Practices, Configuration, Get Started, Guidance  

## Major Changes

- **Build plugins for Copilot Cowork**

  Overhauled plugin development to center on the cross-platform Microsoft 365 Agents Toolkit CLI (atk), replacing the previous PowerShell conversion flow with an import/export model. Added step-by-step guidance for installing atk, importing Claude Code or Cursor plugins, handling required privacy/terms URLs, and packaging outputs, plus round-trip export back to a plugin directory. Clarified manifest and schema guidance (including devPreview vs v1.28), deterministic ID generation, and authentication handling with autodetection and override options, while flagging authorization.referenceId placeholders that must be updated before publishing. Marked the PowerShell script as legacy, removed the “accept files from the Cowork workspace” guidance, and refreshed examples to bash along with updated FAQs and icon behavior.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/cowork/cowork-plugin-development

## Moderate Changes

- **What's new in Copilot Cowork**

  Updated the July 2026 notes to remove the “Workspace file input for plugin tools” enhancement and its link, aligning the page with current capabilities. This avoids pointing readers to a deprecated approach and keeps the changelog accurate.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/cowork/whats-new