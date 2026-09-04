# Microsoft Foundry
**Date created:** 2026-09-04 UTC  
**Tags:** Best Practices, Configuration, Deprecation, Get Started, Governance, Guidance, Performance, Security  

## Major Changes

- **MAI-Transcribe-2 - Speech Service**
  
  Introduced MAI-Transcribe-2 as the primary transcription model with expanded guidance on capabilities such as speaker diarization, word-level timestamps, phrase biasing, transcription styles (clean/verbatim), multilingual support with code switching, and noise robustness. Updated REST usage to require enhancedMode.enabled=true and enhancedMode.model="MAI-Transcribe-2", with new examples for diarization, timestamps, transcription style, and phrase lists. The model catalog now highlights MAI-Transcribe-2 and notes prior versions (1.5 and 1) including deprecation status. Content was reorganized and SDK guidance updated to align with the REST configuration, helping teams adopt the new model consistently.
  
  https://learn.microsoft.com/en-us/azure/ai-services/speech-service/mai-transcribe

## Moderate Changes

- **Batch synthesis API for text to speech**
  
  Added a requirement that the destination storage account for batch synthesis output must allow access from all networks; network-restricted accounts aren’t supported. This clarifies storage firewall needs to prevent job failures during output writes.
  
  https://learn.microsoft.com/en-us/azure/ai-services/speech-service/batch-synthesis

- **Batch synthesis properties for text to speech avatar**
  
  Updated properties.destinationContainerUrl to require a destination storage account that allows access from all networks; network-restricted accounts aren’t supported. The doc also clarifies expectations for multi-video jobs, optionality for single video, and that this property isn’t returned in responses, improving configuration accuracy.
  
  https://learn.microsoft.com/en-us/azure/ai-services/speech-service/text-to-speech-avatar/batch-synthesis-avatar-properties

- **Batch synthesis properties for text to speech**
  
  Clarified that properties.destinationContainerUrl must point to a storage account open to all networks; network-restricted accounts aren’t supported. This helps avoid access errors when writing batch synthesis results.
  
  https://learn.microsoft.com/en-us/azure/ai-services/speech-service/batch-synthesis-properties

- **Improve recognition accuracy with phrase list**
  
  Increased the maximum phrase list size from 500 to 2,000 entries. Added guidance that very long lists can degrade recognition quality and increase latency so users can balance coverage with performance.
  
  https://learn.microsoft.com/en-us/azure/ai-services/speech-service/improve-accuracy-phrase-list

- **Use personal voice in your application**
  
  Removed MAI-Voice-1 from the base model comparison. Updated guidance to direct project creation and management to the Microsoft Foundry portal, positioning Speech Studio as a demo-only experience to streamline production workflows.
  
  https://learn.microsoft.com/en-us/azure/ai-services/speech-service/personal-voice-how-to-use

- **What is personal voice for text to speech?**
  
  Updated availability and demo guidance to include the Microsoft Foundry portal alongside Speech Studio, with a new link to “Create a project for personal voice.” The page now encourages using the Foundry portal for managing projects while leveraging Speech Studio for guided demos.
  
  https://learn.microsoft.com/en-us/azure/ai-services/speech-service/personal-voice-overview

- **Prebuilt analyzers in Azure Content Understanding in Foundry Tools**
  
  Removed the “Lock analyzer behavior” section and the associated copy API example. This signals that freezing a prebuilt analyzer via copy is no longer documented, prompting teams to plan for analyzer evolution in their pipelines.
  
  https://learn.microsoft.com/en-us/azure/ai-services/content-understanding/concepts/prebuilt-analyzers

- **Service limits in Azure AI Search**
  
  Reworked knowledge source limits to a single tier-based maximum and clarified that API version and reasoning effort now govern how many sources can be selected at retrieval time. Updated the API version matrix and noted that minimal reasoning uses all sources, guiding customers to tune retrieval behavior by version and effort level.
  
  https://learn.microsoft.com/en-us/azure/search/search-limits-quotas-capacity

- **Connect to Azure AI Search using keys**
  
  Rewrote migration guidance from keys to roles with explicit assignments: use Search Service Contributor for managing search objects and Search Index Data Contributor/Reader for data-plane access. Added an IMPORTANT note that Search Service Contributor is a control-plane role that can retrieve admin keys, recommending limited assignment to trusted users.
  
  https://learn.microsoft.com/en-us/azure/search/search-security-api-keys

- **Connect to Azure AI Search using roles**
  
  Clarified the Search Service Contributor role: it can retrieve admin and query keys via control-plane operations but cannot perform data-plane actions like loading documents or querying indexes. This helps set correct expectations and align security assignments.
  
  https://learn.microsoft.com/en-us/azure/search/search-security-rbac

- **Voice Live `2025-10-01` API Reference**
  
  Updated personal voice configuration to remove MAI-Voice-1 from allowed base models. Only DragonLatestNeural and DragonHDOmniLatestNeural are supported, guiding customers to compatible models.
  
  https://learn.microsoft.com/en-us/azure/ai-services/speech-service/voice-live-api-reference-2025-10-01

- **Voice Live `2026-01-01-preview` API Reference (preview)**
  
  Removed MAI-Voice-1 from the list of allowed base models in personal voice settings. Supported options are now DragonLatestNeural and DragonHDOmniLatestNeural, aligning preview usage with current model support.
  
  https://learn.microsoft.com/en-us/azure/ai-services/speech-service/voice-live-api-reference-2026-01-01-preview

- **Voice Live `2026-04-10` API Reference**
  
  Updated the personal voice model list to remove MAI-Voice-1. The configuration now supports only DragonLatestNeural and DragonHDOmniLatestNeural, reducing confusion about deprecated models.
  
  https://learn.microsoft.com/en-us/azure/ai-services/speech-service/voice-live-api-reference-2026-04-10

- **Voice Live `2026-06-01-preview` API Reference**
  
  Removed MAI-Voice-1 from allowed base models for the personal voice configuration. Use DragonLatestNeural or DragonHDOmniLatestNeural to ensure compatibility with current APIs.
  
  https://learn.microsoft.com/en-us/azure/ai-services/speech-service/voice-live-api-reference-2026-06-01-preview

- **How to customize Voice Live input and output**
  
  Updated supported base model lists to remove MAI-Voice-1 for personal voice and voice sync for custom avatars. The guidance now lists only DragonLatestNeural and DragonHDOmniLatestNeural, helping users select supported models for customization.
  
  https://learn.microsoft.com/en-us/azure/ai-services/speech-service/voice-live-how-to-customize