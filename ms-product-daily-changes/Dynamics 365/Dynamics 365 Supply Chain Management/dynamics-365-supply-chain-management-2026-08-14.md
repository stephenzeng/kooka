# Dynamics 365 Supply Chain Management
**Date created:** 2026-08-14 UTC  
**Tags:** Configuration, Troubleshooting  

## New Articles

- **Purchase Requisition "You Are Not Set Up as an Employee" Error**

  Introduced troubleshooting guidance for the purchase requisition error indicating the user isn’t set up as an employee. Clarifies that the issue stems from the user account not being linked to an active worker record (Person/party) in the correct legal entity. Provides step-by-step checks to verify or create the worker, ensure active employment, and link the user’s Person field. This helps administrators quickly resolve access issues and restore requisition creation.

  https://learn.microsoft.com/en-us/troubleshoot/dynamics-365/supply-chain/procurement/purchase-requisition-employee-not-linked

- **Summary Update Error Blocks Direct Delivery Invoice Posting**

  Added troubleshooting for direct delivery scenarios where invoice posting fails due to incorrect posting sequence and Accounts receivable Summary update settings. Explains the correct order: post the product receipt on the purchase order to auto-post the sales order packing slip, then invoice the sales order. Includes procedures to adjust Summary update parameters (matching criteria, split by invoice site or delivery information) and notes when to override Summary update to None. These adjustments prevent aggregation issues and ensure invoices post successfully.

  https://learn.microsoft.com/en-us/troubleshoot/dynamics-365/supply-chain/procurement/summary-update-error-direct-delivery-po-invoice