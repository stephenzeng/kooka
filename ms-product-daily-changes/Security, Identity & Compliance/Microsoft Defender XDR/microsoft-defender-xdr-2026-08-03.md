# Microsoft Defender XDR
**Date created:** 2026-08-03 UTC  
**Tags:** AI, Security  

## New Articles

- **Tutorial: Gather vulnerability intelligence in Microsoft Defender**

  Introduced a new step-by-step tutorial for gathering vulnerability intelligence in the Defender portal using Microsoft Threat Intelligence. It walks analysts through opening Intel explorer, searching CVE-2020-1472, pivoting to related articles and indicators (including IP 50.116.3[.]164), and exploring rich context such as reputation, services, certificates, WHOIS, subdomains, trackers, and DNS. This guidance helps teams learn practical workflows to assess exposure and pivot across intelligence artifacts efficiently. The article includes prerequisites, a safety disclaimer, a cleanup note, and links to related tutorials.

  https://learn.microsoft.com/en-us/defender-xdr/gathering-vulnerability-intelligence

## Major Changes

- **Tutorial: Gather threat intelligence and perform infrastructure chaining in Microsoft Defender**

  Relocated and retitled the tutorial to align with the rebranding to Microsoft Threat Intelligence in the Defender portal, and added an in-article rebranding notice while removing the prior retirement notice. Updated prerequisites to focus on portal access and streamlined the tutorial flow, including infrastructure chaining steps and pivots such as host pairs and WHOIS, while removing images but retaining key investigative details (IOCs, IP/ASN insights, and chaining rationale). These improvements modernize the experience under Defender XDR and make the investigation steps clearer and more actionable. The closing section was refreshed to “Related content” with an additional relevant link.

  https://learn.microsoft.com/en-us/defender-xdr/gathering-threat-intelligence-and-infrastructure-chaining

- **Use Microsoft Security Copilot for threat intelligence**

  Moved the article to Defender XDR and substantially revised it to reflect rebranding from Defender Threat Intelligence to Microsoft Threat Intelligence. Expanded guidance on where capabilities are available (Security Copilot portal and Defender portal) and added detailed steps to enable the Microsoft Threat Intelligence plugin, including updated UI elements (Sources and Prompts). Clarified how to view system capabilities and promptbooks, updated numerous links to new Defender XDR pages, and enhanced related content, feedback, and privacy sections. These updates help security teams effectively leverage Security Copilot with Microsoft Threat Intelligence for faster, more guided investigations.

  https://learn.microsoft.com/en-us/defender-xdr/security-copilot-and-defender-threat-intelligence

## Moderate Changes

- **Microsoft Threat Intelligence in Microsoft Defender XDR**

  Added guidance on using Copilot for threat intelligence within the Defender portal, including where the embedded experience appears (Threat analytics, Intel profiles, Intel explorer) and how to issue an initial request with built-in prompts. Noted session behavior changes—each page starts a new chat and conversations are saved in the standalone Security Copilot portal—so analysts can use Copilot more effectively during investigations.

  https://learn.microsoft.com/en-us/defender-xdr/defender-threat-intelligence

- **View threat intelligence in entity pages in Microsoft Defender (Preview)**

  Clarified the Reputation model with a 0–100 score, mapped categories (Malicious, Suspicious, Neutral, Unknown), contributing signals, and machine learning rule severities. Enhanced Infrastructure relationships with underlying Microsoft internet data sources (passive DNS, port scans, web crawling) and added clarity on DNS, including reverse lookups and historical mappings to improve context and decision-making.

  https://learn.microsoft.com/en-us/defender-xdr/entity-page-threat-intelligence

- **Investigate an identity**

  Updated identity risk guidance so “Confirm safe” now encompasses “Reset risk” for both the identity risk score and Microsoft Entra risk level. This streamlines remediation steps and reduces ambiguity during incident handling.

  https://learn.microsoft.com/en-us/defender-xdr/investigate-users

- **Investigate and respond using Microsoft Defender XDR**

  Replaced legacy references to Defender Threat Intelligence with Microsoft Threat Intelligence in Defender XDR and aligned capability descriptions accordingly. Refined wording and formatting for clarity without changing the procedure, improving consistency and readability for operational teams.

  https://learn.microsoft.com/en-us/defender-xdr/pilot-deploy-investigate-respond