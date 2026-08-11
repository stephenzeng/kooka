# Microsoft Copilot Studio
**Date created:** 2026-08-04 UTC  
**Tags:** Administration, Agent, AI, Analytics, Automation, Governance, Monitoring  

## New Articles

- **Agents overview**

  Introduces Copilot Studio agents and where they can be deployed, with clear guidance on integrations and extensibility. Explains the three harness options—GitHub Copilot, standard, and Copilot chat—and when to use each. Highlights capabilities such as tool orchestration, file reasoning, conversational memory, and cross‑channel publishing.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/agents-overview

- **Overview of usage-based billing**

  Introduces usage-based billing for agents, workflows, and apps powered by the GitHub Copilot harness. Details what usage covers (LLM tokens, tools, and harness runtime), when billing starts, and where to monitor consumption. Explains how to purchase and manage Copilot credits and references enforcement behavior when credits are depleted.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/agents-experience/billing-credit-overview

- **Purchase and manage Copilot credits**

  Describes two ways to obtain credits: pay‑as‑you‑go via an Azure subscription or a one‑year prepaid plan using Copilot Credit Commit Units. Covers environment linking with billing policies, metering, and where to manage credits in the Power Platform admin center. Helps admins choose and operationalize the right purchase model for their organization.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/agents-experience/billing-manage-buy-credits

- **Build a new agent**

  Provides step‑by‑step guidance to create an agent powered by the GitHub Copilot harness, including naming, instructions, and saving. Clarifies that the last name before first save becomes the schema name, which is then read‑only. Explains next steps after save (Share, Preview, Evaluate) and how to adjust language, solution, and schema settings.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/agents-experience/build-new-agent

- **Enforcement policy**

  Explains what happens when Copilot credits are not available: end users won’t get responses and maker authoring and evaluation features are blocked. Outlines the notification shown to users and grace/overage behavior. Provides remediation options including reallocating or purchasing capacity or configuring pay‑as‑you‑go.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/agents-experience/enforcement-policy-credits

- **Connect to Fabric IQ from an agent (preview)**

  Introduces how to connect Fabric IQ as a tool through the Build > Add tool flow in the new experience. Covers prerequisites, selection, and removal of the connection, noting that only accessible items appear in the picker. Clarifies that removing the link in Copilot Studio does not modify underlying Microsoft Fabric assets.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/agents-experience/fabric-iq-connect

- **Choose a harness**

  Explains what a harness is and how to select among GitHub Copilot, standard, and Copilot chat harnesses based on reasoning needs, predictability, and billing. Details capabilities such as multi‑step reasoning, tool orchestration, file operations, memory, and publishing options. Provides comparison guidance and links to related topics like licensing and usage‑based billing.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/harnesses-overview

## Major Changes

- **Monitor an agent overview**

  General availability update with removal of preview status and significant expansion of analytics. Added new areas including AI‑generated Summary insights, Cost and billing with Copilot Credit consumption and savings, Reactions, and Agent capabilities. Improved guidance on filters, error monitoring, and transcript downloads via Dataverse and the app.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/agents-experience/analytics-overview

- **Start building**

  Refocused from a detailed creation walkthrough to a consolidated “Start building” guide from the homepage. Surfaces build choices for agents and workflows powered by the GitHub Copilot harness and entry points to standard harness options. Introduces natural language agent creation (preview) with visuals and removes redundant step‑by‑step content.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/agents-experience/authoring-first-bot

- **Monitor and analyze an agent (preview)**

  Expanded scope from monitoring to comprehensive analytics with new Overview KPIs, extended time filtering, and detailed active user metrics. Added Billings and Savings panels with Copilot Credit trends and calculators, plus a Reactions section and tool‑use analytics. Updated notes, callouts, and related links while deprecating older sections.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/agents-experience/authoring-review-activity

- **Overview**

  Rewrote the product overview to position Copilot Studio as a low‑code studio for AI‑powered agents and workflows. Introduces harness choices, natural language authoring (preview), and end‑to‑end manage/operate topics including analytics, evaluations, and administration. Updates access, browser support, and billing references while retiring legacy guidance.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/fundamentals-what-is-copilot-studio

