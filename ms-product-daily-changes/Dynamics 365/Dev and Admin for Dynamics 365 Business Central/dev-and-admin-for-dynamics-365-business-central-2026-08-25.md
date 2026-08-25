# Dev and Admin for Dynamics 365 Business Central
**Date created:** 2026-08-25 UTC  
**Tags:** Best Practices, Configuration, Guidance, Identity, Licensing  

## Major Changes

- **Codeunit Object Properties in AL**

  Refocused the reference to list only properties that apply to codeunit objects and significantly expanded coverage. Added missing entries such as Description, InherentEntitlements, InherentPermissions, ObsoleteState/Reason/Tag, RequiredTestIsolation, TestHandlers, TestHttpRequestPolicy, TestPermissions, and TestType. Consolidated and streamlined navigation with updated links to the codeunit object and the central property overviews to make discovery faster and more consistent.

  https://learn.microsoft.com/en-us/dynamics365/business-central/dev-itpro/developer/properties/devenv-codeunit-properties

- **Control Add-In Object Properties**

  Expanded and reorganized the control add-in property reference to be more complete and easier to scan. Added properties for client resources and initialization (Images, Scripts, StyleSheets, StartupScript, RefreshScript, RecreateScript) and documented obsolescence fields. The cleaner structure and clearer naming make it simpler to configure and maintain control add-ins.

  https://learn.microsoft.com/en-us/dynamics365/business-central/dev-itpro/developer/properties/devenv-control-addin-properties

- **Table Key Property Reference in AL**

  Rewrote the article to explain how key properties map to SQL Server indexes and influence performance. Introduced new entries like Description, IncludedFields, and Obsolete* properties, and clarified existing ones such as Clustered, Enabled, MaintainSIFTIndex, MaintainSQLIndex, SQLIndex, SumIndexFields, and Unique. The structured reference helps developers design and govern indexes more effectively.

  https://learn.microsoft.com/en-us/dynamics365/business-central/dev-itpro/developer/properties/devenv-key-properties

- **Query Object and Element Properties**

  Restructured the content to cover query objects and their elements (data items, columns, filters) with concise lists per area. Added numerous properties including AboutText/ML, AboutTitle/ML, ContextSensitiveHelpPage, HelpLink, InherentEntitlements, InherentPermissions, ObsoleteTag, ToolTip/ML, UsageCategory, and expanded API fields, while removing generic placeholders. This provides a complete and practical reference for building robust queries.

  https://learn.microsoft.com/en-us/dynamics365/business-central/dev-itpro/developer/properties/devenv-query-properties

- **Report Property Reference in AL**

  Replaced large, inline property tables with a concise reference that links to generated overviews for report objects, extensions, data items, columns, and layouts. Added targeted pointers to frequently used properties like DataItemLink, OptionMembers, and UseTemporary, and directed request page settings to the page property overview. The streamlined structure helps authors quickly find the right property in the right context.

  https://learn.microsoft.com/en-us/dynamics365/business-central/dev-itpro/developer/properties/devenv-report-properties

- **XMLport Object and Element Properties**

  Reorganized the XMLport reference by object and element types (object, table elements, field elements, text elements, and their attributes) and expanded property coverage. Added properties like Description, NamespacePrefix, InherentEntitlements, InherentPermissions, ObsoleteTag, XmlVersionNo, FieldDelimiter, FieldSeparator, RecordSeparator, TableSeparator, and FormatEvaluate. The clearer structure and broader coverage improve discoverability and implementation accuracy.

  https://learn.microsoft.com/en-us/dynamics365/business-central/dev-itpro/developer/properties/devenv-xmlport-properties

## Moderate Changes

- **DataItemLink Property Reference**

  Clarified where DataItemLink applies by object type and added direct links to the dedicated report and query articles. Streamlined related links and reorganized the content for easier navigation.

  https://learn.microsoft.com/en-us/dynamics365/business-central/dev-itpro/developer/properties/devenv-dataitemlink-property

- **DataItemLink Property for Queries**

  Clarified how DataItemLink works on query data items, including updated syntax using AncestorDataItem.ReferenceField and emphasis on ancestor links. Documented restrictions (no FlowField/FlowFilter, and not allowed with SqlJoinType = CrossJoin) and refined the example and remarks for consistency.

  https://learn.microsoft.com/en-us/dynamics365/business-central/dev-itpro/developer/properties/devenv-dataitemlink-query-property

