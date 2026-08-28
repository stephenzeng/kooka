# Power Apps
**Date created:** 2026-08-28 UTC  
**Tags:** Best Practices, Configuration, Get Started, Guidance, Security  

## Major Changes

- **Create a Model-Driven App Field Component**

  Added a complete React-based ChoicesPicker example using Fluent UI with responsive behavior and dynamic resizing via trackContainerResize. Introduced guidance for handling read-only and column-level security states, plus a full localization workflow using RESX and manifest updates. Expanded end-to-end deployment steps with Power Platform CLI, including environment auth, solution setup, and control configuration, along with post-deployment debugging via Fiddler and guidance for optimized production builds. Updated images and clarified instructions to streamline implementation.

  https://learn.microsoft.com/en-us/power-apps/developer/component-framework/tutorial-create-model-driven-field-component

## Moderate Changes

- **Community resources for Power Apps component framework**

  Reorganized and expanded community resources to improve discoverability, renaming sections (for example, PCF Gallery and PCF Builder) and clarifying notes and warnings. Added updated screenshots with descriptive alt text, refined the Videos section, and significantly grew the Blogs section with new topics and practical tips. Enhanced the PCF Builder coverage across XrmToolBox, Visual Studio Code, and Power Platform Tools with updated capability descriptions.

  https://learn.microsoft.com/en-us/power-apps/developer/component-framework/community-resources

- **Publish Power Apps code apps with a service principal**

  Updated environment variable names for service principal authentication to PA_CLI_SP_CLIENT_ID, PA_CLI_SP_TENANT_ID, and PA_CLI_SP_CLIENT_SECRET across PowerShell and Bash examples. This aligns with current CLI conventions and reduces confusion without changing functionality.

  https://learn.microsoft.com/en-us/power-apps/developer/code-apps/how-to/use-service-principal