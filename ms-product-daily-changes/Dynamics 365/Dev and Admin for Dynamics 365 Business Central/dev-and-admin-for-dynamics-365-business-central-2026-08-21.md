# Dev and Admin for Dynamics 365 Business Central
**Date created:** 2026-08-21 UTC  
**Tags:** Analytics, Best Practices, Deprecation, Guidance, Monitoring, Performance  

## Major Changes

- **Analyzing Performance Toolkit Telemetry**

  Renamed multiple telemetry custom dimension fields to use an al-prefixed schema across key events (for example, runId -> alRunID, code -> alCode, sessionCount -> alSessionCount, and lineNo -> alLineNo). Updated descriptions to clarify terminology (such as BCPT vs PRT) and corrected phrasing like “iteration.” These changes align the documentation with the latest telemetry dimension names and schema so your queries, dashboards, and alerts reflect the current field names. Update any KQL queries, analytics pipelines, or monitoring rules that reference the old names to avoid broken reports.

  https://learn.microsoft.com/en-us/dynamics365/business-central/dev-itpro/administration/telemetry-performance-toolkit-trace

## Moderate Changes

- **EventSubscriber attribute**

  Clarified how to set ObjectType and ObjectId for different event types, including trigger events: use ObjectType Table or Page for triggers and reference Database::<ObjectName> and Page::<ObjectName> accordingly. Expanded guidance on SkipOnMissingLicense and SkipOnMissingPermission defaults and streamlined examples. This helps avoid misconfigured subscriptions and ensures predictable behavior in licensed and permission-constrained environments.

  https://learn.microsoft.com/en-us/dynamics365/business-central/dev-itpro/developer/attributes/devenv-eventsubscriber-attribute

- **HandlerFunctions attribute**

  Added HttpClientHandler to the list of supported handlers and clarified invocation rules: only nonoptional handlers listed must be called, while notification handlers can be optional. Removed prior limits on invocation counts and reorganized content for clarity. This simplifies test and handler design and prevents unnecessary constraints in automation scenarios.

  https://learn.microsoft.com/en-us/dynamics365/business-central/dev-itpro/developer/attributes/devenv-handlerfunctions-attribute

- **InDataSet attribute**

  Marked InDataSet as obsolete starting with runtime 11.0 and framed its usage as legacy. Clarified historical use with dynamic control expressions and removed guidance implying it must be defined for those properties. This steers new development away from deprecated patterns and supports cleaner migration strategies.

  https://learn.microsoft.com/en-us/dynamics365/business-central/dev-itpro/developer/attributes/devenv-indataset-attribute

- **Method Attributes in AL for Business Central**

  Reworked the conceptual overview and corrected the attribute syntax pattern, replacing the prior example with a concrete IntegrationEvent(false, false) sample. Added a direct link to the IntegrationEvent reference. This improves accuracy and helps developers apply attributes correctly with practical examples.

  https://learn.microsoft.com/en-us/dynamics365/business-central/dev-itpro/developer/attributes/devenv-method-attributes

- **RunOnClient attribute**

  Clarified that RunOnClient applies to DotNet variables and is supported only in on-premises deployments. Explained that supported client API providers are routed to the web client and that arbitrary .NET objects can’t be instantiated on the web client. This guidance prevents incorrect assumptions about .NET interoperability and helps plan deployment-specific behavior.

  https://learn.microsoft.com/en-us/dynamics365/business-central/dev-itpro/developer/attributes/devenv-runonclient-attribute

- **Scope attribute**

  Updated deprecated scope mappings to use OnPrem (replacing Solution/Internal) and Cloud (replacing Personalization/Extension), and clarified that Cloud is the default. Advised using OnPrem only when methods depend on on-premises-only APIs. This ensures correct scoping for cloud compatibility and clearer intent in extensions.

  https://learn.microsoft.com/en-us/dynamics365/business-central/dev-itpro/developer/attributes/devenv-scope-attribute

- **SessionSettingsHandler attribute**

  Clarified that the handler is invoked when code calls RequestSessionUpdate rather than on generic SessionSetting updates. This sets accurate expectations for when the handler runs, improving reliability of session-related customizations.

  https://learn.microsoft.com/en-us/dynamics365/business-central/dev-itpro/developer/attributes/devenv-sessionsettingshandler-attribute

- **SuppressDispose attribute**

  Clarified when to apply [SuppressDispose] to prevent runtime disposal when a local variable goes out of scope, especially if external .NET code retains the object. Noted that assigning to another AL DotNet variable doesn’t require the attribute because the runtime tracks AL references. This prevents premature disposal issues and resource-related bugs.

  https://learn.microsoft.com/en-us/dynamics365/business-central/dev-itpro/developer/attributes/devenv-suppressdispose-attribute

- **Test attribute**

  Expanded guidance that test methods should target specific units of business logic and that transaction behavior is governed by the TransactionModel attribute. Added a related link to the TransactionModel reference and reorganized the links. This helps authors design reliable, transaction-aware tests.

  https://learn.microsoft.com/en-us/dynamics365/business-central/dev-itpro/developer/attributes/devenv-test-attribute

- **TryFunction attribute**

  Replaced the example with a complete AL codeunit that demonstrates [TryFunction], including a simplified HTTPS URL check, a local labeled error message, and handling in OnRun to continue execution. This provides a clearer, production-relevant pattern for error handling without exceptions interrupting flow.

  https://learn.microsoft.com/en-us/dynamics365/business-central/dev-itpro/developer/attributes/devenv-tryfunction-attribute