- **DataItemLink property on report data items**

  Explained how DataItemLink filters a child report data item using a parent/ancestor identified via DataItemLinkReference, with updated syntax and support for multiple field pairs. Streamlined the example and showed an equivalent OnPreDataItem approach for clarity.

  https://learn.microsoft.com/en-us/dynamics365/business-central/dev-itpro/developer/properties/devenv-dataitemlink-reports-property

- **Enabled Profile Property Reference**

  Updated availability to runtime 4.0, clarified the property’s behavior and default, and replaced the example with a realistic, explicitly enabled profile. This improves guidance on controlling profile availability.

  https://learn.microsoft.com/en-us/dynamics365/business-central/dev-itpro/developer/properties/devenv-enabled-profile-property

- **Enum Object and Value Properties**

  Retitled and reorganized the properties table to clearly distinguish enum object properties from enum value properties. Added documentation for Scope and UnknownValueImplementation, improving guidance for enum design and compatibility.

  https://learn.microsoft.com/en-us/dynamics365/business-central/dev-itpro/developer/properties/devenv-enum-properties

- **OptionMembers Property Reference**

  Clarified applicability to table fields and report columns and reorganized the content to focus on where and how to use OptionMembers. Updated related links and headings for consistency.

  https://learn.microsoft.com/en-us/dynamics365/business-central/dev-itpro/developer/properties/devenv-optionmembers-property

- **Profile Object Properties in AL**

  Expanded and reorganized the profile property reference into a comprehensive table. Added entries like CaptionML, Description, Obsolete*, and ProfileDescriptionML for clearer configuration and lifecycle guidance.

  https://learn.microsoft.com/en-us/dynamics365/business-central/dev-itpro/developer/properties/devenv-profile-properties

- **Promoted property on page actions**

  Clarified the legacy status of the Promoted property and recommended the newer actionref syntax, noting that removing Promoted from a published action is breaking. Expanded applicability details, defaults, and provided a concise legacy example to guide safe usage.

  https://learn.microsoft.com/en-us/dynamics365/business-central/dev-itpro/developer/properties/devenv-promoted-action-property

- **Promoted Property for Profiles**

  Clarified how Promoted controls profile visibility in Role Explorer and that the profile must be enabled. Updated version notes and example, and aligned related links for better cross-referencing.

  https://learn.microsoft.com/en-us/dynamics365/business-central/dev-itpro/developer/properties/devenv-promoted-profile-property

- **Promoted Property Reference in AL**

  Recast the page to show that Promoted applies to both page actions and profiles with explicit runtime availability for each. Added links to the specialized pages to reduce ambiguity and duplication.

  https://learn.microsoft.com/en-us/dynamics365/business-central/dev-itpro/developer/properties/devenv-promoted-property

- **AL Properties Overview for Business Central**

  Clarified how properties control objects vs. elements and added explicit syntax guidance. Expanded the AL page example to show object-level and field-level properties with captions, tooltips, and correct bindings, and refined the IntelliSense tip to encourage property discovery.

  https://learn.microsoft.com/en-us/dynamics365/business-central/dev-itpro/developer/properties/devenv-properties

- **Scope Property for Page Actions**

  Clarified that Scope determines whether an action applies to the page or to a repeater, with values Page (default) and Repeater. Simplified the article by removing platform-specific behavior and providing a concise value description.

  https://learn.microsoft.com/en-us/dynamics365/business-central/dev-itpro/developer/properties/devenv-scope-action-property

- **Scope Property Reference in AL**

  Organized the Scope property by object type, adding coverage for enum and interface objects and availability from runtime 14.0. Included a table for Cloud vs. OnPrem behavior and a syntax example to help target the right deployment environment.

  https://learn.microsoft.com/en-us/dynamics365/business-central/dev-itpro/developer/properties/devenv-scope-property

- **Scope Property for Table Objects**

  Added a clear value table for Cloud and OnPrem (runtime 4.0), documented deprecations (Extension, Internal, Personalization), and provided AL syntax. Included an important restriction for Scope = OnPrem on Microsoft-reserved platform tables and clarified that cloud-targeted extensions cannot access OnPrem tables.

  https://learn.microsoft.com/en-us/dynamics365/business-central/dev-itpro/developer/properties/devenv-scope-table-property

- **SourceTableView Property for Pages**

  Clarified how SourceTableView sets key, sort order, and filters and expanded the AL example with practical fields, captions, and tooltips. Added guidance for descending sort when overriding OnFindRecord and how to control the initial record on open.

  https://learn.microsoft.com/en-us/dynamics365/business-central/dev-itpro/developer/properties/devenv-sourcetableview-pages-property

