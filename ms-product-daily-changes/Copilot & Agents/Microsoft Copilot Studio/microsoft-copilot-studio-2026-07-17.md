# Microsoft Copilot Studio
**Date created:** 2026-07-17 UTC  
**Tags:** Administration, AI, Analytics, Agent, Automation, Governance, Monitoring, Programming, Security  

## New Articles

- **Troubleshoot agent conversations with Agent Debugger in Copilot Agent Kit**

  Introduced Agent Debugger to analyze conversations from Dataverse transcripts or Copilot Studio snapshot ZIPs. The guide explains metrics, execution path, performance timelines, recommendations with severities, and a full JSON/debug view per step. It includes permissions, setup, and extensive troubleshooting to speed diagnosis of slow steps, errors, and missing traces.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/guidance/kit-agent-debugger

- **Monitor agent performance with Agent Insights Hub in Copilot Agent Kit**

  Added Agent Insights Hub for end-to-end monitoring using Application Insights, conversation transcripts, and usage history. The article covers setup, data aggregation into Dataverse, and rich dashboards across metrics, topics, tools, errors, transcripts, and sync logs. It also introduces a preview for custom dashboards and forecasting, plus a troubleshooting guide to validate data flows.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/guidance/kit-agent-insights-hub

- **Accelerate agent development with Agent Library in Copilot Agent Kit**

  Introduced Agent Library as a centralized place to discover and install prebuilt agent templates and reusable components. It outlines availability, roles, and how makers and admins browse templates and component collections. Clear links guide readers to related setup and management topics.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/guidance/kit-agent-library

- **Best practices for working in Agent Library in Copilot Agent Kit**

  Added guidance to start from templates, tailor topics, and test with realistic scenarios. It recommends disciplined component use, managed solutions, and connection health management. Environment practices and custom template lifecycle tips help teams standardize and safely evolve solutions.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/guidance/kit-agent-library-best-practices

- **Components management in Agent Library in Copilot Agent Kit**

  Documented how to discover, install, and manage reusable component collections, including dependencies and connection setup. The reference lists notable components like Document Extraction, Content Synthesizer, Research, Executive Brief, Log Chain of Thoughts, Save Conversation History, and ServiceNow Ticket Assistant. It explains installation paths, permissions, and how to wire components into agents via instructions and connection references.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/guidance/kit-agent-library-components

- **Custom agent templates in Agent Library in Copilot Agent Kit**

  Explained how to install and configure custom agent templates packaged as Power Platform solutions. The guide covers connection reference readiness and remediation, in-product installation flow, and manual import via Power Apps. Post-install steps help makers quickly customize and launch agents.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/guidance/kit-agent-library-custom-agent-templates

- **Custom templates in Agent Library in Copilot Agent Kit**

  Added admin-focused instructions to create, publish, and manage custom templates stored in Dataverse. It details required roles, publish statuses that govern maker visibility, and template metadata including ZIP uploads and helpful URLs. Deletion behavior and drafting practices ensure safe lifecycle management.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/guidance/kit-agent-library-custom-templates

- **Declarative agent templates in Agent Library in Copilot Agent Kit**

  Introduced workflows for Microsoft 365 declarative agent templates with options to customize and download, use Agent Builder, or build with VS Code and the Microsoft 365 Agents Toolkit. Step-by-step guidance covers editing instructions, capabilities, and prompts, plus packaging and Teams upload. Best practices emphasize high-quality instructions for reliable outcomes.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/guidance/kit-agent-library-declarative-agent-templates

- **End-to-end usage of Agent Library in Copilot Agent Kit**

  Provided a complete workflow to discover templates, install or import them, and configure agents with instructions, knowledge, triggers, and auth. It shows how to extend agents using component collections and validates functionality through testing. The article concludes with publishing across channels.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/guidance/kit-agent-library-end-to-end-usage

- **Templates overview in Agent Library in Copilot Agent Kit**

  Added an overview of prebuilt and custom templates, covering Copilot Studio and Microsoft 365 categories. A catalog lists available templates and their purposes to help teams pick proven starting points. This accelerates solution selection and reduces initial design time.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/guidance/kit-agent-library-templates-overview

