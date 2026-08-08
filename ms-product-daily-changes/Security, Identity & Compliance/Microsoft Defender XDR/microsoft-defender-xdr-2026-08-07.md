# Microsoft Defender XDR
**Change date:** 2026-08-07 UTC  
**Tags:** Administration, AI, Agent, Analytics, Automation, Monitoring, Security  

## Major Changes

- **General information on Defender Experts MDR service**
  
  Overhauled the FAQ to remove plan-based distinctions and third‑party scope, refocusing coverage on Microsoft Defender incidents. Simplified guidance on investigation actions to reflect roles in the Defender portal and clarified that Microsoft Sentinel is only needed for enriching with third‑party network signals. Updated scope and wording across product coverage and SOC collaboration to align with the new, Defender‑only focus.

  https://learn.microsoft.com/en-us/defender-xdr/defender-experts/defender-experts-mdr-faq

- **What is Microsoft Defender Experts MDR?**
  
  Rewrote the overview to introduce a two‑plan model: Plan 1 for Microsoft Defender workloads and Plan 2 extending expert coverage to selected non‑Microsoft telemetry via Microsoft Sentinel. Added capabilities, prerequisites, minimum seat requirements, third‑party source coverage, service boundaries, and a comparison of plan differences. Documented renaming from Defender Experts for XDR to Defender Experts MDR and noted future deprecation of certain third‑party network signal enrichment.

  https://learn.microsoft.com/en-us/defender-xdr/defender-experts/defender-experts-mdr-overview

- **Before you begin using Defender Experts MDR**
  
  Added a comprehensive Plan 2 prerequisites section detailing Sentinel‑based requirements, including supported security controls, connector ingestion into standard tables, workspace access, data retention baselines, and UEBA enablement. This clarifies what organizations must deploy and configure to enable Plan 2 coverage and smooth onboarding.

  https://learn.microsoft.com/en-us/defender-xdr/defender-experts/defender-experts-mdr-prerequisites

- **Step 3. Plan for Microsoft Defender integration with your SOC catalog of services**
  
  Rebranded terminology from “Microsoft Defender XDR” to “Microsoft Defender” and refined phrasing around capability integration and next steps. A merge conflict marker was inadvertently introduced near the Next step section, which may break the document and should be resolved promptly to avoid reader confusion.

  https://learn.microsoft.com/en-us/defender-xdr/integrate-microsoft-365-defender-secops-services

## Moderate Changes

- **AlertEvidence**
  
  Expanded scope to include entities from onboarded Microsoft Sentinel workspaces, alongside Microsoft Defender services. Clarified entity types and data availability, and added guidance to join with AlertInfo on AlertId to pull related metadata.

  https://learn.microsoft.com/en-us/defender-xdr/advanced-hunting-alertevidence-table

- **AlertInfo**
  
  Clarified that when Sentinel is onboarded, alerts from accessible workspaces appear in the table, with availability depending on deployed services and workspace access. Recommended joining with AlertEvidence on AlertId to retrieve related entities and evidence.

  https://learn.microsoft.com/en-us/defender-xdr/advanced-hunting-alertinfo-table

- **Use Microsoft Sentinel functions, saved queries, and custom rules**
  
  Documented a limitation that the adx() operator isn’t supported with GDAP and advised using Microsoft Entra B2B authentication instead. This helps teams avoid unsupported configurations in custom detections.

  https://learn.microsoft.com/en-us/defender-xdr/advanced-hunting-defender-use-custom-rules

- **DeviceProcessEvents table in the advanced hunting schema**
  
  Clarified that InitiatingProcessSignerType and InitiatingProcessSignatureStatus refer to the initiating process and that ProcessVersionInfo fields are file version metadata rather than signing status. Added guidance and a sample query to join with DeviceFileCertificateInfo to retrieve signing details for created processes.

  https://learn.microsoft.com/en-us/defender-xdr/advanced-hunting-deviceprocessevents-table

- **Proactively hunt for threats with advanced hunting in Microsoft Defender**
  
  Clarified data scope and retention: native Defender XDR data is 30 days, and Sentinel analytics‑tier data is queryable per configured retention. Updated quotas and noted that data stored only in the Sentinel data lake isn’t available in advanced hunting, recommending onboarding Sentinel and configuring analytics‑tier retention for longer history.

  https://learn.microsoft.com/en-us/defender-xdr/advanced-hunting-overview

- **Take action on advanced hunting query results**
  
  Removed a sample Kusto query related to enabling certain email actions while keeping the rest of the action guidance intact. This streamlines examples without changing overall procedures.

  https://learn.microsoft.com/en-us/defender-xdr/advanced-hunting-take-action

- **Detect and investigate threats to AI agents using Microsoft Defender (Preview)**
  
  Refined the detection taxonomy to include LLM reconnaissance and rephrased several items (for example, indirect prompt injection as XPIA attempts and secret/credential leakage). Broadened access indicators to capture suspicious user or IP access.

  https://learn.microsoft.com/en-us/defender-xdr/security-for-ai/ai-agent-detection-protection

