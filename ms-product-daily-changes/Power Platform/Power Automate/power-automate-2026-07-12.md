# Power Automate
**Date created:** 2026-07-12 UTC  
**Tags:** Administration, AI, Automation, Governance  

## New Articles

- **AI-assisted UI automation repair (preview)**

  Introduced an AI-powered feature that helps repair broken UI/browser selectors during debugging in Power Automate for desktop. The capability is available to organization premium accounts (not in government/sovereign clouds), operates only in the designer during debugging, and is distinct from runtime self-healing. Admins must enable Copilot in the Power Platform admin center, and clients require Power Automate for desktop v2.70 or later. Guidance covers how to run with AI-assisted repair, review and test suggested selectors, and accept or skip changes, with noted limits to selector-related issues that require user review.

  https://learn.microsoft.com/en-us/power-automate/desktop-flows/ai-assisted-ui-automation-repair

- **Trigger actions reference**

  Added a new reference for desktop flow trigger actions that monitor mouse and keyboard events on UI elements. The article explains trigger behavior (one-time or sequential), timeout handling, and how to stop monitoring. It documents inputs for the UI element event trigger, the output handle variable, and defined exceptions for failures and timeouts.

  https://learn.microsoft.com/en-us/power-automate/desktop-flows/actions-reference/triggers

## Moderate Changes

- **Actions reference**

  Updated the action groups index to include Triggers and Power Automate environment, and reorganized several groups to improve discoverability. This refinement helps users locate related actions more quickly without content removals.

  https://learn.microsoft.com/en-us/power-automate/desktop-flows/actions-reference

- **Governance in Power Automate for desktop**

  Added guidance on a registry key (Global\PreserveCustomServiceAccount) to preserve custom UIFlowService accounts across MSI upgrades (v2.69+). The update clarifies first-upgrade behavior from older versions and how setting the key to 1 preserves the custom account, while removing it or setting 0 reverts to the default service on the next upgrade.

  https://learn.microsoft.com/en-us/power-automate/desktop-flows/governance

- **Self-healing (preview)**

  Expanded supported error types to include Window not found and clarified behavior across primary and secondary screens. Updated admin guidance for enabling Copilot-related settings and noted that run pages now show a summary of up to three successful self-healing attempts, with a registry-based option still available for detailed local logs.

  https://learn.microsoft.com/en-us/power-automate/desktop-flows/self-healing

- **Tags in desktop flows**

  Updated guidance to reflect that tags can be managed in both the Power Automate for desktop console and the Power Automate portal. Clarified entry points to Manage tags and removed a prior limitation, signaling broader visibility and management of tags across experiences.

  https://learn.microsoft.com/en-us/power-automate/desktop-flows/tags