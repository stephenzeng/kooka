# Microsoft Fabric
**Date created:** 2026-08-01 UTC  
**Tags:** Administration, Analytics, Automation, Governance, Programming, Security  

## New Articles

- **Deploy Fabric Data Warehouse Using Pipelines**

  Introduced guidance for deploying Fabric Data Warehouse with deployment pipelines across Dev, Test, and Prod workspaces. Explains how to compare and validate T-SQL schema changes via DacFx and execute deployments from the pipeline UI, including smart defaults and exclusions (for example, security principals). Details prerequisites, column collation nuances, current limitations (no SQL analytics endpoint support, one warehouse at a time, no cross-item sequencing), and links to troubleshooting and Git integration resources.

  https://learn.microsoft.com/en-us/fabric/data-warehouse/deploy-pipelines

- **Error codes and resolutions**

  Added a comprehensive troubleshooting reference of user-facing error codes with activities, titles, and recommended fixes. Coverage spans capacity and schema issues, connections and permissions, OneLake and authentication, semantic model and Direct Lake considerations, approvals, forms, snapshots, table configuration, writeback, pipelines, and more. Helps admins and makers quickly diagnose issues and apply targeted resolutions or escalation steps.

  https://learn.microsoft.com/en-us/fabric/iq/plan/resources/error-codes-and-resolutions

- **Git Integration for Fabric Warehouse Development**

  New concept article explaining Fabric’s built-in Git integration for Data Warehouse, including branch workflows, versioning schema as a database project, and DacFx-based incremental deployment. Documents constraints and known issues for source control and Git synchronization, and provides guidance to avoid problematic patterns (for example, three-part names, inconsistent schema casing, ambiguous columns). The limitations guidance has been updated to remove the prior ALTER TABLE drop/recreate data-loss workaround and instead highlights that cyclic dependencies across warehouse items are detected and will block branch/sync operations. Includes links to how-to, troubleshooting, and related development content.

  https://learn.microsoft.com/en-us/fabric/data-warehouse/git-integration

- **How to Use Git Integration for Fabric Data Warehouse Development and Deployment**

  Step-by-step guide for connecting a workspace to Git, managing branches, and working with database projects in VS Code or SQL database projects. Shows how to sync changes between Git and Fabric, review and resolve diffs, and commit live warehouse changes using DacFx extraction. Provides practical tips for conflict resolution and verification, with links to related Git documentation.

  https://learn.microsoft.com/en-us/fabric/data-warehouse/how-to-git-integration

- **Connected Planning with Infobridge in Fabric Plan**

  Introduces connected planning concepts where updates in individual planning sheets automatically roll up into enterprise views. Walks through common scenarios and a detailed budget consolidation use case across regions, demonstrating how to import, append, and aggregate measures for corporate planning. Highlights how changes propagate automatically to consolidated budgets, improving visibility and governance.

  https://learn.microsoft.com/en-us/fabric/iq/plan/infobridge-concept-connected-planning

- **Troubleshoot Git Integration for Fabric Warehouse Development**

  Provides targeted fixes for common Git integration issues such as avoiding three-part self-references, updating outdated .sqlproj SDK versions, and qualifying columns across multi-warehouse joins. Covers schema casing under case-insensitive collations, extraction behavior for collations, and mitigating ambiguous column errors. Helps teams maintain reliable source control and smoother CI processes.

  https://learn.microsoft.com/en-us/fabric/data-warehouse/troubleshoot-git-integration

- **Upgrade Fabric Data Warehouse System File Version in a Git Integrated Fabric workspace**

  Explains how to detect and apply system file version updates for warehouses in Git-connected workspaces. Details prerequisites, the workspace-wide update flow, and how to commit resulting project changes (for example, updated SDK versions and project structure). Helps ensure repositories stay aligned with the latest project schema and tooling.

  https://learn.microsoft.com/en-us/fabric/data-warehouse/upgrade-warehouse

- **Fabric Data Warehouse System File Version History**

  Release notes for system file versions, including Version 2.0 changes such as updating Microsoft.Build.Sql SDK, adding system references, organizing shared queries, excluding XMLA.json, and introducing a project-level .gitignore. Describes re-extraction improvements for cleaner diffs and consistency, and includes guidance to upgrade from GA (Version 1.0). Enables teams to understand platform-level changes that affect source control and deployments.

  https://learn.microsoft.com/en-us/fabric/data-warehouse/warehouse-system-file-version-history

## Major Changes

- **Develop and Deploy Cross-Warehouse Dependencies**

  Streamlined guidance to focus on one-way dependencies via database references and removed the approach using pre- and post-deployment scripts. Renamed the pattern to emphasize direct references and updated tips to steer teams away from mutual dependencies. Recommends refactoring shared logic into downstream semantic models or reports to reduce coupling and improve maintainability.

  https://learn.microsoft.com/en-us/fabric/data-warehouse/cross-warehouse-development-database-projects

- **Direct Lake overview**

  Clarified that calculated columns and calculated tables that reference Direct Lake tables are not supported, removing prior preview language. Aligns OneLake and SQL endpoints on the same unsupported status for these scenarios. Helps authors avoid unsupported modeling patterns and plan alternatives early.

  https://learn.microsoft.com/en-us/fabric/fundamentals/direct-lake-overview

## Moderate Changes

- **Development and Deployment Overview**

  Retitled and reframed the article as an overview, with a feature preview note. Expanded guidance on when to use non-Git workflows, detailed Git integration capabilities, and refined explanations of deployment pipelines and CI/CD. Added links for deeper Git process understanding and related content.

  https://learn.microsoft.com/en-us/fabric/data-warehouse/development-deployment

- **Develop Warehouse Projects in Visual Studio Code**

  Added a feature preview notice and updated samples to use Microsoft.Build.Sql SDK 2.2.0. Removed pre/post-deployment script guidance and idempotency tips, and streamlined the deployment caution to focus on reviewing deployment settings, making the setup clearer and safer.

  https://learn.microsoft.com/en-us/fabric/data-warehouse/develop-warehouse-project

- **Develop Direct Lake semantic models**

  Updated guidance to state that only calculated tables referencing Direct Lake tables are supported in preview, not calculated columns. This helps model authors choose supported techniques and avoid unsupported designs.

  https://learn.microsoft.com/en-us/fabric/fundamentals/direct-lake-develop

- **Customer Lockbox for Microsoft Fabric**

  Added clarification that Microsoft engineer access to customer data in OneLake is governed by Customer Lockbox. Access requires customer approval and is time-bound, reinforcing control and transparency.

  https://learn.microsoft.com/en-us/fabric/security/security-lockbox

- **What's New?**

  Added a July 2026 entry for Warehouse source control (Preview) and removed the pre/post-scripts deployment preview entries. Updated the features table link to the new development and deployment page, improving discoverability of current guidance.

  https://learn.microsoft.com/en-us/fabric/fundamentals/whats-new