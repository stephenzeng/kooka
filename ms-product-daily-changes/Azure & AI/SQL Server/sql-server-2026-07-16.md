# SQL Server
**Date created:** 2026-07-16 UTC  
**Tags:** Administration, Programming, Security  

## New Articles

- **Customize Keyboard Shortcuts**

  Introduced a how-to guide for tailoring keyboard shortcuts in the MSSQL extension for Visual Studio Code using either VS Code keybindings or the extension’s Result View shortcuts. Explained when to use each approach and highlighted the MSSQL Database Management Keymap for familiar SSMS/Azure Data Studio bindings. Added a Shortcuts Configuration (Preview) UI for managing both systems, along with step-by-step instructions and JSON examples. Included default command mappings and reference tables to speed up query and results-grid workflows, plus links to related resources.

  https://learn.microsoft.com/en-us/sql/tools/visual-studio-code-extensions/mssql/mssql-keyboard-shortcuts?view=sql-server-ver17

- **SQL Database Projects Refactor Overview**

  Added a conceptual article on how refactoring is tracked in SQL database projects and how the refactor log alters deployment to handle renames and moves without drop-and-create. Described the refactor log lifecycle, tracking via [dbo].[__RefactorLog], and how to include a .refactorlog so it’s packaged into the .dacpac. Provided step-by-step guidance for rename and move-to-schema operations in Visual Studio Code and Visual Studio, with notes on manual entries for SSMS. Included an XML reference with examples and best practices, plus links to project properties, tutorials, and SqlPackage publish guidance.

  https://learn.microsoft.com/en-us/sql/tools/sql-database-projects/concepts/refactor-overview?view=sql-server-ver17

## Moderate Changes

- **ALTER DATABASE (Transact-SQL) compatibility level**

  Updated the documented default compatibility level for new databases on Azure SQL Managed Instance (with the SQL Server 2022 update policy) from 150 to 160. This affects optimizer behavior and feature availability, so administrators should review deployment templates and scripts that assume the prior default.

  https://learn.microsoft.com/en-us/sql/t-sql/statements/alter-database-transact-sql-compatibility-level?view=sql-server-ver17

- **Extended Security Updates: Frequently asked questions**

  Clarified ESU support boundaries by removing prior guidance about obtaining general support through migration or ESUs with an existing support plan. ESU subscribers can file tickets specifically for issues related to ESU content or problems introduced by installing ESUs, setting clear expectations for the support process.

  https://learn.microsoft.com/en-us/sql/sql-server/end-of-support/extended-security-updates-frequently-asked-questions?view=sql-server-ver17

- **Overview**

  Expanded the MSSQL extension documentation with a Shortcuts Configuration (Preview) feature and a link to the new keyboard-shortcuts customization article. Introduced a preview Results Grid experience with a dedicated enablement setting and refined instructions for Table designer and View and edit data. These changes improve discoverability and consistency across features and headings.

  https://learn.microsoft.com/en-us/sql/tools/visual-studio-code-extensions/mssql/mssql-extension-visual-studio-code?view=sql-server-ver17

- **Deploy availability groups on Kubernetes with DH2i DxOperator on Azure Kubernetes Service**

  Revised Kubernetes YAML examples to use TCP port 51444, enable the mssqlConfigMap, and update the Service selector label key to dh2i.com/entity-name. These updates align with current labeling conventions and help avoid connectivity or deployment mismatches.

  https://learn.microsoft.com/en-us/sql/linux/business-continuity/containers/tutorial-kubernetes-dxoperator?view=sql-server-ver17