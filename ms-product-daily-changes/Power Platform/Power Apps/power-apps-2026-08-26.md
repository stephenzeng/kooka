# Power Apps
**Date created:** 2026-08-26 UTC  
**Tags:** Billing, Configuration, Consumption, Guidance, Licensing, Troubleshooting  

## Major Changes

- **Avatar Modern Control in Canvas Apps: Properties and Examples**

  The Avatar control documentation was overhauled with new interactive behavior and accessibility properties, including OnSelect, DisplayMode, AccessibleLabel, Tooltip, and ContentLanguage. Presence and shape options are now typed enums, and legacy font properties were standardized and renamed for consistency across modern controls. Defaults and styling guidance were clarified, and a comprehensive example shows badges, shapes, and navigation patterns. These updates make the control easier to configure, more accessible, and more consistent for app makers.

  https://learn.microsoft.com/en-us/power-apps/maker/canvas-apps/controls/modern-controls/modern-control-avatar

- **Spinner Modern Control in Canvas Apps: Properties and Examples**

  The Spinner control article was substantially rewritten to clarify usage as an indeterminate loader, with guidance to bind visibility to loading state. Properties were standardized and renamed, enums introduced for key settings, and new Tooltip and ContentLanguage properties added. Examples and a change log improve discoverability and help makers implement consistent, accessible loading experiences.

  https://learn.microsoft.com/en-us/power-apps/maker/canvas-apps/controls/modern-controls/modern-control-spinner

## Moderate Changes

- **Example: Create and customize a model-driven app form | MicrosoftDocs**

  Added guidance on embedding a generative page in a model-driven form to create record-aware visualizations. This enables low-code, contextual experiences that leverage the current record and links to detailed generative pages documentation.

  https://learn.microsoft.com/en-us/power-apps/maker/model-driven-apps/create-and-edit-a-model-driven-form

- **Productive main form design in model-driven apps | MicrosoftDocs**

  Expanded form design guidance to show how to embed a generative page for record-aware scenarios using natural language with editable generated code. Clarified that Power Apps component framework controls bind to fields or datasets, helping makers choose the right approach.

  https://learn.microsoft.com/en-us/power-apps/maker/model-driven-apps/design-productive-forms

- **Export, Edit, and Import the Ribbon in Model-Driven Apps**

  The ribbon editing workflow was modernized to use the maker portal for solution create/edit and export/import, with streamlined steps for preparing and editing customizations.xml. Packaging guidance was updated and troubleshooting expanded with targeted articles for common ribbon issues. These changes reduce reliance on legacy paths and make diagnostics easier.

  https://learn.microsoft.com/en-us/power-apps/developer/model-driven-apps/export-prepare-edit-import-ribbon

- **Generate a page using natural language**

  Added instructions for embedding a generative page in a form, including selecting the page in the designer and optionally providing static inputs. The form now passes the current record ID automatically to the page, simplifying setup for contextual experiences.

  https://learn.microsoft.com/en-us/power-apps/maker/model-driven-apps/generative-pages

- **Create and manage personal views on a grid page**

  Updated screenshots and refined steps for saving and managing views, including using the current view drop-down to Save as new view. Adjusted terminology (Default to Standard) and clarified flows for modern advanced find tasks to reduce confusion.

  https://learn.microsoft.com/en-us/power-apps/user/grid-filters-advanced

- **Recent updates to modern controls in canvas apps**

  Added Avatar and Spinner to the recent updates list, noting enum-based properties, new Tooltip support, and consolidated font property renames. The cross-control rename table was updated to help makers quickly align to the modern property model.

  https://learn.microsoft.com/en-us/power-apps/maker/canvas-apps/controls/modern-controls/modern-control-updates

- **Override Default Open Behavior of Data Rows in Grids**

  Reorganized and clarified the steps to override row open behavior with a custom JavaScript action, including explicit solution setup, web resource creation, and button configuration in customization.xml. Updated UI labels, added screenshots, and refined notes and code placement without changing the sample function. This makes the procedure easier to follow and implement reliably.

  https://learn.microsoft.com/en-us/power-apps/developer/model-driven-apps/override-default-open-behavior-grids

- **Configure structured content in the rich text editor (preview)**

  Clarified that structured content in the rich text editor is now a paid preview feature and requires pay-as-you-go billing. Removed prior grace-period language to set clear expectations for usage and costs.

  https://learn.microsoft.com/en-us/power-apps/maker/model-driven-apps/rte-structured-notes

- **Use the model-driven app main form and its components**

  Replaced web resource properties with a new Custom visualizations section introducing generative pages for record-aware visuals. Added guidance on creating generative pages with natural language, how the current record ID provides context, and where to configure them in the form designer, with links to embedding and web resource alternatives.

  https://learn.microsoft.com/en-us/power-apps/maker/model-driven-apps/use-main-form-and-components