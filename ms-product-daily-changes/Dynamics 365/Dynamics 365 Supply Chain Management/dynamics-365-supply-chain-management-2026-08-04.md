# Dynamics 365 Supply Chain Management
**Date created:** 2026-08-04 UTC  
**Tags:** Administration  

## New Articles

- **Source Document Line Error During PO Confirmation**

  Introduced a new troubleshooting guide for purchase order confirmations that fail with “Cannot create a record in Source document line (SourceDocumentLineTmpJournalize). The record already exists.” The article outlines symptoms and provides a clear resolution path using System administration > Periodic tasks > Consistency check with targeted settings for Purchase order. It instructs enabling Fix error, using a from date before the PO was created, selecting Purchase order accounting distributions, and then re-confirming the PO. This helps admins quickly remediate blocked confirmations and restore procurement workflows.

  https://learn.microsoft.com/en-us/troubleshoot/dynamics-365/supply-chain/procurement/cannot-create-record-sourcedocumentline

## Moderate Changes

- **Configure Supplier Engagement elements in Power Platform (preview)**

  Streamlined guidance by removing the section on configuring supplier portal sign-in and onboarding URLs, including steps for setting the Supplier Portal URL via Power Apps environment variables and related validation. Users should follow current configuration guidance elsewhere in the documentation; no other substantive updates were made.

  https://learn.microsoft.com/en-us/dynamics365/supply-chain/supplier-engagement/deploy-configure-power-platform