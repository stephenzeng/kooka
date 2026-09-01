# Dynamics 365 Field Service
**Date created:** 2026-09-01 UTC  
**Tags:** Best Practices, Configuration, Guidance, Performance, Security  

## Major Changes

- **Dynamics 365 Field Service version history**

  Updated the release schedule to make 8.8.149.301 the next version across stations, including USG and Dedicated Scale Groups timelines. Introduced features that improve usability and clarity, such as hiding financial details on booking cards and adding field-level help for key columns. Enhanced performance with asynchronous bulk booking operations and reduced lookups, and delivered multiple reliability fixes across bookings, products, requirement characteristics, posting flows, localization, and environment analysis checks. Included additional security improvements to strengthen overall platform resilience.

  https://learn.microsoft.com/en-us/dynamics365/field-service/version-history

- **Customization considerations for the work order form**

  Expanded and reorganized customization guidance to make configuring the work order form more predictable and secure, including a tip on using field-level security. Added detailed instructions for the form header and command bar, clarified popup behavior for subgrids, and significantly rewrote the maps control steps with clearer procedures. Introduced a comprehensive “Work order form controls” section with configuration steps, dependencies, and limitations for recap, status, priority, timeline, location/contact/asset/booking/financial cards, products and services, tasks, and references. Added “Work order grid controls” guidance covering grid/action bar applicability, context menu behavior, side pane constraints, and known issues so makers can avoid misconfigurations.

  https://learn.microsoft.com/en-us/dynamics365/field-service/work-order-customization

## Moderate Changes

- **Send frontline workers a download link for the mobile app**

  Updated the email approval and mailbox configuration steps to reflect current navigation and requirements in the Power Platform admin center, including explicit sign-in, environment selection, and corrected privilege paths. Clarified mailbox approval flow (active mailbox selection, approve email, test and enable) and added a new step to set the start date for processing incoming email; images were realigned to match the sequence.

  https://learn.microsoft.com/en-us/dynamics365/field-service/frontline-worker-set-up-email-approval