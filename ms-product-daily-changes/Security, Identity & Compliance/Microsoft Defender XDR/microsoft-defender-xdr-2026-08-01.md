# Microsoft Defender XDR
**Date created:** 2026-08-01 UTC  
**Tags:** Security  

## Major Changes

- **What is Microsoft Defender Experts MDR?**

  Introduced a two-plan model: Plan 1 focuses on Microsoft Defender workloads, while Plan 2 adds expert-led coverage for selected third-party telemetry via Microsoft Sentinel. Added detailed capabilities, prerequisites, and guidance to help customers choose the right plan, along with a supported third‑party source matrix (for example, Okta, Proofpoint TAP, AWS, Palo Alto, Cisco, Zscaler, Fortinet). Clarified service boundaries: the service is not a managed SIEM or an incident response engagement, and Defender for Cloud workloads are out of scope. Announced deprecation of third‑party network signal enrichment under Plan 1 effective September 1, 2026, with coverage shifting to Plan 2, and added links to getting started and FAQ.

  https://learn.microsoft.com/en-us/defender-xdr/defender-experts/defender-experts-mdr-overview

- **General information on Defender Experts MDR service**

  Expanded the FAQ to introduce the differences between Plan 1 and Plan 2, including Sentinel dependencies by plan. Clarified that Plan 2 requires a Microsoft Sentinel workspace, is not a managed SIEM, and customers retain ownership for connectors, ingestion, analytics, retention, permissions, and costs. Emphasized that MDR augments rather than replaces a SOC, and that for third‑party products under Plan 2, analysts provide guidance rather than act directly in those tools.

  https://learn.microsoft.com/en-us/defender-xdr/defender-experts/defender-experts-mdr-faq

- **Enriching Defender Experts MDR with third-party network signals**

  Announced deprecation of third‑party network signal enrichment in favor of Defender Experts MDR Plan 2, effective September 1, 2026; new enablements are closed and existing coverage continues until renewal. Updated guidance directs customers to contact their Security Delivery Expert only for questions on existing coverage. Clarified that enrichment does not include triage or investigation, while Plan 2 includes investigation for approved third‑party and multicloud sources, with a link to plan details.

  https://learn.microsoft.com/en-us/defender-xdr/defender-experts/defender-experts-mdr-third-party-enrichment

## Moderate Changes

- **Before you begin using Defender Experts MDR**

  Added a dedicated Plan 2 prerequisites section covering Sentinel-based telemetry, deployment of supported EDR, identity and email security for all users, CNAPP/CWPP for monitored infrastructure, and data ingestion via built‑in Sentinel connectors. Included required configurations such as granting experts access to Sentinel workspaces, connecting Sentinel to the Defender portal, setting 90‑day Log Analytics retention, and enabling UEBA for supported sources—helping customers prepare environments for successful onboarding.

  https://learn.microsoft.com/en-us/defender-xdr/defender-experts/defender-experts-mdr-prerequisites

- **Communicating with experts in the Microsoft Defender Experts service**

  Updated eligibility for inclusion of a Security Delivery Expert from “licensed for 500 or more devices” to “licensed for 1,500 or more seats,” aligning terminology and threshold with the new plan model. Organizations should review licensing to understand whether they qualify for this engagement model.

  https://learn.microsoft.com/en-us/defender-xdr/defender-experts/defender-experts-mdr-communication

- **Understanding Defender Experts coverage for servers and cloud workloads**

  Clarified that Defender Experts MDR Plan 2 does not cover Microsoft Defender for Cloud workloads. Reinforced that Plan 2 provides expert coverage for supported third‑party telemetry via Sentinel and directed customers to Defender Experts for Servers or Defender Experts Hunting – Servers for servers protected by Defender for Cloud, with a link to plan guidance.

  https://learn.microsoft.com/en-us/defender-xdr/defender-experts/defender-experts-faq-cloud-coverage

- **Microsoft Defender Experts**

  Updated the service overview to reflect a two‑plan MDR model, covering Microsoft Defender workloads in Plan 1 and extending expert triage and investigation to supported third‑party sources via Microsoft Sentinel in Plan 2. This helps customers align service selection with their telemetry mix and operational needs.

  https://learn.microsoft.com/en-us/defender-xdr/defender-experts/defender-experts-overview