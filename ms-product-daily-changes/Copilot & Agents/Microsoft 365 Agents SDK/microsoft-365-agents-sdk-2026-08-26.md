# Microsoft 365 Agents SDK
**Date created:** 2026-08-26 UTC  
**Tags:** Automation, Configuration, Deprecation, Get Started, Guidance, Identity, Security, Troubleshooting  

## New Articles

- **Use adaptive cards in agents**

  Introduced guidance for designing and sending Adaptive Cards from .NET and JavaScript agents, including creating attachments and using CardFactory. Explained routing for Action.Execute and action submit handlers across attribute and fluent APIs, plus dynamic search via SearchRoute/app.adaptiveCards.search. Clarified OAuth requirements for card routes in .NET, JavaScript auth considerations, and channel-specific behaviors with Teams references.

  https://learn.microsoft.com/en-us/microsoft-365/agents-sdk/adaptive-cards

- **Provision Azure resources with an Agents SDK plugin**

  Introduced an Agents SDK provisioning plugin for GitHub Copilot CLI and Claude Code to streamline setup. Covered prerequisites, installation, and automated steps to create Azure Bot and identity resources, choose authentication (managed identity, federated credentials, or client secret), add the Teams channel, enable OAuth/Teams SSO, and generate connection configuration. Emphasized secure secret storage and offered a path to manual provisioning if preferred.

  https://learn.microsoft.com/en-us/microsoft-365/agents-sdk/provision-with-agent-plugin

- **Handle Microsoft Teams lifecycle events**

  Added end-to-end guidance for handling Teams lifecycle events across .NET, Node.js, and Python using the Teams extension. Documented channel and team event handlers and available .NET route attributes, with code examples for common scenarios. Included patterns to retrieve team and channel details through the Teams API client and links to related topics.

  https://learn.microsoft.com/en-us/microsoft-365/agents-sdk/teams/teams-configuration-lifecycle

- **Access Microsoft Teams conversation members**

  Added how-to guidance for retrieving conversation members using the Teams API client from the Teams extension. Demonstrated fetching single members, listing and paging, and querying a team roster with samples in .NET, Node.js, and Python. Clarified client access from turn context and availability on the Teams channel.

  https://learn.microsoft.com/en-us/microsoft-365/agents-sdk/teams/teams-context

- **Use AI citations and collect feedback in Microsoft Teams**

  Introduced AI citation support that converts source markers to numbered references with metadata in streaming responses. Added patterns to enable and process user feedback (thumbs up/down) and handle message reactions via Teams handlers, with language-specific examples. Noted current Python limitations for typed routes and linked to related Teams guidance.

  https://learn.microsoft.com/en-us/microsoft-365/agents-sdk/teams/teams-feedback

- **Handle files and file consent in Microsoft Teams**

  Explained how agents receive and securely download file attachments, including .NET setup with attachment downloaders and Node.js/Python approaches using content URLs. Documented the file consent flow for uploading to a user’s OneDrive in personal chats, manifest requirements, and limitations for channels and group chats. Provided accept/decline handler samples and guidance to upload via the consent URL or Microsoft Graph.

  https://learn.microsoft.com/en-us/microsoft-365/agents-sdk/teams/teams-files

- **Handle Microsoft Teams meeting events**

  Added guidance for registering handlers for meeting start/end and participant join/leave with typed data. Called out required RSC permission (OnlineMeeting.ReadBasic.Chat) and provided code samples in .NET, Node.js, and Python. Included examples for retrieving meeting and participant details using the Teams API client.

  https://learn.microsoft.com/en-us/microsoft-365/agents-sdk/teams/teams-meetings

- **Use message extensions in Microsoft Teams**

  Provided end-to-end guidance for building compose extensions, including query/select item handlers, action commands that return Adaptive Cards, and link unfurling (including zero‑install). Covered message preview edit/send flows and settings page configuration with handlers. Included .NET, Node.js, and Python samples with Adaptive Card payload examples and related links.

  https://learn.microsoft.com/en-us/microsoft-365/agents-sdk/teams/teams-message-extensions

- **Handle messages in Microsoft Teams**

  Documented targeted (private) messages, expiration, and privacy considerations, with language-specific samples. Clarified Prompt Preview behavior for targeted messages, sending public vs. private responses, and proactive scenarios, plus quoted reply APIs and when to use them. Included slash command setup details and guidance on message formatting and suggested actions.

  https://learn.microsoft.com/en-us/microsoft-365/agents-sdk/teams/teams-messages

- **Use task modules in Microsoft Teams**

  Explained how to show Adaptive Cards or web pages in modal dialogs and map routes from card data. Demonstrated fetch and submit flows, response types (continue vs. message), and dialog chaining with .NET, Node.js, and Python samples. Provided reusable patterns for building rich interactive experiences.

  https://learn.microsoft.com/en-us/microsoft-365/agents-sdk/teams/teams-task-modules

- **Test a local agent with a dev tunnel**

  Added a step-by-step guide to expose a locally running agent via a secure dev tunnel and connect it to Azure Bot Service for channel testing. Covered prerequisites, creating and hosting the tunnel, configuring the bot messaging endpoint, and validating message flow. Included diagnostics tips, credential guidance for local testing, options for persistent tunnels, and security considerations.

  https://learn.microsoft.com/en-us/microsoft-365/agents-sdk/test-with-dev-tunnel

## Major Changes

- **Teams extension for the Agents SDK**

  Restructured the article into a concise overview that links to feature-specific pages for easier navigation and maintenance. Introduced migration guidance away from TeamsActivityHandler-based bots to AgentApplication with Teams routes to align with current SDK patterns. Renamed the source-generated property from TeamsExtension to Teams and updated related fluent APIs, and changed meeting handler payloads to Microsoft.Teams.Apps.Clients.MeetingDetails. Streamlined the exposed properties list and expanded related content to Adaptive Cards, app manifest schema, and device capabilities.

  https://learn.microsoft.com/en-us/microsoft-365/agents-sdk/teams/teams-extension

## Moderate Changes

- **Integrate with Copilot Studio**

  Clarified current client library support for agents built with the standard harness and noted that the GitHub Copilot harness is not yet officially supported. Added related guidance to help connect a Copilot Studio agent with the Microsoft 365 Agents SDK for a clearer integration path.

  https://learn.microsoft.com/en-us/microsoft-365/agents-sdk/integrate-with-mcs

- **Provision Azure resources for your agent manually**

  Reorganized the flow to focus on provisioning Azure Bot and identity resources first, then configuring the agent connection before testing or deploying. Refined authentication guidance (managed identity, federated credentials, and client secret), added steps for provisioning storage and dependencies, and consolidated next steps with a single connection configuration guide and dev tunnel testing.

  https://learn.microsoft.com/en-us/microsoft-365/agents-sdk/provision-azure-bot-service-manually