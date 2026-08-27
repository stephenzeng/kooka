# Dynamics 365 Supply Chain Management
**Date created:** 2026-08-27 UTC  
**Tags:** Configuration, Get Started, Guidance, Identity  

## Major Changes

- **Set up and configure supplier communications features of the Procurement Agent (production-ready preview)**
  
  Expanded and reorganized the setup guidance to provide end-to-end instructions, including detailed prerequisites, required app versions and installation order, DLP considerations, and Copilot Studio agent publishing. Added a new section on the agent identity user, clarified wizard steps for prerequisite verification, identity setup, mailbox configuration (shared and private), and linked permission references, plus a video instructions link. Removed outdated sandbox refresh and personal email testing content, and updated the title to reflect production-ready preview status, improving clarity, security alignment, and reducing setup errors.
  
  https://learn.microsoft.com/en-us/dynamics365/supply-chain/procurement/procurement-agent-supplier-com-setup-wizard

## Moderate Changes

- **Set up and configure impact analysis features of the Procurement Agent (production-ready preview)**
  
  Updated guidance with a comprehensive prerequisites list (required versions, feature flags, app components, and install order), DLP policy considerations, and verification steps for Copilot Studio agent publication. Introduced an explanation of the agent identity user and refined the deployment wizard steps to reference and validate prerequisites. These changes streamline deployment and help ensure correct configuration and compliance.
  
  https://learn.microsoft.com/en-us/dynamics365/supply-chain/procurement/procurement-agent-impact-analysis-setup-wizard

- **Test supplier communications features (production-ready preview)**
  
  Enhanced sandbox testing guidance by prioritizing a full data refresh followed by ongoing purchase-order delta syncs via Data management. Clarified that the agent processes emails only from vendor domains and provided steps to add a tester’s email as a vendor contact to enable forwarding from personal accounts. These updates improve test realism and ensure accurate email processing behavior.
  
  https://learn.microsoft.com/en-us/dynamics365/supply-chain/procurement/procurement-agent-supplier-com-testing