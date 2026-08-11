# Microsoft Foundry
**Date created:** 2026-07-30 UTC  
**Tags:** AI, Agent, Governance, Security  

## New Articles

- **How to use the Azure AI Content Safety Provenance Detect API**

  Introduced a step-by-step guide for detecting content provenance using C2PA Content Credentials and invisible watermark markers. The article covers end-to-end setup, including creating a Content Safety resource, configuring Azure Blob Storage, enabling managed identity, and assigning the correct roles. It provides a complete PowerShell workflow for submitting asynchronous detection jobs, polling status, and interpreting results, with examples for success, no markers, and failures. Troubleshooting guidance helps resolve authorization, access, timeout, and validation errors.

  https://learn.microsoft.com/en-us/azure/ai-services/content-safety/how-to/how-to-provenance-detection

- **Provenance detection overview**

  Added an overview of the Content Provenance Detection API, explaining how it identifies Microsoft C2PA manifests and invisible watermark signals. The article clarifies scope and limitations—it's not a truth or safety detector and won’t identify all AI-generated content—so teams set the right expectations. It lists supported media types and size limits, offers practical guidance for files over 100 MB, and links to detailed how-to and reference documentation.

  https://learn.microsoft.com/en-us/azure/ai-services/content-safety/concepts/provenance-detection

## Major Changes

- **What is the Whisper model?**

  Expanded guidance separates offline (file-based) and realtime transcription workflows to help teams pick the right approach. The update details the offline transcription route, supported models, endpoint formats, and language hints with a cURL example, and clarifies that gpt-transcribe is offline-only. A comparison table outlines differences in API patterns, inputs, latency, and scenarios, improving decision-making. Recommendations under Whisper vs. Azure Speech models were reorganized for clarity without changing intent.

  https://learn.microsoft.com/en-us/azure/ai-services/speech-service/whisper-overview

## Moderate Changes

- **Deep dive into Foundry Agent Service networking**

  Updated concurrency guidance replaces a fixed global cap with region-dependent limits and clarifies the default 1:1 mapping of usable subnet IPs to concurrent sessions. Organizations can now request higher concurrency (up to 1:10) via Azure support, with details required to process requests. Subnet sizing recommendations were revised to reflect these options.

  https://learn.microsoft.com/en-us/azure/foundry/agents/concepts/agents-networking-deep-dive

- **Quickstart: Deploy a Microsoft Foundry resource by using a Bicep file**

  Added a troubleshooting section covering common deployment issues and resolutions. Guidance includes handling ServiceModelDeprecating errors, surfacing masked Azure CLI 2.74–2.75 errors with --debug, fixing AccountNameInvalid naming, and avoiding unintended region deployments by explicitly setting the location parameter.

  https://learn.microsoft.com/en-us/azure/foundry/how-to/create-resource-template

- **Built-in policies for model deployment in Microsoft Foundry portal**

  Introduced notes on built-in Azure Policy definitions for model router (public preview) to extend governance beyond model deployments. The update enables control over router regions, required routing rules, and logging, with a link to deeper policy guidance.

  https://learn.microsoft.com/en-us/azure/foundry/how-to/model-deployment-policy

- **Govern model router deployments with Azure Policy**

  Expanded policy assignment scope to management groups and clarified enforcement through the portal, API, CLI, and templates. Added compliance monitoring and drift detection details, explained Deny vs. Audit effects, updated approved-models policy naming, and introduced preview router-specific governance options for regions, routing rules, and logging.

  https://learn.microsoft.com/en-us/azure/foundry/how-to/model-router-policy

- **Rubric evaluators (preview)**

  Updated judge model guidance by replacing a ranked table with a curated list of supported chat models and recommendations. Added new model options and highlighted gpt-5.4-mini as the best balance of performance and cost while removing prior “not recommended” labeling.

  https://learn.microsoft.com/en-us/azure/foundry/concepts/evaluation-evaluators/rubric-evaluators