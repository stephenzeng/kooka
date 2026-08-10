# Dynamics 365 Supply Chain Management
**Date created:** 2026-07-15 UTC  
**Tags:** Administration  

## Major Changes

- **Print labels by using an external service**

  Mandates using the newer label layouts instead of legacy document routing label layouts when printing via an external service, reducing misconfiguration risk and aligning with current capabilities. Expanded prerequisites and added clear navigation to create and review label layouts, with guidance for container, license plate, and custom scenarios. Introduces step-by-step instructions to enable label layouts for license plate labels in Warehouse management parameters to ensure correct runtime behavior. Provides migration guidance using Data entities (Document routing printer layouts, Label layouts with active versions, Label layout data sources) to export and import existing configurations. Includes minor clarifications for consistency without changing core behavior.

  https://learn.microsoft.com/en-us/dynamics365/supply-chain/supply-chain-dev/label-printing-using-external-label-service