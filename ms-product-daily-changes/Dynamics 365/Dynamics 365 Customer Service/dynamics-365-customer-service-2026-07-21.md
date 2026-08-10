# Dynamics 365 Customer Service
**Date created:** 2026-07-21 UTC  
**Tags:** Administration, AI, Programming, Security  

## Moderate Changes

- **Configure knowledge management**

  Updated guidance to configure knowledge management in the Copilot Service admin center, enabling AI-powered article search and link sharing for agents. Added clear prerequisites, including required admin roles and environment-level security boundaries for KnowledgeArticle access, plus a caution against storing secrets or regulated data in draft/internal content. Streamlined setup steps to reflect the new admin center.

  https://learn.microsoft.com/en-us/dynamics365/customer-service/administer/set-up-knowledge-management-embedded-knowledge-search

- **View conversation transcripts and call recordings**

  Removed the requirement for read access to the ConversationInsights table to view conversation summaries. This reduces permission overhead and simplifies access for eligible users.

  https://learn.microsoft.com/en-us/dynamics365/customer-service/use/voice-channel-call-recordings-transcripts

- **KnowledgeArticle table in Dynamics 365 Customer Service**

  Retitled and expanded the article to focus on the KnowledgeArticle table with deeper guidance for creating, versioning, translating, publishing, and associating articles, including programmatic scenarios. Clarified key behaviors and attributes (for IDs, states, numbering, translations), updated lifecycle explanations, and aligned terminology from entity to table. Added migration and search/view count guidance to help admins and developers implement reliable knowledge workflows.

  https://learn.microsoft.com/en-us/dynamics365/customer-service/administer/work-knowledge-articles