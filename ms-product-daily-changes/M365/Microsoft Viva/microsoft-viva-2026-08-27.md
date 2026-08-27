# Microsoft Viva
**Date created:** 2026-08-27 UTC  
**Tags:** Best Practices, Compliance, Configuration, Governance, Guidance, Identity, Security  

## Major Changes

- **Delete user data from Viva Glint**

  Overhauled the data deletion guidance to clearly present admin choices and set the default to retain survey responses and identifiable data for deleted users. Introduced a 30‑day soft-delete period with details on reinstatement, removal from distribution lists and surveys, role/permission cleanup, and placeholder assignment for direct reports. Added steps and a link for retroactive user uploads to correctly reflect manager changes in historical data. Streamlined the deletion procedure by simplifying confirmation steps to reduce ambiguity.

  https://learn.microsoft.com/en-us/viva/glint/setup/delete-user-data

- **Manage General Settings in Viva Glint**

  Added a new consolidated control, “Retain survey responses and identifiable data for deleted users,” replacing prior settings and clarifying tenant behavior. Documented soft-delete behavior (30 days), reinstatement requirements, and how raw data exports are handled to align governance with privacy expectations. Noted a temporary pause of Microsoft Entra delete signal processing until September 30, 2026 and mapped prior settings to the new control, including a clear On/Off definition table.

  https://learn.microsoft.com/en-us/viva/glint/setup/manage-general-settings

## Moderate Changes

- **Use Viva Glint's Comments report**

  Updated instructions to enable supported languages in Comment analytics language before submission; otherwise, comments in unsupported languages may not be analyzed. Clarified that Copilot‑enhanced topic assignment is governed by the tenant’s Copilot setting, includes current availability (ad‑hoc and recurring surveys), and added robust privacy/security details with a reminder not to use AI‑generated topics for employment decisions; the FAQ now advises caution when comparing results before and after enablement.

  https://learn.microsoft.com/en-us/viva/glint/reports/comments-report

- **User Roles with custom data access in Viva Glint**

  Clarified that Focus area access applies only to the Focus Area Overview Report and not to viewing focus areas on the dashboard. This reduces confusion about role permissions and helps admins assign the correct access for reporting scenarios.

  https://learn.microsoft.com/en-us/viva/glint/setup/custom-user-role

- **FAQs for deleting user data**

  Aligned FAQs with the new “Retain survey responses and identifiable data for deleted users” control, detailing outcomes when On versus Off. Announced the retirement of deidentification while retaining responses starting September 1, 2026, and provided the pause/resume schedule for Microsoft Entra delete signals with guidance to review user status and request the Deleted users list.

  https://learn.microsoft.com/en-us/viva/glint/setup/delete-user-data-faq

- **Import historical response data in Viva Glint**

  Revised CSV guidance to require quoting only when comments contain commas, line breaks, quotation marks, or other escapable characters. Included a practical example to reduce parsing errors during imports.

  https://learn.microsoft.com/en-us/viva/glint/setup/import-historical-response-data

- **Responding to Data Subject Requests (DSRs) in Viva Glint**

  Expanded deletion lifecycle details, including a 30‑day soft-delete window, reinstatement via HRIS, and effects on distribution lists, surveys, roles, and reporting permissions with placeholder assignment for direct reports. Introduced a streamlined procedure with clear confirmation and verification steps, and noted that reports update based on user data controls.

  https://learn.microsoft.com/en-us/viva/glint/setup/raw-data-request-response

- **Use Viva Glint's People page to view employee information**

  Clarified that DSR or Microsoft Entra delete signals place users in a 30‑day soft-deleted state with permanent deletion afterward per user data controls; reinstatement requires reuploading the user. Documented impacts such as removal from distribution lists and future surveys, role/permission cleanup, and placeholder assignment for direct reports, with guidance to run a retroactive user upload to fix historical manager mapping.

  https://learn.microsoft.com/en-us/viva/glint/setup/viewing-employee-info