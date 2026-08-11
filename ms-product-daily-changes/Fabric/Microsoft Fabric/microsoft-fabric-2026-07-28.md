# Microsoft Fabric
**Date created:** 2026-07-28 UTC  
**Tags:** Administration, Analytics, Automation, Governance, Monitoring, Programming, Security  

## New Articles

- **Merge Queries**

  Introduced a how-to guide for the Merge Query feature in Infobridge, which creates a new merged query without altering sources. Clarifies that merging requires matching row and column dimensions and walks through selecting measures from multiple queries. Includes an end-to-end example (Product Sales + Product Pricing) with illustrative results and step-by-step instructions.

  https://learn.microsoft.com/en-us/fabric/iq/plan/infobridge-transform-queries/how-to-merge-query

- **Read data secured with OneLake security**

  Added guidance on how OneLake-enforced row-level (RLS) and column-level (CLS) security are evaluated across engines and what happens when engines aren’t authorized. Details support and configuration requirements for engines such as Eventhouse, Lakehouse, Spark notebooks, SQL analytics endpoints (user’s identity access mode), semantic models using Direct Lake, and authorized third-party engines. Explains enforcement behavior, how authorized engines retrieve effective permissions, and provides links to core OneLake security setup topics.

  https://learn.microsoft.com/en-us/fabric/onelake/security/read-secured-data

- **OneLake row-level security (RLS) syntax**

  Published a reference for writing OneLake RLS rules using SQL SELECT predicates, including supported operators, syntax limits, and collation behavior. Provides patterns and best practices for secure, strongly typed filters, plus placeholder conventions for schema, table, and column references. Links to related role management and security guidance to help authors implement and troubleshoot RLS.

  https://learn.microsoft.com/en-us/fabric/onelake/security/row-level-security-syntax

- **OneLake table, column, and row-level security**

  Introduced a concept article covering object-level security for tables/folders, column-level security (CLS), and row-level security (RLS) in OneLake. Explains enforcement modes for authorized vs. unauthorized engines, supported table types, and evaluation behavior and errors for rule mismatches. Describes differences in CLS behavior across engines, how RLS is applied to tabular data, and how to combine CLS and RLS in a single role (and the limitation of using separate roles). Includes links to creation, reading, and syntax references.

  https://learn.microsoft.com/en-us/fabric/onelake/security/table-column-row-security

- **Temp tables in Fabric Data Warehouse**

  Added documentation for session-scoped temporary tables, including lifecycle and visibility. Describes non-distributed (MDF-backed) and distributed (Parquet-backed) temp tables with creation syntax and when to use each for full T-SQL compatibility. Highlights limitations such as unsupported global temp tables, time-travel hints, and ALTER TABLE constraints.

  https://learn.microsoft.com/en-us/fabric/data-warehouse/temp-tables

- **Tutorial: End-to-end automation in Fabric**

  Launched a comprehensive tutorial demonstrating a full CI/CD flow for Fabric with clear separation of control-plane and data-plane operations. Covers provisioning dev/test workspaces via Terraform, configuring an Azure DevOps Git connection with a service principal, and deploying items using the fabric-cicd Python library with environment parameterization. Prerequisites were clarified to ensure the ADO repo has the target branch and directory (with a placeholder file) to avoid provisioning failures, and the Terraform provider was updated to version 1.12.0 with the preview flag removed. Includes validation, deployment, pipeline automation considerations, and cleanup steps.

  https://learn.microsoft.com/en-us/fabric/cicd/tutorial-end-to-end-automation

## Major Changes

- **Collect Apache Spark applications logs and metrics using Azure Event Hubs**

  Removed guidance for certificate-based authentication, including app registration, Key Vault certificate setup, and related Spark properties. This deprecates certificate-driven setup for Event Hubs emitters and directs users toward supported authentication methods to simplify configuration and reduce security complexity.

  https://learn.microsoft.com/en-us/fabric/data-engineering/azure-fabric-diagnostic-emitters-azure-event-hub

- **Collect your Apache Spark applications logs and metrics using Azure Storage account**

  Eliminated the certificate authentication option for Azure Storage diagnostic emitters and the associated steps (app registration, Key Vault certificates, role assignments, ServicePrincipalCert Spark properties). This streamlines guidance to supported authentication approaches and helps prevent misconfiguration with deprecated patterns.

  https://learn.microsoft.com/en-us/fabric/data-engineering/azure-fabric-diagnostic-emitters-azure-storage