- **SubType Property for BLOB Fields**

  Tightened scope to BLOB table fields and clarified property values and defaults (UserDefined by default). Added a typed syntax example and refreshed links to help choose the correct subtype.

  https://learn.microsoft.com/en-us/dynamics365/business-central/dev-itpro/developer/properties/devenv-subtype-blob-property

- **SubType Property for Codeunits**

  Expanded the description of Normal, Test, TestRunner, Upgrade, and Install subtypes with modern behavior details. Documented test orchestration triggers and upgrade/install triggers, and updated syntax and links to improve reliability during testing and lifecycle operations.

  https://learn.microsoft.com/en-us/dynamics365/business-central/dev-itpro/developer/properties/devenv-subtype-codeunit-property

- **SubType Property Reference in AL**

  Clarified that SubType applies to BLOB fields and codeunits and pointed to the specific, detailed articles for each. Streamlined related links and added a brief summary to set expectations.

  https://learn.microsoft.com/en-us/dynamics365/business-central/dev-itpro/developer/properties/devenv-subtype-property

- **Type Property for Entitlement Objects**

  Clarified that Type identifies the licensing source and expanded the value table with runtime availability and refined definitions. Added guidance to pair Type = Role with RoleType and updated syntax and examples for correct entitlement modeling.

  https://learn.microsoft.com/en-us/dynamics365/business-central/dev-itpro/developer/properties/devenv-type-entitlement-property

- **Type Property Reference by Object**

  Reorganized the content to show Type usage for entitlement objects (runtime 7.0) and report layouts (runtime 9.0). Simplified the page with clearer links and headings so authors can navigate to the right object-specific guidance.

  https://learn.microsoft.com/en-us/dynamics365/business-central/dev-itpro/developer/properties/devenv-type-property

- **Type Property for Report Layouts**

  Clarified the purpose and values for report layouts (RDLC, Word, Excel, Custom) with sharper definitions. Added a note to set MimeType when using Custom and documented runtime availability from 9.0.

  https://learn.microsoft.com/en-us/dynamics365/business-central/dev-itpro/developer/properties/devenv-type-report-property

- **UseTemporary Property Reference**

  Clarified applicability by directing usage to report data items and XMLport table elements, with updated links to object-specific pages. Streamlined related links and organization to reduce duplication.

  https://learn.microsoft.com/en-us/dynamics365/business-central/dev-itpro/developer/properties/devenv-usetemporary-property

- **UseTemporary Property for Report Data Items**

  Focused the page on report data items, clarified true/false usage, and emphasized that temporary tables are in-memory and ideal for calculated or aggregated data. Cleaned up examples and related links for a smoother workflow.

  https://learn.microsoft.com/en-us/dynamics365/business-central/dev-itpro/developer/properties/devenv-usetemporary-report-property

- **UseTemporary property on XMLport table elements**

  Clarified the setting for XMLport table elements with explicit true/false values and a default of false. Explained that imported records go to an in-memory temporary table (not persisted), supporting transformations before insertion.

  https://learn.microsoft.com/en-us/dynamics365/business-central/dev-itpro/developer/properties/devenv-usetemporary-xmlport-property

- **Page View Property Reference in AL**

  Reframed the article as a consolidated page view property reference and expanded the list to include Caption, CaptionML, Obsolete*, OrderBy, SharedLayout, Filters, and Visible. Updated related links for consistent navigation across property overviews.

  https://learn.microsoft.com/en-us/dynamics365/business-central/dev-itpro/developer/properties/devenv-view-properties

- **Width Property for Table and Page Fields**

  Clarified that Width suggests a column width in characters and expanded applicability to table fields, page fields, and page labels with noted runtime versions. Documented which page types are affected, inheritance and precedence rules, behavior for 0/omitted values, and how fonts/personalization can override the setting.

  https://learn.microsoft.com/en-us/dynamics365/business-central/dev-itpro/developer/properties/devenv-width-property

- **Width Property for XMLport Elements**

  Expanded coverage to XMLport text/field elements and attributes, with a property value section and a default of 0. Clarified that Width applies only when Format = FixedText and updated the syntax accordingly.

  https://learn.microsoft.com/en-us/dynamics365/business-central/dev-itpro/developer/properties/devenv-width-xmlport-property