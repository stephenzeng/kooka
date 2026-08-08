# Power Automate
**Change date:** 2026-08-07 UTC  
**Tags:** Administration  

## Major Changes

- **Install Power Automate**

  Overhauled installation guidance with a clear MSI vs. Microsoft Store comparison (admin rights, update behavior including auto-update from v2.54+, machine runtime inclusion, and silent install support) and clarified non-coexistence, with the exception of Store app plus MSI machine runtime for admins. Updated prerequisites to require the .NET 10 runtime starting with v2.69, added rationale and remediation steps for failed installs, and noted that future versions won’t re-download once the runtime is present. Expanded procedures for both MSI and Store installations, introduced proxy/network readiness tips, and added an “Update Power Automate desktop” section covering auto-updates for Store, configurable updates for MSI 2.54+, and manual updates for older MSI versions, plus guidance to identify the installation type. Added comprehensive troubleshooting for silent failures, error 1603, launch issues, and version mismatches, and clarified lack of support on Windows multi-session with a recommendation for silent deployment to ensure consistency.

  https://learn.microsoft.com/en-us/power-automate/desktop-flows/install