- **Build**

  Reframed content to focus on agents powered by the GitHub Copilot harness and to contrast with the standard harness. Updated concepts across authoring, lifecycle, orchestration, and availability; removed preview toggles and legacy links. Clarified knowledge behavior by removing Microsoft IQ references.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/agents-experience/overview

## Moderate Changes

- **Add a connected agent to an agent**

  Removed preview status and updated terminology to GitHub Copilot harness. Adjusted prerequisites and descriptions to reflect the harness without changing procedures.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/agents-experience/add-agent-connected

- **Add a tool to an agent**

  Removed preview labels and aligned terminology and prerequisites to the GitHub Copilot harness. Clarifies that tool support applies to GitHub Copilot–powered agents; no procedural changes.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/agents-experience/add-tools-custom-agent

- **Create a test set for an agent (preview)**

  Updated prerequisites and wording for GitHub Copilot–powered agents and replaced banners with a production‑ready preview note. Clarified evaluation setup steps including CSV import, AI conversation generation options, and manual test authoring.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/agents-experience/analytics-agent-evaluation-create

- **Run an evaluation for an agent (preview)**

  Scoped content to GitHub Copilot–powered agents and replaced experience banners with a preview note. Included minor rephrasing and UI label clarifications for consistency.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/agents-experience/analytics-agent-evaluation-results

- **Use the activity trace to debug your agent**

  Removed preview status and aligned the scope and prerequisites to the GitHub Copilot harness. Language and framing were updated without changing the debug workflow.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/agents-experience/authoring-activity-trace

- **Configure agent details and instructions**

  Reoriented guidance to emphasize instructions as the primary control for GitHub Copilot–powered agents and contrasted with the standard harness. Removed preview references and updated terminology across the page.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/agents-experience/authoring-instructions

- **Select a model for an agent**

  Removed preview designation and clarified that agents use the GitHub Copilot harness. Core guidance remains unchanged.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/agents-experience/authoring-select-agent-model

- **Share agents with other makers and groups**

  Removed preview status and updated sharing guidance to reference using the GitHub Copilot harness for editing. No other changes to sharing steps.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/agents-experience/authoring-share-agent

- **Test an agent**

  Promoted to general availability and aligned terminology and prerequisites to the GitHub Copilot harness. Testing guidance and structure are unchanged.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/agents-experience/authoring-test-bot

- **Standard harness licensing**

  Retargeted licensing content to apply specifically to standard harness agents and added a classic experience banner. Retains the Copilot Studio Licensing Guide.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/billing-licensing

- **Build an agent**

  Removed preview status and repositioned the article to focus on GitHub Copilot harness agents. Eliminated Microsoft IQ references and clarified that Build configures model, instructions, tools, and knowledge; updated comparisons to “standard harness vs. GitHub Copilot harness.”

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/agents-experience/build-overview

- **Quickstart: Create an automated solution with natural language in the GitHub Copilot harness (preview)**

  Retargeted the quickstart to the GitHub Copilot harness with updated steps, notes, and screenshots. Added a production‑ready preview notice and clarified model availability and compatibility.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/create-automation-natural-language

- **Workflows overview**

  Removed preview status and clarified that workflows run on the GitHub Copilot harness, updating getting‑started guidance. Also clarified how agent flows behave when initiated from the GitHub Copilot harness by opening standard harness authoring in a new tab.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/workflows-experience/flows-overview

- **Connect to Foundry IQ from an agent**

  Updated to the new Tools model and GitHub Copilot harness prerequisites. Clarified connection flow, UI labels, and removal steps using the Tools panel.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/agents-experience/foundry-iq-connect

- **Add knowledge sources to an agent**

  Refocused on GitHub Copilot harness with updated source list and removal of Microsoft/Work IQ references. Clarified differences from the standard harness, including behavior for general knowledge and file uploads.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/agents-experience/knowledge-add-existing-copilot

- **Knowledge overview for agents**

  Removed preview status and oriented content to GitHub Copilot harness configuration. Eliminated the “Knowledge vs. Microsoft IQ” comparison and related link.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/agents-experience/knowledge-copilot-studio

