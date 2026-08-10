# Microsoft Copilot Studio
**Date created:** 2026-07-19 UTC  
**Tags:** Administration, AI, Agent, Governance  

## Major Changes

- **Overview of real-time agent design optimization**
  Expanded guidance from voice-only to all real-time agents, removing preview labels and updating the title and descriptions. Language and sections were generalized beyond voice scenarios while keeping speech handling as an optional, secondary design decision. Section naming and examples were adjusted to apply broadly across channels, improving relevance for both voice and text experiences.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/guidance/voice-agents-optimize-voice

- **Configure real-time agents**
  Reworked the article for multi-channel use, adding digital messaging support (preview) alongside voice. Setup now centers on selecting a single real-time model used across channels and clarifies channel-specific capabilities (for example, SSML and DTMF for voice; Adaptive Cards and Quick Replies for digital messaging in preview). Trigger behavior and context variables were split by channel, and guidance was added on variable passing and descriptions. New channel-specific settings detail voice options (voice selection, VAD, DTMF, silence detection) and digital messaging behaviors (text-only, inactivity handling). Evaluation guidance was updated to note text-only support during evaluation.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/voice-realtime-configure

- **Customize your real-time agent**
  Broadened scope from voice to cross-channel, adding a preview note for digital messaging. Introduced a simplified, channel-aware sample instructions JSON template and streamlined guidance on topic and tool descriptions. Examples and best practices were updated to distinguish voice-specific versus digital messaging scenarios, helping teams design clearly across channels.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/voice-realtime-customize

- **Publish real-time agents**
  Expanded deployment guidance from voice-only to multichannel, with steps for connecting to both voice and digital messaging channels (digital messaging in preview). Consolidated instructions under “Deploy to channels” and added a new multichannel deployment section covering shared configuration and channel-specific features (DTMF, VAD, and voice selection apply only to voice). Clarified that voice workstream profile settings don’t apply to real-time agents and listed supported voices. Added tips to review and align channel-aware instructions before going live.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/voice-realtime-publish

- **Test your real-time agent**
  Generalized testing to cover both voice and digital messaging channels with distinct modes (Speech & DTMF for voice, Text for digital messaging in preview). The test workflow was restructured with tabbed guidance per channel, clarified authentication for voice testing, and refined microphone permission steps. Limitations were separated by channel, highlighting environment differences, audio-path impacts, and considerations for barge-in, VAD, and rendering behaviors.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/voice-realtime-test

- **Real-time agents overview**
  Elevated the article from voice-only to multi-channel, adding digital messaging support (preview) and clarifying voice-native capabilities like PSTN/SIP, DTMF, barge-in, and VAD. Prerequisites now include digital messaging roles and workstreams, and regional notes were updated, including that EU Data Boundary customers can’t use real-time agents. A new Known limitations section details digital messaging preview constraints such as authentication, session length, and analytics coverage.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/voice-realtime-voice-agents

## Moderate Changes

- **Microsoft MCP server certification (preview)**
  Added a critical note that only ASCII header names and values are supported in manifest and tool definition files. This helps prevent validation failures caused by non-ASCII characters during certification workflows.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/mcp-certification

- **Choose how to control the conversation**
  Generalized the guidance from voice-specific to agent design across channels and removed preview labels to reflect GA. The core design guidance remains, making the article applicable for broader agent scenarios.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/guidance/voice-agents-control-conversation

- **Voice agent prompt best practices**
  Updated to reflect GA by removing preview labels and notices. The underlying best practices remain unchanged.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/guidance/voice-agents-prompt-best-practices

- **Tools, knowledge, MCP, and API**
  Removed preview status indicators to align with GA. Guidance content remains the same while signaling production readiness.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/guidance/voice-agents-tools-knowledge-mcp