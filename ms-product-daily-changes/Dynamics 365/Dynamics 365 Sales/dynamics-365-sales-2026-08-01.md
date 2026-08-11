# Dynamics 365 Sales
**Date created:** 2026-08-01 UTC  
**Tags:** Administration, Agent, AI, Automation, Programming, Security  

## New Articles

- **Integrate custom agents with Recommended Actions Agent**
  
  Introduced an end-to-end guide to integrate custom agents with the Recommended Actions Agent so developers can push prioritized actions into Dynamics 365 Sales and keep execution state synchronized. The article details prerequisites and required Dataverse privileges, the scoring architecture and UICE pipeline, and key Dataverse tables and custom APIs involved. It covers agent registration and configuration (including UpsertRecommendationAgentConfigRequest), action push and UI payload contracts with a C# example, versioning and invalidation, and bidirectional sync flows. Testing steps and a reference example using Sales Opportunity Agent help teams validate integrations and accelerate implementation.

  https://learn.microsoft.com/en-us/dynamics365/sales/developer/recommended-actions-api

## Major Changes

- **Copilot Studio agents and app registrations for sales agents**
  
  Reframed terminology to “skill-based agents” and clarified tenant-wide Entra app registration behavior with a concrete example. Expanded the Sales Qualification Agent and Sales Close Agent sections with structured tables listing agents, purposes, shared usage, and internal identifiers, and added new entries such as Company Resolver and SQA Config Assistant while removing a duplicate. Introduced a comprehensive Sales Opportunity Agent section covering research, stakeholder mapping, and shared utilities with identifiers. These updates make it easier for admins to map capabilities, standardize configuration, and govern agent usage across sales scenarios.

  https://learn.microsoft.com/en-us/dynamics365/sales/ai-agents-apps

## Moderate Changes

- **Export sales records to PDF**
  
  Removed wording that implied PDFs can be created from all entities with PDF generation enabled, narrowing and clarifying supported scope. Administrators and makers should verify which entities are supported before relying on PDF exports in processes.

  https://learn.microsoft.com/en-us/dynamics365/sales/create-quote-pdf

- **Responsible AI FAQ about natural language chat in Copilot**
  
  Updated guidance to note that sales-specific terminology works best in English and pointed to official language availability. Clarified that chat surfaces answers from structured Dataverse data only and recommended SharePoint search for unstructured documents, with steps for admins to extend results using glossary terms. This helps set accurate expectations and directs users to the right data sources.

  https://learn.microsoft.com/en-us/dynamics365/sales/faqs-sales-copilot-natural-language

- **Responsible AI FAQ about the Research and engage mode of Sales Qualification Agent**
  
  Clarified operational constraints: only one mode per organization, upgrades from Research-only to Research and engage are allowed, and removal requires Microsoft support. Added admin controls for role-based access, lead scoping, and configuration of email signatures and AI disclaimers for agent-sent emails. These changes strengthen governance, access control, and compliance for production deployments.

  https://learn.microsoft.com/en-us/dynamics365/sales/faqs-sales-qualification-agent-engage