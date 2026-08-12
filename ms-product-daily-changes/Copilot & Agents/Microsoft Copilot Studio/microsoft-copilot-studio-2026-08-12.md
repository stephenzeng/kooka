# Microsoft Copilot Studio
**Date created:** 2026-08-12 UTC  
**Tags:** Analytics, Automation, Best Practices, Compliance, Configuration, Consumption, Governance, Guidance, Monitoring  

## New Articles

- **Run and validate an AI model migration for Copilot Studio agents**

  Introduced an end-to-end guide to plan, run, and validate AI model migrations for Copilot Studio agents. It defines acceptance gates, a reusable evaluation baseline, and key evaluation areas such as answer quality, groundedness, safety, and reliability. The article shows how to automate test runs via Power Platform APIs and outlines updates required across agent artifacts when models change. A phased plan covers preparation through post-deployment monitoring, including rollout/rollback and telemetry with OpenTelemetry/Application Insights.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/guidance/manage-agent-model-migration

- **Decide when to upgrade an AI model for Copilot Studio agents**

  Added decision guidance to determine if and when to upgrade production agents to newer AI models. It covers model lifecycle events, prerequisite checks (availability, region, safety posture, and admin enablement), and distinguishes strong versus weak reasons to upgrade. The article explains how to handle retirements, including a time-limited option to continue using a retired model, and directs readers to migration execution and validation steps.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/guidance/manage-agent-model-upgrade

- **Manage the AI model lifecycle for Copilot Studio agents**

  Added a framework to manage the full AI model lifecycle—from discovery and inventory through evaluation, deployment (ALM), and monitoring. It explains model release types, use categories and tradeoffs, provider options, and admin controls that affect availability. Practical instructions show how to build an agent/model inventory with the Power Platform Inventory API, PPAC views, and Power Platform CLI, including recommended metadata to track. The article links to follow-up guidance on upgrade decisions and migration execution.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/guidance/plan-agent-model-lifecycle

## Moderate Changes

- **Communicate the value story to stakeholders**

  Updated terminology to reflect the rebrand from Copilot Studio Kit to Copilot Agent Kit across sections, tables, and link labels. This aligns language with current naming and reduces confusion without changing guidance or functionality.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/guidance/agent-business-value-tell-value-story

- **Configure and deploy agents from the Agent Library**

  Revised FAQ and related links to use the Copilot Agent Kit name and descriptions. This ensures consistency with current product terminology while leaving link destinations and procedures unchanged.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/guidance/agent-library-overview

- **Enhance user engagement with Adaptive Cards Gallery in Copilot Agent Kit**

  Refreshed the article to use Copilot Agent Kit naming in the title, alt text, and steps, including guidance to publish the Adaptive Card Gallery agent from the new kit. The update improves clarity in setup instructions without introducing new features.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/guidance/kit-adaptive-cards-gallery

- **Monitor agents by using Agent Inventory in Copilot Agent Kit**

  Renamed connection references to the Copilot Agent Kit variants for Dataverse and Power Platform for Admins. This helps admins select the correct references and understand visibility controls, with no procedural changes.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/guidance/kit-agent-inventory

- **Install Copilot Agent Kit**

  Standardized product and connection reference names to Copilot Agent Kit across installation steps, including Dataverse, SharePoint, and Power Platform for Admins. Adjusted UI labels and download instructions to match current nomenclature so users pick the right components; no functional steps changed.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/guidance/kit-install

- **Rubrics refinement in Copilot Agent Kit**

  Updated the title and in-article references to the Copilot Agent Kit name. The content remains the same; changes are limited to terminology for consistency.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/guidance/kit-rubrics-overview

- **Rubrics reference guide**

  Replaced glossary references to Copilot Studio Kit with Copilot Agent Kit across relevant entries. No structural or procedural updates were made.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/guidance/kit-rubrics-reference

- **Set up Copilot Agent Kit by using the Setup Wizard**

  Updated the setup table to use Copilot Agent Kit connection reference names for Dataverse, Power Platform for Admins, and SharePoint. This helps users identify required references accurately; links and steps are unchanged.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/guidance/kit-setup-wizard