# Power Apps
**Date created:** 2026-07-22 UTC  
**Tags:** Other, Programming  

## New Articles

- **Form modern control in canvas apps - Power Apps**

  Introduced new documentation for the modern Form control, covering how to display, edit, and create records with key properties, events, and output values. Includes guidance for using Power Fx functions (NewForm, EditForm, ViewForm, SubmitForm, ResetForm) and compares the modern control with the classic form. Highlights Fluent 2 design, responsive layout, theming, and accessibility improvements, plus clearer validation, required-field indicators, updated templates, and more reliable date and people fields. This helps makers adopt the modern form experience with consistent behavior and improved usability.

  https://learn.microsoft.com/en-us/power-apps/maker/canvas-apps/controls/modern-controls/modern-control-form

- **Upgrade Fluent UI Controls to Modern Controls**

  Added a step-by-step upgrade guide for moving from deprecated Fluent UI (v8) controls to modern controls across Teams canvas apps and custom pages. Explains benefits such as Fluent 2 design, theming, responsive sizing, accessibility, performance, and enum-based properties, and lists supported surfaces and upgradable controls. Details property mappings and breaking changes to streamline migrations and reduce friction during transitions. This guidance enables makers to plan and execute upgrades confidently while aligning with current platform best practices.

  https://learn.microsoft.com/en-us/power-apps/maker/canvas-apps/controls/modern-controls/upgrade-fluent-ui-controls-to-modern

## Major Changes

- **How to: Create a connection from the CLI (preview)**

  Expanded the article to include the list-connectors command with options, output formats, pagination behavior, and examples to improve discoverability and scripting. Clarified environment targeting using power.config.json, prefaced option usage for create-connection, and refined CI-focused examples to support automation scenarios. Removed outdated limitations that previously restricted creation to SSO-only connectors and updated cross-references for better navigation. These updates streamline connection setup, reduce confusion, and improve CI/CD workflows for app makers.

  https://learn.microsoft.com/en-us/power-apps/developer/code-apps/how-to/create-connection

- **Data Grid modern control in canvas apps**

  Promoted the Data Grid control to general availability and documented recent reliability and performance improvements, including virtualization, consistent row heights, Reset support, and fixes for search, selection, and copy/paste behaviors. Clarified column configuration using ThisItem and improved guidance on handling data source changes and search state. Updated limitations and recommended Data Grid over the Table control for tabular scenarios to enhance performance and usability. These changes help makers build scalable, data-dense experiences with clearer expectations and guidance.

  https://learn.microsoft.com/en-us/power-apps/maker/canvas-apps/controls/modern-controls/modern-control-data-grid

## Moderate Changes

- **Design a custom page for your model-driven app**

  Added a deprecation notice for Fluent UI (v8) controls in custom pages and directed makers to upgrade to modern controls. Included links to upgrade guidance to ensure continued improvements in design, performance, and accessibility. This helps teams plan migrations and avoid technical debt.

  https://learn.microsoft.com/en-us/power-apps/maker/model-driven-apps/design-page-for-model-app

- **Modern controls and properties in canvas apps**

  Updated the catalog to mark Data Grid as generally available and added a new entry for the modern Form control. This improves accuracy and helps makers discover the recommended controls for form and grid scenarios.

  https://learn.microsoft.com/en-us/power-apps/maker/canvas-apps/controls/modern-controls/modern-controls-reference

- **Table modern control in Power Apps (preview)**

  Added an important recommendation to use the Data Grid control instead of Table for tabular data, especially in data-dense or performance-sensitive cases. Clarified runtime behavior such as ReflowBehavior and that column width changes aren’t persisted, and refined capability descriptions. This guidance helps makers choose the right control and set proper expectations.

  https://learn.microsoft.com/en-us/power-apps/maker/canvas-apps/controls/modern-controls/modern-control-table

- **Recent updates to modern controls in canvas apps**

  Updated the release history to include the Form control, summarizing improvements like new screen templates, clearer required indicators, consistent typography, and more reliable people and date fields. Confirmed it retains the classic form model and functions, easing adoption for existing makers. This helps teams understand what’s new and plan updates accordingly.

  https://learn.microsoft.com/en-us/power-apps/maker/canvas-apps/controls/modern-controls/modern-control-updates

- **Use Fluent UI controls**

  Announced the deprecation of Fluent UI (v8) controls in canvas apps in Microsoft Teams and advised upgrading to modern controls. Added links to upgrade guidance to simplify migration. This ensures apps remain supported and benefit from ongoing improvements.

  https://learn.microsoft.com/en-us/power-apps/teams/use-the-fluent-ui-controls