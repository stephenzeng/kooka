# Power Platform
**Date created:** 2026-08-25 UTC  
**Tags:** Automation, Configuration, Get Started, Guidance, Security  

## New Articles

- **Connect Dataverse Git integration to Azure DevOps**

  Added a step-by-step how-to for connecting Microsoft Dataverse Git integration to Azure DevOps. It outlines prerequisites, repository setup, and how to connect from the Solutions experience using either environment or solution binding. The article clarifies selection of organization, project, repository, and branch (including optional branch creation) and documents limitations such as not supporting Default or Common Data Service Default solutions. It also links to guidance on choosing binding types, performing repository operations, and using the API to connect or disconnect.

  https://learn.microsoft.com/en-us/power-platform/alm/git-integration/connecting-to-azure-devops

- **Connect Dataverse Git integration to GitHub**

  Introduced a preview how-to for connecting Dataverse Git integration to GitHub. The guidance covers end-to-end setup: creating and configuring a GitHub App, installing it on the target repo, storing the private key in Azure Key Vault, and creating a GitHub OAuth connection in Power Apps. It explains how to connect from an unmanaged solution with the required app configuration, and how to grant Key Vault access to the Dataverse managed identity. The article includes verification steps and programmatic alternatives via the Dataverse Web API or PowerShell.

  https://learn.microsoft.com/en-us/power-platform/alm/git-integration/connecting-to-github

## Major Changes

- **FAQs about source code integration**

  Expanded Git integration from Azure DevOps-only to include GitHub, with updated prerequisites for provider-specific permissions and managed environments. Revised licensing guidance and clarified repository initialization, default branch selection, and that file size limits depend on the chosen provider. Generalized security scanning recommendations, updated related links to provider-specific connection guides, and refined wording for branch workflows and CI/CD automation.

  https://learn.microsoft.com/en-us/power-platform/alm/git-integration/faqs

- **Connect and disconnect Dataverse from a Git repository by using code**

  Extended API guidance to support GitHub in addition to Azure DevOps, including new parameters for GitHub integration and related requirements. Added end-to-end examples for creating a GitHub App configuration via the Dataverse Web API, setting up Azure Key Vault and RBAC for the managed identity, and invoking ConnectToGit with GitHub parameters. Included a full PowerShell example to automate configuration and connection, and removed the prior limitation that only Azure DevOps was supported.

  https://learn.microsoft.com/en-us/power-platform/alm/git-integration/git-api

## Moderate Changes

- **Connect to Git**

  Reworked the page to be provider-agnostic, focusing on common connection options and post-connection tasks while moving Azure DevOps specifics to new provider guides. Clarified when to use environment versus solution binding and updated multi-environment guidance with provider-neutral language and links to provider-specific setup.

  https://learn.microsoft.com/en-us/power-platform/alm/git-integration/connecting-to-git

- **Overview of Git integration in Power Platform**

  Updated the overview to reflect support for GitHub and other providers, and clarified that Git integration is intended for developer environments with deployments handled through builds and pipelines. Refreshed Next steps with targeted guides for connecting to a provider, Azure DevOps, and GitHub.

  https://learn.microsoft.com/en-us/power-platform/alm/git-integration/overview

- **Source control repository operations**

  Generalized instructions to work with any Git provider when viewing commits and related repository operations. Expanded Next steps with specific links for connecting to a provider, Azure DevOps, and GitHub.

  https://learn.microsoft.com/en-us/power-platform/alm/git-integration/source-control-operations