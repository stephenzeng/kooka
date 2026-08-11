# Microsoft 365 Copilot
**Date created:** 2026-08-05 UTC  
**Tags:** Administration  

## Major Changes

- **Integrate ServiceNow HRSD and ITSM with your Employee Self-Service deployment**

  Updated configuration guidance to use Dataverse environment variables instead of editing template records, centralizing setup and reducing maintenance. Added a reference table of environment variables for the HRSD and ITSM extension packs with example values, and clarified that values should point to the ServiceNow portal root (for example, /sp or /esc). Introduced step-by-step instructions in the Power Platform admin center and noted that these settings persist across updates, with template configuration now serving only as a fallback. This streamlines deployments, minimizes rework after updates, and lowers the risk of configuration drift.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/employee-self-service/servicenow-hrsd-itsm