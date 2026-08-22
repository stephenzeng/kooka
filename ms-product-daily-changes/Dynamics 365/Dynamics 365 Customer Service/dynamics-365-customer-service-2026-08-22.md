# Dynamics 365 Customer Service
**Date created:** 2026-08-22 UTC  
**Tags:** Automation, Configuration, Guidance  

## New Articles

- **Use the email classification custom action**

  Introduced a new article explaining how to call the msdyn_EmailClassificationCustomAction to classify email records, including prerequisites and detailed request/response schema. Provides guidance on invoking the action from Power Automate with json() parsing, plus HTTP and JSON examples to accelerate implementation. Covers outcome handling (skipped, failed, HTTP errors, permissions) and notes side effects that may retrigger flows, helping teams design resilient automations. Advises against reclassifying emails already handled by built-in classification to avoid conflicts.

  https://learn.microsoft.com/en-us/dynamics365/customer-service/develop/use-email-classification-custom-action

## Major Changes

- **Configure email classification in Customer Service**

  Expanded configuration guidance to support a hierarchical email taxonomy with clearly defined limits and design criteria, enabling consistent categorization at scale. Updated navigation to the Copilot Service admin center and added step-by-step instructions to create categories/subcategories and configure scope rules with a condition builder. Introduced options to run classification on arrival or via custom automation, including invoking the Dataverse action for integrated scenarios. Added a simulation capability to test taxonomy changes against historical emails (with Excel upload and results review), so teams can validate and refine configurations before rollout.

  https://learn.microsoft.com/en-us/dynamics365/customer-service/administer/configure-email-classification