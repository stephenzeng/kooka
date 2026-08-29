# Microsoft Defender for Cloud Apps
**Date created:** 2026-08-29 UTC  
**Tags:** Compliance, Configuration, Governance, Guidance, Troubleshooting  

## Major Changes

- **Migrate file policies to Microsoft Purview**

  Added comprehensive guidance to migrate Defender for Cloud Apps DLP file policies to Microsoft Purview using the DLP-to-Purview migration tool. The article details prerequisites, supported scopes (SharePoint and OneDrive), and a step-by-step wizard to select policies, review payloads, track progress, and finalize results, with instructions to validate in Purview before disabling originals. It also includes FAQs, known issues, and workarounds to help admins plan and troubleshoot migrations. For non-Microsoft connected apps (Box, Dropbox, Google Workspace, Salesforce in preview), it clarifies requirements and limitations and directs admins to manually recreate these policies since the tool does not migrate them yet.

  https://learn.microsoft.com/en-us/defender-cloud-apps/migrate-file-policies-to-purview

## Moderate Changes

- **Conditional Access app control known limitations | Microsoft Defender for Cloud Apps**

  Documented a limitation where launching Microsoft Teams or Teams-integrated features from a proxied Google Workspace (Gmail) session may fail due to separate authentication contexts not preserved by the session proxy. Advises users to open Microsoft Teams directly rather than from within the proxied Gmail session to avoid disruptions.

  https://learn.microsoft.com/en-us/defender-cloud-apps/caac-known-issues