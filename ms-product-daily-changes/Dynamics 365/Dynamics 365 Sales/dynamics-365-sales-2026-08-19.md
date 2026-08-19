# Dynamics 365 Sales
**Date created:** 2026-08-19 UTC  
**Tags:** Configuration, Deprecation, Guidance, Security  

## Major Changes

- **Set up and configure AI-powered Data Enrichment**
  
  Clarified and expanded the required security permissions to configure Data Enrichment with the agent. Added explicit table-level needs, including org-level read for Sales Agent Configuration V2 and Sales agent profile, org-level read and user-level write for Data Quality Suggestion, and org-level read for Data Quality Source. Specified required access to the target record (Opportunity) and field-level read/update for enriched fields, and retained existing permissions for Connector, Process/Workflow, and Connection with updated terminology. These updates help admins set correct privileges, reduce setup errors, and ensure compliant deployments.
  
  https://learn.microsoft.com/en-us/dynamics365/sales/data-enrichment-agent-configure

- **Removed or deprecated features in Dynamics 365 Sales**
  
  Introduced deprecation timelines for Sales Close Agent: creation of new instances is blocked starting September 30, 2026, and all existing instances will be removed on October 30, 2026. Provided guidance to transition to the Sales Development agent to retain agent capabilities. This update helps organizations plan migrations and avoid service interruptions.
  
  https://learn.microsoft.com/en-us/dynamics365/sales/deprecations-sales

- **Sales Close Agent overview (preview)**
  
  Added a prominent deprecation notice for Sales Close Agent with key dates: no new instances after September 30, 2026, and full removal on October 30, 2026. Directed users to adopt the Sales Development agent as the replacement. This ensures teams can proactively migrate and maintain supported, forward-compatible workflows.
  
  https://learn.microsoft.com/en-us/dynamics365/sales/sales-close-agent