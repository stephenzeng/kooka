# Microsoft Foundry
**Date created:** 2026-07-20 UTC  
**Tags:** AI, Agent, Programming  

## Major Changes

- **Use the GPT Realtime API via WebSockets**

  Added a guided Voice-agent quickstart for speech-to-speech conversations over WebSockets, with language-specific pivots for JavaScript, Python, TypeScript, C#, and the Microsoft Foundry portal. This accelerates setup for conversational experiences by providing end-to-end samples and configuration steps. The translation guidance was refined to explicitly use the /openai/v1/realtime/translations endpoint with a model query parameter, helping ensure correct API usage and faster troubleshooting.

  https://learn.microsoft.com/en-us/azure/foundry/openai/how-to/realtime-audio-websockets

## Moderate Changes

- **Use the GPT Realtime API for speech and audio**

  Reorganized the guidance to focus on “Understand Realtime session types,” clarifying voice-agent, translation, and transcription patterns and how to configure them via session.update and session.type. The getting-started flow now points to dedicated WebSockets and WebRTC implementation pages, and language-specific quickstart pivots were removed in favor of a consolidated, session-based approach for clearer setup choices.

  https://learn.microsoft.com/en-us/azure/foundry/openai/how-to/realtime-audio