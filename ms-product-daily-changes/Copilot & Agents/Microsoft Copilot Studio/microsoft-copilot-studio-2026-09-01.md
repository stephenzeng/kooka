# Microsoft Copilot Studio
**Date created:** 2026-09-01 UTC  
**Tags:** Automation, Billing, Compliance, Get Started, Governance, Guidance, Licensing, Troubleshooting  

## Moderate Changes

- **Overview of billing for agents and workflows powered by the GitHub Copilot harness**

  Expanded billing guidance to cover both agents and workflows, with a new banner highlighting the updated experience. Clarified that Copilot credits measure usage across agents and workflows, and that consumption varies by design choices, run frequency, and enabled features. Standardized terminology and refreshed “What’s new” details to align with usage-based billing.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/agents-experience/billing-credit-overview

- **Create a new agent**

  Added a public preview path to create agents directly from Copilot chat, including artifact cards with clear actions (open, preview/publish and test, settings, delete). Documented how to delete generated agents from chat with safeguards and permanence, and expanded next steps to guide users to add knowledge, tools, skills, testing, and sharing.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/agents-experience/build-new-agent

- **Edit and manage your workflow in the designer**

  Introduced sample values in the token picker sourced from the most recent successful test run to speed configuration and mapping. Added instructions for deleting chat-generated workflows from the artifact card, including confirmation, permanent removal, and clearing of run history. Minor wording updates improve clarity in testing and UI references.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/workflows-experience/flow-designer

- **Publish an agent**

  Updated publishing guidance to reflect how organizational data loss prevention policies are enforced, including blocked channels/connectors and related notifications. Clarified that the built-in Direct Line test channel doesn’t block publishing but policies still apply at runtime, and outlined conditions when publishing is blocked. The publish dialog now surfaces blocking details with direction to reconfigure channels or work with an administrator.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/agents-experience/publication-publish-agent

- **Manage and delete skills in an agent**

  Added troubleshooting for skills that fail to load, with common root causes and fixes such as invalid or missing metadata, duplicate names, encoding issues, and partial file writes. Notes that partially written files can affect runtime behavior and recommends re-uploading the package after correcting issues.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/agents-experience/skills-manage