- **Manage connected agents in an agent**

  Removed preview labels and specified applicability to the GitHub Copilot harness. Procedures remain the same.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/agents-experience/manage-connected-agents

- **Memory (preview)**

  Expanded guidance on Memory behavior, privacy, and controls, noting per‑user storage and maker enablement per agent. Documented lifecycle, retention, chat and portal management, and limitations such as group chat behavior.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/agents-experience/memory-overview

- **Extend Microsoft 365 Copilot with the Copilot chat harness**

  Retitled to emphasize the Copilot chat harness and added a note on harness‑specific billing/licensing. Clarifies positioning of features within the harness model.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/microsoft-365-copilot-extend-with-agents

- **Manage preview conversations**

  Removed preview designation and aligned the context and prerequisites to the GitHub Copilot harness. Clarifies that the Preview tab applies to GitHub Copilot–powered agents.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/agents-experience/preview-history

- **Preview and test an agent**

  Promoted to GA by removing preview markers and aligning with the GitHub Copilot harness. No changes to the testing flow.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/agents-experience/preview-overview

- **Add a prompt node to an agent flow**

  Clarified availability: the prompt node isn’t available in GitHub Copilot harness workflows and remains in standard harness agent flows. Points to using an Agent action to achieve similar outcomes.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/prompt-node-workflow

- **Available channels for agents**

  Removed preview status and clarified scope for GitHub Copilot harness agents. Channel guidance remains intact.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/agents-experience/publication-channels-overview

- **Publish overview for agents**

  Oriented publishing guidance to GitHub Copilot harness agents and removed Microsoft IQ from the pre‑publish checklist. Reflects the updated publish capture details.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/agents-experience/publication-fundamentals-publish-channels

- **Quotas and limits**

  Re‑scoped content to standard harness agents with updated title and description. Adjusts introduction to reflect the narrower focus.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/requirements-quotas

- **Manage sessions and capacity for the legacy Power Virtual Agents license**

  Clarified that sessions management guidance applies to the legacy Power Virtual Agents license. Updates title and description for precision.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/requirements-sessions-management

- **Settings**

  Updated description to state settings apply to GitHub Copilot harness agents. No other changes.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/agents-experience/settings-overview

- **Add an existing skill to an agent**

  Updated prerequisites to require a GitHub Copilot harness agent; removed preview markers. No procedural changes.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/agents-experience/skills-add-existing

- **Create a skill for an agent**

  Removed preview status and aligned prerequisites and description to GitHub Copilot harness agents. Core steps remain the same.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/agents-experience/skills-create

- **Access standard harness agents and agent flows**

  Reframed from experience switching to harness selection, adding concrete steps to build and access standard harness agents/flows. Includes navigation via homepage toggle, “Other ways to build,” and Agents/Workflows lists.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/agents-experience/switch-experiences

- **Available tools for agents**

  Removed preview markers and clarified applicability to GitHub Copilot harness agents. No changes to tool type descriptions.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/agents-experience/tools-available

- **Manage and delete tools in an agent**

  Removed preview status and updated description for GitHub Copilot harness agents. Procedures are unchanged.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/agents-experience/tools-manage

- **Tools overview for agents**

  Removed preview markers and aligned terminology to GitHub Copilot harness orchestration and tool invocation behavior. Simplifies language by removing “new experience” references.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/agents-experience/tools-overview

- **Error codes reference for agents**

  Removed preview labels and clarified that error codes pertain to GitHub Copilot harness agents, including where they appear. No changes to the codes themselves.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/agents-experience/troubleshooting-error-codes

- **Upgrade to Copilot Studio unified authoring**

  Rewrote to focus on cloning classic Power Virtual Agents chatbots into standard harness agents. Clarifies migration eligibility, cloning workflow, configuration considerations, and recommended testing.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/unified-authoring-conversion

- **What's new in Copilot Studio**

  Updated the June 2026 note to explain that the GitHub Copilot harness powers enhanced orchestration for better response quality and reasoning. Confirms availability alongside the classic experience.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/whats-new