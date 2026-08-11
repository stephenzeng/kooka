# Dynamics 365 Guidance
**Date created:** 2026-08-01 UTC  
**Tags:** Administration, Analytics, Governance, Other  

## Major Changes

- **Overview of the Deliver services business process area within the Service to deliver end-to-end scenario**

  Removed the Deliver services process flow diagram temporarily and updated the important note to explain the catalog rename and pending July 2026 refresh. Reworked the implementation guidance into a detailed, ordered workflow covering end-to-end stages and granular execution steps such as gathering work order details, location tracking, collaboration, inventory management, asset updates, feedback collection, timesheets, and finalization. Retitled the execution section to “Do the work” to better align with the revised structure and improve clarity for implementers.

  https://learn.microsoft.com/en-us/dynamics365/guidance/business-processes/service-to-cash-perform-service-work

## Moderate Changes

- **Manage business process catalog updates in Azure DevOps**

  Standardized terminology from “deprecated” to “obsolete” and aligned guidance on handling rows marked for deletion or obsolescence. Added practical recommendations such as keeping obsolete/deleted rows for two releases, linking replacements using the Alternate Process Sequence ID, and closing the “removed” work item for consistency.

  https://learn.microsoft.com/en-us/dynamics365/guidance/business-processes/about-import-catalog-devops-updates

- **Administer system features overview**

  Added a new step, “Define address and location policies,” to the flow and implementation list, with a note that it isn’t yet reflected in the diagram. Minor formatting adjustments improve readability and alignment with the current process.

  https://learn.microsoft.com/en-us/dynamics365/guidance/business-processes/administer-to-operate-administer-system-features

- **Dynamics 365 and Azure-powered manufacturing sales framework**

  Updated technology scope to add Power BI and Azure Service Bus, renamed Azure AD to Microsoft Entra ID, renamed Azure SQL Database to Azure SQL, and removed Azure Key Vault. Clarified positioning by referring to Dynamics 365 Sales as a customer engagement solution, refreshed branding to Microsoft 365, and broadened ERP references in the lakehouse pattern to include Dynamics 365 or SAP.

  https://learn.microsoft.com/en-us/dynamics365/guidance/reference-architectures/dynamics-365-azure-powered-manufacturing-sales-framework

- **Add a control for note-taking to the Field Service mobile app**

  Removed preview labels and disclaimers to reflect general availability. The guidance remains the same, signaling that the feature is now supported for production use.

  https://learn.microsoft.com/en-us/dynamics365/guidance/resources/field-service-mobile-take-notes

- **Dynamics CRM or Dynamics 365 (on-premises) to Dynamics 365 online migration process overview**

  Expanded the scope to cover Dynamics 365 (on-premises) in addition to Dynamics CRM, and updated the supported versions table and SQL Server wording. Removed an eligibility note and refined language to emphasize available migration tools and factory support.

  https://learn.microsoft.com/en-us/dynamics365/guidance/migrate/opol-crm-migration-high-level-overview

- **Overview of the Define accounting policies business process area**

  Standardized the naming to “Define accounting policies” and added a new subprocess, “Define fiscal document policies.” Lists were updated to include the new subprocess, with a note that the diagram will be updated later.

  https://learn.microsoft.com/en-us/dynamics365/guidance/business-processes/record-to-report-define-accounting-policies

- **Introduction to the record to report end-to-end business process**

  Added actionable steps for getting started, including links to solution guidance, demos/trials, and an overview. Introduced a Related information section with resources for financial reporting, analytics, community content, and certification to accelerate adoption.

  https://learn.microsoft.com/en-us/dynamics365/guidance/business-processes/record-to-report-introduction

- **Overview of the Manage budgets business process area within the Record to report end-to-end scenario**

  Replaced a numbered list with a clearer, updated bullet list aligned to the latest catalog and noted that the diagram will follow. Clarified decision points and outcomes, including approvals, reservations, transfers, and downstream steps.

  https://learn.microsoft.com/en-us/dynamics365/guidance/business-processes/record-to-report-manage-budgets

- **Overview of the record to report end-to-end business process**

  Streamlined the list of business process areas, adding “Analyze financial performance” and removing areas no longer in scope. Simplified the end-to-end flow to focus on Record to report and corrected the upstream label from Service to cash to Service to deliver.

  https://learn.microsoft.com/en-us/dynamics365/guidance/business-processes/record-to-report-overview

- **Stay current with Dynamics 365 service updates**

  Added concrete guidance for early access through monthly channels, sandbox testing, backups, and automated validation to reduce upgrade risk. Clarified terminology around feature removal/obsolescence and highlighted selecting One Version maintenance windows to fit business schedules.

  https://learn.microsoft.com/en-us/dynamics365/guidance/implementation-guide/service-solution-service-updates

- **Overview of the Service to deliver business process areas**

  Expanded coverage with new sections on “Deliver services” and “Analyze service performance,” detailing execution, tracking, communication, measurement, and quality. Added a reference to the Deliver services overview to guide navigation across the end-to-end process.

  https://learn.microsoft.com/en-us/dynamics365/guidance/business-processes/service-to-cash-areas-overview

- **Overview of Manage Service Work**

  Replaced a short, linear list with a comprehensive hierarchical flow covering Service to deliver, strategy, planning, managing, delivering, and analyzing service work. Introduced detailed sub-steps and updated links to related guidance to help teams implement the full lifecycle.

  https://learn.microsoft.com/en-us/dynamics365/guidance/business-processes/service-to-cash-create-process-service-work

- **Overview of the Manage service assets business process**

  Renamed the process to “Manage service assets” and noted the end-to-end scenario rename and relocation to the Plan service work area. Streamlined the introduction and expanded Next steps with a structured set of links across Plan and Deliver phases.

  https://learn.microsoft.com/en-us/dynamics365/guidance/business-processes/service-to-cash-manage-service-assets

- **Overview of the Plan service work business process area within the Service to deliver end-to-end scenario**

  Reorganized the implementation steps into a hierarchical end-to-end sequence, adding sub-steps for capacity, demand, parts forecasting, contractor planning, and asset management. Included additional links to overviews and related process pages for easier navigation.

  https://learn.microsoft.com/en-us/dynamics365/guidance/business-processes/service-to-cash-manage-service-resources

- **Overview of the Finalize work orders business process within the Service to deliver end-to-end scenario**

  Expanded the Next steps into a full service process flow, including detailed Deliver services tasks such as performing work, updating assets, collecting feedback, and finalizing work orders. Reorganized related links to align with the new structured path.

  https://learn.microsoft.com/en-us/dynamics365/guidance/business-processes/service-to-cash-review-close-service-requests

- **Overview of the Develop procurement and sourcing strategy business process area within the Source to pay end-to-end scenario**

  Added the “Define vendor classifications” subprocess to the strategy list and implementation resources, with a note that the diagram will be updated. This change clarifies governance expectations and enriches the planning scope for sourcing.

  https://learn.microsoft.com/en-us/dynamics365/guidance/business-processes/source-to-pay-define-procurement-sourcing-strategy-overview