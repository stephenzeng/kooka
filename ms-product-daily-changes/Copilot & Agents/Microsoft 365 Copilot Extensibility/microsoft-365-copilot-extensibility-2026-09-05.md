# Microsoft 365 Copilot Extensibility
**Date created:** 2026-09-05 UTC  
**Tags:** Automation, Configuration, Get Started, Governance, Guidance, Security  

## New Articles

- **Add custom skills to your declarative agent in Agent Builder (preview)**
  Introduced a step-by-step guide to add custom skills to declarative agents in Agent Builder using zipped skill packages. Provides prerequisites, usage limits (up to eight skills per agent; .zip up to 50 MB), and guidance to generate a skill from natural-language prompts in Copilot chat. Clarifies required package structure (SKILL.md plus optional resources/scripts) and instruction constraints to ensure reliable execution. Helps makers quickly upload, configure, and test skills, accelerating prototyping and governed rollout.
  https://learn.microsoft.com/en-us/microsoft-365/copilot/extensibility/agent-builder-add-skills

- **Add custom skills to a declarative agent created with Microsoft 365 Agents Toolkit (preview)**
  Added a how-to for creating and managing custom skills with the Agents Toolkit via CLI and the Visual Studio Code extension. Explains enabling the TEAMSFX_AGENT_SKILLS environment variable, working with skill folders (not .zip), and meeting manifest version 1.9 requirements. Details limits and known issues (for example, up to 8 skills, 10 MB app package, max directory depth of 3, and 400 files) to prevent deployment failures. This guidance streamlines local development, provisioning, and testing workflows for skill-enabled agents.
  https://learn.microsoft.com/en-us/microsoft-365/copilot/extensibility/build-declarative-agents-add-custom-skills

- **Custom skills in declarative agents (preview)**
  Introduced a conceptual overview of custom skills, defining the SKILL.md–based structure and how skills replace inline task instructions for modularity and accuracy. Outlines benefits, supported file/script types, and a support matrix across Agent Builder and Agents Toolkit, including key limits on size, depth, and count. Clarifies sandbox execution constraints (no network access or runtime package install; use only preinstalled packages) and data handling (sensitivity labels honored; storage in tenant-scoped SharePoint Embedded). Highlights a known preview limitation that agents cannot combine skills with embedded files, helping teams plan implementations accordingly.
  https://learn.microsoft.com/en-us/microsoft-365/copilot/extensibility/declarative-agent-skills

## Moderate Changes

- **Add capabilities and custom actions to a declarative agent created with Microsoft 365 Agents Toolkit**
  Updated terminology and headings from “skills” to “capabilities and custom actions,” aligning with MCP/API plugin concepts. Improves clarity on how to enhance agents using built-in capabilities or custom actions so authors follow consistent guidance across the platform.
  https://learn.microsoft.com/en-us/microsoft-365/copilot/extensibility/build-declarative-agents-add-capabilities

- **Show citations with response semantics**
  Relaxed guidance for clickable citations in plugin responses: links are now optional, and citations can be included without URLs. This change removes the prior policy coupling and gives plugin authors more flexibility while still enabling attribution where appropriate.
  https://learn.microsoft.com/en-us/microsoft-365/copilot/extensibility/plugin-citations