# Dynamics 365 Field Service
**Date created:** 2026-08-27 UTC  
**Tags:** Best Practices, Configuration, Guidance, Troubleshooting  

## New Articles

- **Configure service account requirements for work orders**

  Introduced a new how-to that lets admins control whether the Service Account field is required by Work Order Type. The article explains when to require a Service Account versus when to allow accountless work orders and provides step-by-step setup instructions. It highlights downstream implications for billing, territory, tax, instructions, customer assets, and agreements/entitlements. It also includes troubleshooting for save failures, missing account-derived fields, and integration behaviors, with links to related creation guides and APIs.

  https://learn.microsoft.com/en-us/dynamics365/field-service/configure-service-account-requirements-work-orders

## Moderate Changes

- **Create and manage customer accounts in Field Service**

  Clarified when work orders can be created without a Service Account and how that choice affects defaults such as service location, billing, price list, tax, territory, travel charges, work hours, and instructions. Added guidance on account-based service processes and linked to configuration for controlling Service Account requirements by Work Order Type.

  https://learn.microsoft.com/en-us/dynamics365/field-service/accounts

- **Create a work order**

  Updated creation steps so the Service Account field is conditionally required based on the selected Work Order Type. Added tips for B2C, internal maintenance, and project-centered scenarios, with a link to configure Service Account requirements.

  https://learn.microsoft.com/en-us/dynamics365/field-service/create-work-order

- **Create work orders using the Dataverse Web API**

  Clarified prerequisites by making Service Account and Price List conditional on Work Order Type and process needs. Added an HTTP example that creates a work order without a Service Account and updated error handling to reflect conditional requirements and validation.

  https://learn.microsoft.com/en-us/dynamics365/field-service/create-work-order-api-example

- **Create work orders using Power Automate**

  Refined guidance so Service Account is optional when allowed by the Work Order Type and process. Updated the HTTP-trigger schema and examples to make serviceAccountId optional and adjusted mappings to set Service Account only when provided, with context on when to leave it blank.

  https://learn.microsoft.com/en-us/dynamics365/field-service/create-work-order-flow

- **Create work orders from an agreement**

  Added guidance to validate agreement and booking setup when a Work Order Type does not require a Service Account. Introduced troubleshooting for missing account-derived details on generated work orders and linked to configuration for Service Account requirements.

  https://learn.microsoft.com/en-us/dynamics365/field-service/create-work-order-from-agreement

- **Create a work order from a case**

  Clarified that whether the Service Account is populated or required depends on the selected Work Order Type and available account context. Added a note for contact-centered cases to verify service address, functional location, billing, price list, and other required details when creating work orders without a Service Account.

  https://learn.microsoft.com/en-us/dynamics365/field-service/create-work-order-from-case

- **Create a work order type**

  Added options and recommendations for requiring a Service Account by Work Order Type, including when to rely on account-derived context versus other records. Expanded guidance on price list and related defaults when Service Account is not required, with a link to configuration steps.

  https://learn.microsoft.com/en-us/dynamics365/field-service/create-work-order-types

- **Work order architecture**

  Expanded guidance on how Service Account inheritance provides service address, territory, billing, tax, and instructions, and how admins can require Service Account by Work Order Type. Emphasized maintaining service context across assets and outlined alternatives—such as functional location, contact, or project—when Service Account isn’t used.

  https://learn.microsoft.com/en-us/dynamics365/field-service/field-service-architecture

- **Create a work order using the finance and operations integration**

  Introduced the required Owning Company field for work orders and described how it auto-populates from Service Account, Billing Account, Project, or single-company access. Replaced service-account-based filtering with company-based filtering for related records and clarified alignment requirements, including scenarios without a Service Account and behavior for agreements.

  https://learn.microsoft.com/en-us/dynamics365/field-service/finance-operations-integration-create-wo