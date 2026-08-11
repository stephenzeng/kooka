# Microsoft Copilot Studio
**Date created:** 2026-07-24 UTC  
**Tags:** AI, Agent, Governance  

## Moderate Changes

- **Configure real-time agents**

  Added support for a Text LLM option using GPT-5-Chat (Preview) that produces voice via Microsoft Neural TTS, expanding model choices for real-time agents. Introduced a comparison table and selection guidance to help choose between GPT-Realtime, GPT-Realtime-Mini (Preview), and GPT-5-Chat based on latency, voice customization, branded voice needs, and regional flexibility. Clarified expected latency from ASR→LLM→TTS processing and recommended setting caller expectations with latency messaging, while noting the broader voice catalog and custom voice support for GPT-5-Chat.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/voice-realtime-configure

- **Real-time agents overview**

  Introduced a Text LLM voice model using GPT-5-Chat (Preview) and overhauled regional prerequisites to enumerate supported models, hosting regions, and in-region processing behavior while confirming data stays in the AI resource’s Azure geography. Updated regional limitations for North America, Australia, EU, UK, and other regions, including cross-geo requirements for GPT-Realtime and GPT-Realtime-Mini (Preview) and in-region processing for GPT-5-Chat. Expanded Known limitations to note that transcript logging for Text LLM voice agents may be incomplete, affecting analytics and monitoring.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/voice-realtime-voice-agents