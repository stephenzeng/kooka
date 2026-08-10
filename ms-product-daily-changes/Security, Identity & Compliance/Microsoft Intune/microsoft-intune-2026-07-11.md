# Microsoft Intune
**Date created:** 2026-07-11 UTC  
**Tags:** Administration  

## Moderate Changes

- **Troubleshoot co-management: Bootstrap with modern provisioning**

  Updated co-management bootstrap guidance for Windows 11, including verification steps and token validation using CcmAAD.log. Clarified PKI communication requirements and limitations—Autopilot into co-management isn’t supported with PKI certificates—and reinforced that when HTTPS management points are enabled for CMG traffic, a valid client authentication certificate is required, with CRL validation failures being a common cause of errors. Removed outdated Windows 10/UI guidance and legacy DNS assumptions, and streamlined notes on randomized automatic enrollment timing.

  https://learn.microsoft.com/en-us/troubleshoot/mem/intune/comanage-configmgr/troubleshoot-co-management-bootstrap