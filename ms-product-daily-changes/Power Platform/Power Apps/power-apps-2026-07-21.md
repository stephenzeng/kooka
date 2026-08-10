# Power Apps
**Date created:** 2026-07-21 UTC  
**Tags:** Administration, Analytics, Programming  

## New Articles

- **Push a code app into a solution from the CLI (preview)**

  Introduced a new how-to for using the power-apps push command to add code apps into Dataverse solutions from the CLI. Covers prerequisites, usage patterns, and the --solution-id option (including SOLUTION_ID environment variable) for precise targeting. Explains automatic solution selection behavior, how to locate a solution ID, and typical validation messages. Includes CI/CD guidance using environment variables and notes current limitations such as requiring a GUID and no source integration support.

  https://learn.microsoft.com/en-us/power-apps/developer/code-apps/how-to/push-to-solution

## Major Changes

- **Link to Microsoft Fabric**

  Overhauled and reorganized guidance to make the Link data page the central entry point, with dedicated Fabric Links and Other Links sections. Added a step-by-step wizard (Getting started, Setup configuration with Workspace identity recommendation, Select tables including finance and operations, Review and create) to streamline setup. Introduced standalone Manage tables to add/remove tables, refresh after metadata changes, and unlink without editing the link. Updated low-latency sync instructions, clarified long-term retention implications, and expanded steps for switching to Workspace identity and linking existing Azure Synapse profiles via Other Links.

  https://learn.microsoft.com/en-us/power-apps/maker/data-platform/fabric-link-to-data-platform

## Moderate Changes

- **Query and analyze the incremental updates with Azure Synapse Link for Dataverse**

  Updated the creation procedure to use Link data > Other Links > + New link > Azure Synapse, reflecting the current UI. Guidance for selecting resources, enabling incremental updates, and configuring capture intervals remains the same to reduce setup friction.

  https://learn.microsoft.com/en-us/power-apps/maker/data-platform/azure-synapse-incremental-updates

- **Create an Azure Synapse Link for Dataverse with Azure Data Lake in Power Apps**

  Revised navigation throughout to use Link data > Other Links and updated command labels for creating new links. Added notes confirming existing links require no migration and removed the obsolete Discover Hub “What’s next?” section and image.

  https://learn.microsoft.com/en-us/power-apps/maker/data-platform/azure-synapse-link-data-lake

- **Export Dataverse data in Delta Lake format**

  Aligned steps with the new interface by replacing Azure Synapse Link navigation with Link data > Other Links and clarifying + New link > Azure Synapse actions. Updated the Spark version upgrade section to match current labels and step order.

  https://learn.microsoft.com/en-us/power-apps/maker/data-platform/azure-synapse-link-delta-lake

- **Use managed identities for Azure with your Azure data lake storage**

  Updated setup steps to the Link data > Other Links entry point and clarified selecting + New link > Azure Synapse. This aligns identity and storage setup with the current navigation model.

  https://learn.microsoft.com/en-us/power-apps/maker/data-platform/azure-synapse-link-msi

- **Choose finance and operations data in Azure Synapse Link for Dataverse**

  Refreshed instructions to use Link data > Other Links and consistent command labels, and clarified Spark pool/storage selection. Expanded guidance on table selection and advanced settings, including incremental update intervals and folder structure, to streamline reporting readiness.

  https://learn.microsoft.com/en-us/power-apps/maker/data-platform/azure-synapse-link-select-FnO-data

- **Transport Azure Synapse Link for Dataverse configuration**

  Updated import steps to use Dataverse > Link data > Other Links in the destination environment. This ensures solution transport follows the current UI pathways.

  https://learn.microsoft.com/en-us/power-apps/maker/data-platform/azure-synapse-link-solution

- **Create an Azure Synapse Link for Dataverse with your Azure Synapse Workspace | MicrosoftDocs**

  Moved creation and management to Link data > Other Links and added a note that existing links keep running while new links must be created via the new path. Simplified steps for table management and removed the outdated Discover Hub section.

  https://learn.microsoft.com/en-us/power-apps/maker/data-platform/azure-synapse-link-synapse

- **Link your Dataverse environment to Microsoft Fabric and unlock deep insights**

  Made Link data the primary entry point (+ New link > Fabric link), adjusted Analyze in Fabric commands, and revised admin workflows to Manage tables on the Link data page. Removed an embedded video and added notes on ongoing investments, current single-workspace limitation, and planned improvements for table selection and multiple links.

  https://learn.microsoft.com/en-us/power-apps/maker/data-platform/azure-synapse-link-view-in-fabric