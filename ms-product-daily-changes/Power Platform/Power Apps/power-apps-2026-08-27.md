# Power Apps
**Date created:** 2026-08-27 UTC  
**Tags:** Automation, Configuration, Guidance, Security  

## Major Changes

- **Developer Tools for Model-Driven Apps**

  Reorganized and expanded the article to clearly separate tools available via Power Platform ToolBox and XrmToolBox. Added and detailed popular utilities such as Command Bar Studio, Dataverse Request/REST Builder, FetchXML Builder/Studio, PCF Builder, Easy Translator, Side Pane Studio, View Layout Copier, and Web Resource Manager. Updated the introduction to emphasize developer tooling for model-driven apps and clarified community tool availability, making it easier to find and choose the right tool for the job.

  https://learn.microsoft.com/en-us/power-apps/developer/model-driven-apps/developer-tools

## Moderate Changes

- **Configure Form Query String Parameters in Model-Driven Apps**

  Retitled and refocused guidance to stress secure handling and validation of custom query string parameters. Expanded setup instructions with modern editor context, steps for using Form Properties in the classic editor, clearer FormXml details for name and type (including naming constraints and that PositiveInteger includes 0), and added related links and visuals to streamline configuration.

  https://learn.microsoft.com/en-us/power-apps/developer/model-driven-apps/configure-form-accept-custom-querystring-parameters

- **Package a Code Component in a Solution File**

  Expanded the article to cover the full workflow: packaging a code component into a solution ZIP, importing to Dataverse, and deploying updates with Power Platform CLI. Added step-by-step commands for creating and building solutions, environment authentication and inspection (pac auth, pac org who), deployment via pac pcf push, and clean removal by updating the project, improving reliability and consistency across deployments.

  https://learn.microsoft.com/en-us/power-apps/developer/component-framework/import-custom-controls