# Dev and Admin for Dynamics 365 Business Central
**Date created:** 2026-09-02 UTC  
**Tags:** Configuration, Deprecation, Guidance  

## Moderate Changes

- **Business Central Admin Center API - App Management**

  Clarified how the installOrUpdateNeededDependencies parameter behaves across app install, extension upload/install, and app update endpoints. When enabled, dependencies are installed or updated to the latest version compatible with the environment; when disabled, missing dependencies return error details. This improves predictability for administrators without introducing new endpoints or parameters.

  https://learn.microsoft.com/en-us/dynamics365/business-central/dev-itpro/administration/administration-center-api_app_management

- **The Business Central Admin Center API MCP server (preview)**

  Removed the Uninstall app section and its POST endpoint from the reference, indicating the uninstall operation is not documented for this API. Consumers should avoid relying on an uninstall capability via the MCP server preview and adjust any integrations accordingly.

  https://learn.microsoft.com/en-us/dynamics365/business-central/dev-itpro/administration/administration-center-api-mcp

- **Create an extensibility request**

  Updated guidance to direct extensibility requests from the ALAppExtensions repository to the BCApps repository, with all links and references changed. This ensures requests are submitted and tracked in the correct location for timely processing.

  https://learn.microsoft.com/en-us/dynamics365/business-central/dev-itpro/developer/create-extensibility-request

- **Contribute a change yourself**

  Replaced ALAppExtensions references with BCApps throughout, including repository description, guidelines, and issue creation links. This streamlines contributor workflows by pointing to the active repository for extensibility changes.

  https://learn.microsoft.com/en-us/dynamics365/business-central/dev-itpro/developer/devenv-contribute-extensibility