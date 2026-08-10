# Microsoft 365 Copilot Extensibility
**Date created:** 2026-07-22 UTC  
**Tags:** Agent  

## New Articles

- **Declarative agent schema 1.8 for Microsoft 365 Copilot**

  Introduces declarative agent schema v1.8 with new write-capabilities EmailActions and MeetingActions, and clarifies separation between Email (read/search) and EmailActions (write) scopes. Expands coverage and examples across key capabilities such as WebSearch, OneDrive and SharePoint, Copilot connectors with fine-grained filters, GraphicArt, CodeInterpreter, Dataverse, TeamsMessages, People (with optional related content), and Meetings. Adds behavior_overrides—including default_response_mode (Auto, Quick response, Think deeper)—plus controls for suggestions and special instructions. Documents conversation starters with capability dependencies, referenced or inline plugin actions, editorial answers with similarity thresholds, user_overrides for capability toggles, worker agents (preview), and placeholders for embedded knowledge and sensitivity labels.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/extensibility/declarative-agent-manifest-1.8

## Moderate Changes

- **What's new in Microsoft 365 Copilot extensibility**

  Added a schema 1.8 section detailing new EmailActions and MeetingActions, a new file property for worker agents, and an embedded_resource_snapshot_id for embedded knowledge. These updates enable write operations for email and meeting workflows and improve file referencing and knowledge management, helping builders adopt v1.8 more effectively.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/extensibility/whats-new