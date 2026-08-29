# Microsoft Copilot Studio
**Date created:** 2026-08-29 UTC  
**Tags:** Analytics, Best Practices, Compliance, Configuration, Governance, Guidance, Security, Troubleshooting  

## New Articles

- **Context distribution in the standard harness**

  New guidance explains how the standard harness shares and interprets context across components, and how this differs from the GitHub Copilot harness. It details explicit inputs/outputs and implicit context flows, including what each component can see and return. The article outlines principles to avoid missed or duplicated answers, highlights caveats for topics and subagents, and provides next steps with related references.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/guidance/generative-orchestration-context-design

- **Design best practices to avoid duplicate messages**

  Introduces a design approach to prevent duplicate or missed responses by aligning user-visible output with orchestration context. It recommends that components return clear outputs (for example, answered-state and displayed values), provide precise descriptions of completion criteria, and use a top-level instruction that checks outputs before responding. The guidance covers topics, knowledge calls, generative answers, and subagents, and includes strategies to persist and restore context in long conversations.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/guidance/generative-orchestration-duplicate-messages

- **Troubleshoot duplicate messages and missed answers**

  Provides a troubleshooting playbook for duplicate answers, missing parts of responses, regressions, and double execution in standard harness agents. It maps observable symptoms to root causes and targeted fixes, such as ensuring components report answered-state, establishing a single response owner, scoping child/connected agents, and rehydrating context for long sessions. The guide details evidence to collect, investigation steps (including activity maps), and corrective patterns for prompts, redirects, and interception.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/guidance/generative-orchestration-duplicate-messages-troubleshoot

- **Design subagents that avoid duplicate messages**

  Best-practice guidance for child and connected subagents to prevent duplicate messaging. It recommends disabling parent context for connected agents, scoping work with a dedicated input, and defining a clear input/output contract (for example, answered, interactionSummary, findings, openQuestions). The article includes reusable top-level instructions, delegation patterns (silent vs. speaking subagents), example prompts, and links to related orchestration guidance.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/guidance/generative-orchestration-subagents

- **Design topics as mini-agents that avoid duplicate messages**

  Guidance to design topics as mini-agents that return outputs instead of messaging users directly. It covers naming and descriptions for orchestration, collecting required inputs with robust prompts and validation, keeping deterministic logic inside the topic, and using tested output patterns (such as answered and messageSummary). The article includes a sample top-level instruction to check outputs before replying and an example preventing re-asking after Adaptive Card selections.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/guidance/generative-orchestration-topics

## Moderate Changes

- **Connect to a Microsoft Foundry agent (preview)**

  Added a preview banner and new prerequisites requiring the Activity protocol endpoint to be enabled (via REST API or Python SDK) to prevent runtime HTTP 400 failures. The update clarifies connection steps and adds troubleshooting to detect and resolve unsupported endpoints.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/add-agent-foundry-agent

- **Control how transcripts are retained and accessed**

  Clarified that session information is temporarily stored in Copilot Studio storage for up to 28 days and auto-deleted, with guidance to file a support ticket if transcript viewing/downloading is disabled. The article refines where transcripts are not written (for example, Dataverse for Teams and Microsoft 365 Copilot agents) and emphasizes controlling retention in Dataverse.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/admin-transcript-controls

- **Orchestrate agent behavior with generative AI**

  Expanded guidance recommends returning topic responses as outputs and including an answered-state to prevent duplicate replies from the orchestrator. It notes some behaviors depend on the selected model and advises testing with your configured model; it also clarifies how overlapping topic descriptions can make selection unpredictable.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/advanced-generative-actions

- **Understand downloaded conversation transcripts from Power Apps**

  Updated retention to 28 days in Copilot Studio storage with automatic deletion and guidance to open a support ticket if access is disabled. Clarified SharePoint knowledge behavior (responses not included; questions and source content included with answers redacted) and refined environment exclusions by removing Dataverse developer environments.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/analytics-transcripts-powerapps

- **Understand downloaded session data from Copilot Studio**

  Refined transcript retention to 28 days with automatic deletion and added guidance to review activities in Power Apps or adjust Dataverse retention. Included steps for obtaining data when access is disabled, clarified SharePoint redaction behavior, updated environment exclusions, and noted that recording/downloading is enabled by default in new environments.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/analytics-transcripts-studio

- **Apply generative orchestration capabilities**

  Aligned terminology and descriptions with the standard harness, replacing “orchestrator” references and updating architecture, control layers, authoring, chaining, testing, and triggers accordingly. Added notes on accessing standard agents and flows, plus a new related article link on managing context.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/guidance/generative-orchestration

- **Set up Copilot Agent Kit by using the Setup Wizard**

  Reworked environment variables into a detailed core table with a “Where used” column and expanded guidance. Introduced two new core variables and a feature-specific section covering Compliance Hub variables and per-agent secrets via Azure Key Vault, clarifying that the wizard focuses on core settings.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/guidance/kit-setup-wizard