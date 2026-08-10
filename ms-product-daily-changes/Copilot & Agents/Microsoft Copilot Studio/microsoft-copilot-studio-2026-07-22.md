# Microsoft Copilot Studio
**Date created:** 2026-07-22 UTC  
**Tags:** Administration, AI, Agent, Automation, Monitoring  

## New Articles

- **Monitor real-time voice agents by using Application Insights**

  Introduced a comprehensive how-to for wiring Copilot Studio real-time voice agents to Azure Application Insights and interpreting telemetry. Documents event taxonomy (CallLifecycle, DialogLifecycle, SpeechPipeline, LlmInvocation, ToolExecution), key fields in traces/customDimensions, and correlation practices. Provides Kusto queries for conversation reconstruction, timing analysis, LLM latency, and tool execution outcomes, and clarifies latency measurement (TTFAB) across multi-step turns. Includes best practices for ongoing monitoring and notes current limitations such as lack of per-utterance timing and partial separation of external call time.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/voice-realtime-monitor-application-insights

## Major Changes

- **Allow file input from users**

  Expanded guidance on enabling and handling file uploads across supported channels (e.g., Teams, website via Direct Line/web chat, Facebook, Omnichannel for Customer Service, Microsoft 365 Copilot, and Test panel) and clarifies unsupported channels. Clarifies how Word files are parsed, with caveats for text in shapes, headers/footers, and embedded objects, plus best-practice tips. Details character limits without code interpreter and how enabling the interpreter removes limits for supported structured data, with recommendations for splitting large files. Adds advice for multi-file uploads within a conversation, including managing context limits, and explains behavior for encrypted or password-protected files and when to use Microsoft 365 Copilot Chat.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/image-input-analysis

- **Share your prompt**

  Introduces explicit sharing levels: User (run/use) and Co-owner (edit, share, delete) for prompts, with an updated Share permissions section. Updates the Share action flow and list views, and clarifies that sharing as Co-owner allows recipients to edit prompts—replacing prior guidance. Removes an outdated Important note about model versions, regional availability, and potential usage limits.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/share-your-prompt

## Moderate Changes

- **Add an agent node to a workflow (preview)**

  Added guidance for extracting data from Outlook email attachments and SharePoint files using the agent node within workflows. Covers using the Outlook trigger and SharePoint file content node, passing files to the agent node, and applying extracted data in downstream steps, with illustrative examples.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/workflows-experience/agent-node-workflow

- **Add a public website as a knowledge source**

  Updated step-by-step instructions and UI walkthrough for adding public websites, including variable picker usage and optional field edits, with new screenshots. Introduced a Search query length section explaining the 2,048-character limit for Bing grounding, factors that can trigger it, and tips to keep questions concise.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/knowledge-add-public-website

- **Knowledge sources summary**

  Added guidance on why agents may not return grounded answers when ungrounded responses are disabled, emphasizing citation requirements. Provides best practices to improve citation consistency and notes channel-specific citation behaviors, including Teams limits and manual rendering needs for customized responses.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/knowledge-copilot-studio

- **Add a generative answers node**

  Documented the “Search only selected sources” option, including default behavior, explicit source selection, and no fallback to agent-level sources. Includes instructions to answer solely from custom data by enabling the option with no selections and configuring a data variable, plus clarifications on trigger conditions.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/nlu-boost-node

- **Fix Copilot Studio Usage Limits and Agent Unavailable Errors**

  Added guidance to proactively plan agent deployments for throughput and rate limits across Copilot Studio, Power Automate, Dataverse, connectors, and downstream APIs. Recommends capacity planning before UAT/production, estimating peaks, optimizing designs, and reviewing limits prior to requesting increases, with a link to detailed planning guidance.

  https://learn.microsoft.com/en-us/troubleshoot/power-platform/copilot-studio/licensing/throttling-errors-agents

- **What's new in the Copilot Studio guidance hub**

  Added a July 2026 update highlighting new Copilot Agent Kit capabilities (Agent Debugger, Library, Insights Hub, Power Shield, Review Pipeline) and the initial rename phase from Copilot Studio Kit to Copilot Agent Kit. Notes significant updates to the Agent Review Tool to reflect expanded scope.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/guidance/whats-new