- **Use the Agent Review Pipeline as a CI/CD gate**

  Introduced an automated CI/CD quality gate that evaluates agents with deterministic checks and AI-based scoring. The guide walks through setup using Power Platform Pipelines and GitHub Actions, including Entra app registration, secrets, roles, and managed solution import. It covers running tests, retrieving score reports, customizing thresholds and patterns, and building from-scratch webhook flows with robust troubleshooting.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/guidance/kit-agent-review-pipeline

- **Component reference in Agent Library in Copilot Agent Kit**

  Published a detailed reference for reusable component collections, including inputs/outputs, interaction models, and flow steps. It explains synthesis and research pipelines, executive brief generation, and ServiceNow incident operations with required connections and Entra setup. Guidance covers managed vs. unmanaged management and customization considerations.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/guidance/kit-component-library-reference

- **Govern connector access with Power Shield in Copilot Agent Kit**

  Introduced Power Shield to govern connector access via approval-driven data policies. The article explains architecture, roles, connection references, and automated sync of connectors and actions. It details maker requests, admin review and approvals, policy updates, lifecycle statuses, settings hubs, and troubleshooting to strengthen governance at scale.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/guidance/kit-power-shield

## Major Changes

- **Analyze agents using Agent Review Tool in Copilot Agent Kit**

  Rebranded the solution from Copilot Studio Kit to Copilot Agent Kit and expanded coverage to include Microsoft 365 Declarative Agents. The content adds an end-to-end review workflow, anti-pattern checks with severity, instruction-quality scoring, and comprehensive results with exports (PDF, SARIF, Excel). This upgrade provides a deeper, AI-assisted evaluation to improve quality, compliance, and reliability.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/guidance/kit-agent-review-tool

- **Configure tests in Copilot Agent Kit**

  Updated branding to Copilot Agent Kit and added guidance for testing agents that require connector authorization. The new multi-turn test pattern demonstrates capturing and asserting authorization cards and invoking actions to proceed, after which tests can run as single-turn. Clarifications improve consistency across test types and validation terminology, strengthening automated test reliability.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/guidance/kit-configure-tests

- **Configure users and teams in Copilot Agent Kit**

  Replaced legacy roles with new CSK - Administrator and CSK - Maker roles and marked prior roles as deprecated, with migration guidance. A comparison table clarifies access across key kit features, and step-by-step instructions show how to assign roles via Entra ID and individual users. Additional notes on column security and Dataverse references help admins set secure, least-privilege access.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/guidance/kit-configure-users-teams

- **Copilot Agent Kit overview**

  Rebranded the offering and refreshed capability descriptions to reflect new experiences like Agent Insights Hub, Agent Debugger, Agent Library, and Power Shield. The page clarifies tests, rubrics, compliance, inventory, KPIs, and tooling across the kit, with streamlined descriptions and updated next steps. Readers gain a clearer map of capabilities and where to go for deeper guidance.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/guidance/kit-overview

- **Copilot Agent Kit prerequisites**

  Updated branding and expanded prerequisites with a detailed connector requirements table and usage guidance. The improvements clarify which connectors are needed for specific features and highlight data policy considerations. Teams can now plan environment readiness more precisely and avoid setup blockers.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/guidance/kit-prerequisites

- **Set up Copilot Agent Kit by using the Setup Wizard**

  Rebranded the page and added tables that document connection references and environment variables with purposes and defaults. Instructions clarify prerequisites, flow activation, and data integrations like SharePoint sync and Application Insights. This detail helps admins configure environments consistently and avoid misconfiguration.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/guidance/kit-setup-wizard

## Moderate Changes

- **Use the Power Platform API to quarantine agents**

  Clarified quarantine behavior: makers can interact with quarantined agents during testing, while all other channels remain blocked. This change enables safe validation before re-enabling production access.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/admin-api-quarantine

- **What's new in Copilot Studio**

  Added updates including Windows 365 for Agents MCP server GA, condition groups for authoring, and previews for Teams Phone voice agents, agent delegation, and Foundry IQ grounding. Also noted GA availability to select Claude Sonnet 5 or GPT-5.5 Chat as the primary model, expanding choice for performance and cost alignment.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/whats-new