- **OneLake security roles: create and manage**

  Expanded and reorganized role management guidance, including clearer role scoping, data/member management, and editing workflows. Added detailed instructions for applying RLS and CLS, membership via permission groups, and streamlined delete steps, improving administrators’ ability to set up and audit access consistently.

  https://learn.microsoft.com/en-us/fabric/onelake/security/create-manage-roles

- **Enable workspace monitoring for eventstreams (preview)**

  Added a prominent notice that workspace monitoring for eventstreams is temporarily disabled due to an identified issue, with a link to the known issue. This informs users of current unavailability and directs them to track resolution status.

  https://learn.microsoft.com/en-us/fabric/real-time-intelligence/event-streams/enable-fabric-workspace-monitoring

- **OneLake Security for SQL analytics endpoints**

  Updated the authorization model to evaluate the signed-in user and effective Microsoft Entra group membership, removing the need for strict identity mapping between producer and consumer artifacts. Clarified shortcut behavior and security sync across tables, and removed outdated prerequisites (such as restrictions on service principal ownership). These changes simplify setup, reduce identity management overhead, and align troubleshooting with the new evaluation model.

  https://learn.microsoft.com/en-us/fabric/onelake/security/sql-analytics-endpoint-onelake-security

## Moderate Changes

- **Application lifecycle management tutorial**

  Step 1 now targets creating a general workspace and updates licensing guidance from Power BI Premium to Fabric capacity. References and headings were aligned to reflect the new flow.

  https://learn.microsoft.com/en-us/fabric/cicd/cicd-tutorial

- **Eventstream workspace monitoring overview (preview)**

  Added an IMPORTANT notice that eventstream workspace monitoring is temporarily disabled while a fix with improved controls is implemented. Provides a pointer to the known issues page for status updates.

  https://learn.microsoft.com/en-us/fabric/real-time-intelligence/event-streams/fabric-workspace-monitoring

- **Eventstream workspace monitoring - known limitations (preview)**

  Added an IMPORTANT notice about the temporary disablement of workspace monitoring for eventstreams, with a link to the specific known issue. This helps users understand current constraints and timelines.

  https://learn.microsoft.com/en-us/fabric/real-time-intelligence/event-streams/fabric-workspace-monitoring-known-limitations

- **Eventstream monitoring tables overview (preview)**

  Added an IMPORTANT notice that eventstream workspace monitoring is temporarily disabled and linked to the known issues page, noting that a fix with enhanced controls is in progress. This sets expectations for data availability.

  https://learn.microsoft.com/en-us/fabric/real-time-intelligence/event-streams/fabric-workspace-monitoring-tables

- **Use Iceberg tables with OneLake**

  Introduced a temporary limit of 5,000 transactions/commits on source tables for format conversion in table format virtualization. Recommends compacting transaction logs or manifests to reduce transaction counts and enable conversion.

  https://learn.microsoft.com/en-us/fabric/onelake/onelake-iceberg-tables

- **Use Python for Apache Spark**

  Updated references from Synapse to Fabric and renamed Microsoft Spark Utilities to NotebookUtils with revised examples. This aligns code and guidance with current APIs and reduces confusion for notebook authors.

  https://learn.microsoft.com/en-us/fabric/data-science/python-guide/python-overview

- **Query Eventstream monitoring data (preview)**

  Added an IMPORTANT notice that eventstream workspace monitoring is temporarily disabled and linked to the known issue for details. No changes were made to query procedures.

  https://learn.microsoft.com/en-us/fabric/real-time-intelligence/event-streams/query-fabric-workspace-monitoring-data

- **Tutorial: Use R to predict avocado prices**

  Updated R examples to remove the hms import and align ggplot2 usage with current conventions (using linewidth and removing unsupported outlier.shape). Ensures the tutorial runs cleanly on newer libraries.

  https://learn.microsoft.com/en-us/fabric/data-science/r-avocado

- **Tables in Fabric Data Warehouse**

  Replaced an extensive temp tables section with a concise pointer to a dedicated article and noted support for IDENTITY columns (Preview). Minor language and navigation improvements make temp table guidance easier to find and maintain.

  https://learn.microsoft.com/en-us/fabric/data-warehouse/tables

## Minor Changes