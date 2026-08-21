# Microsoft Viva
**Date created:** 2026-08-21 UTC  
**Tags:** Configuration, Guidance  

## Major Changes

- **Microsoft 365 Organizational Data Service - Attribute reference**

  Introduced two new attributes for organizational data: Microsoft_DotLineManagersEmailAndLabel and Microsoft_AssistantsEmail, and mapped them to relevant colleagues relationships for app scenarios. Updated data quality and schema guidance, including changing Microsoft_HourlyRate to Double and refining Microsoft_SupervisorIndicator values (IC/Mngr/Mngr+). Tightened constraints for Microsoft_GlintEmploymentStatus (ACTIVE/INACTIVE only) and expanded Microsoft_HireDate guidance to handle multiple hire dates and Viva Glint tenure derivation. These updates improve modeling of matrix management, assistant relationships, and data consistency across apps.

  https://learn.microsoft.com/en-us/viva/orgdata-attributes

## Moderate Changes

- **Import organizational data from SAP SuccessFactors**

  Updated field mappings to use emailTypeNav.externalCode == 'B' for Microsoft_PersonEmail and Microsoft_ManagerEmail, improving accuracy over the previous emailType == '8448' reference. Added a mapping for Microsoft_DotLineManagersEmailAndLabel to capture and label matrix (dot-line) manager emails, enabling richer organizational relationship imports.

  https://learn.microsoft.com/en-us/viva/import-org-data-success-factors

- **Import organizational data from Workday**

  Expanded the Workday-to-Microsoft 365 mapping to support matrix (dot-line) managers through a new Microsoft_DotLineManagersEmailAndLabel field. Added a source mapping (ExternalSource_DotLineManagersIdAndLabel) to read Matrix Management Chain data and compose labeled relationships, enabling import and identification of dot-line manager connections.

  https://learn.microsoft.com/en-us/viva/import-org-data-workday