- **Microsoft Defender XDR incidents API and the incidents resource type**
  
  Clarified how to use lastUpdateTime to find incidents that changed after creation. Updated severity descriptions to note that severity can change as alerts are added or removed and that the resource doesn’t retain a severity history.

  https://learn.microsoft.com/en-us/defender-xdr/api-incident

- **List incidents API in Microsoft Defender XDR**
  
  Advised clients to poll using lastUpdateTime and evaluate severity client‑side because server‑side severity filtering isn’t supported. Clarified severity semantics and allowed values.

  https://learn.microsoft.com/en-us/defender-xdr/api-list-incidents

- **Exclude assets from automated responses in automatic attack disruption**
  
  Reframed the article around using exclusions to control automatic responses, with concrete examples like device isolation and account disablement. Corrected and improved the policy application exclusions flow, emphasizing rules for tagged devices and updating steps and headings.

  https://learn.microsoft.com/en-us/defender-xdr/automatic-attack-disruption-exclusions

- **Configure automatic attack disruption in Microsoft Defender XDR**
  
  Introduced preview support for automatic device isolation in Defender for Endpoint and clarified behavior, safeguards, and operator overrides. Added guidance to configure selective isolation and automatic attack disruption exclusions and updated deployment requirements, including containment of unmanaged devices and Standard discovery prerequisites.

  https://learn.microsoft.com/en-us/defender-xdr/configure-attack-disruption

- **Understanding Defender Experts coverage for servers and cloud workloads**
  
  Added a FAQ clarifying that Defender Experts MDR Plan 2 doesn’t cover Defender for Cloud workloads, and directed users to Defender Experts for Servers or Defender Experts Hunting – Servers for server coverage. This prevents misinterpretation of Plan 2 scope.

  https://learn.microsoft.com/en-us/defender-xdr/defender-experts/defender-experts-faq-cloud-coverage

- **Communicating with experts in the Microsoft Defender Experts service**
  
  Updated eligibility criteria to require licensing for 1,500 or more seats, clarifying both the threshold and the licensing metric. This sets clearer expectations for inclusion of Security Delivery Experts.

  https://learn.microsoft.com/en-us/defender-xdr/defender-experts/defender-experts-mdr-communication

- **Enriching Defender Experts MDR with third-party network signals**
  
  Noted that new enablement of third‑party network signal enrichment is closed and instructed organizations with existing enablement to contact their Security Delivery Expert. This sets accurate expectations for future onboarding.

  https://learn.microsoft.com/en-us/defender-xdr/defender-experts/defender-experts-mdr-third-party-enrichment

- **Microsoft Defender Experts**
  
  Updated coverage to introduce two MDR plans: Plan 1 for Microsoft Defender workloads and Plan 2 extending triage and investigation to supported third‑party sources via Microsoft Sentinel. This clarifies service options and scope.

  https://learn.microsoft.com/en-us/defender-xdr/defender-experts/defender-experts-overview

- **Protect AI assets from emerging threats and vulnerabilities using Microsoft Defender**
  
  Clarified Agent 365 integration and enumerated observability sources such as Copilot Studio, Foundry, and Agent Builder. Refined real‑time protection and threat detection descriptions, including policy‑based evaluation, logging to BehaviorInfo, covered attack categories, and incident correlation for investigation and hunting.

  https://learn.microsoft.com/en-us/defender-xdr/security-for-ai/defender-security-for-ai

- **What is Microsoft Defender XDR?**
  
  Updated terminology to “Microsoft Defender” throughout and refreshed cross‑product features by replacing “Automatic response to threats” with “Automatic attack disruption,” emphasizing high‑confidence signal correlation and proactive containment. Added a link to the dedicated automatic attack disruption article.

  https://learn.microsoft.com/en-us/defender-xdr/microsoft-365-defender

- **Search the audit log for events in Microsoft Defender XDR**
  
  Rebranded references from “Microsoft Defender XDR” to “Microsoft Defender” across the article and clarified that auditing is automatically enabled and powered by Microsoft Purview. Link texts were aligned to the new naming.

  https://learn.microsoft.com/en-us/defender-xdr/microsoft-xdr-auditing

- **Detecting human-operated ransomware attacks with Microsoft Defender**
  
  Refreshed terminology from “Microsoft Defender XDR” to “Microsoft Defender” across titles, sections, and integration descriptions. Updated the detection mapping to distinguish data exfiltration via email or cloud apps (including Defender for Cloud Apps coverage) and added a new row for file encryption on endpoints mapped to Defender for Endpoint.

  https://learn.microsoft.com/en-us/defender-xdr/playbook-detecting-ransomware-m365-defender

- **What's new in Microsoft Defender XDR**
  
  Replaced a prior GA entry with two items: a Preview for threat detection for Microsoft Agent 365 agents (with investigation via incidents and hunting) and a GA capability for real‑time protection of Agent 365 tooling servers that evaluates tool invocations and can allow or block MCP tool interactions. This clarifies current AI‑related feature availability and scope.

  https://learn.microsoft.com/en-us/defender-xdr/whats-new