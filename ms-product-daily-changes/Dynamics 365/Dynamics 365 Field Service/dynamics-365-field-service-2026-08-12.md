# Dynamics 365 Field Service
**Date created:** 2026-08-12 UTC  
**Tags:** Billing, Configuration, Guidance, Governance  

## Major Changes

- **Configure travel charges**

  Updated guidance clarifies how Field Service applies and calculates travel charges after a qualifying booking is completed. It explains that the selected Travel Charge Item is added to the work order, using the service account’s Travel Charge as the unit price and the Travel Charge Type (Hourly, Mileage, Fixed) to determine quantity, with one charge item per qualifying booking and standard pricing, discounts, and taxes applied. A new configuration section provides step-by-step setup for Travel Charge Type and Travel Charge on service accounts. An example table illustrates calculation outcomes across charge types, and images were refreshed for accuracy.

  https://learn.microsoft.com/en-us/dynamics365/field-service/travel-charges

## Moderate Changes

- **Set up the mobile offline profile**

  Added instructions for moving a mobile offline profile between environments using solutions, including adding the profile to a solution, exporting it, importing into the target environment, and verifying results. The update also notes that publishing profile changes creates an active solution layer and recommends reviewing solution management and layering strategy.

  https://learn.microsoft.com/en-us/dynamics365/field-service/mobile/set-up-offline-profile