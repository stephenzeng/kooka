# Microsoft Intune
**Date created:** 2026-08-07 UTC  
**Tags:** Administration, Security  

## Moderate Changes

- **Microsoft Intune licensing**

  Added guidance for device-only subscriptions with a new section on device-only management scenarios. Clarified that device-targeted policies, apps, and actions continue to apply even when a signed-in user lacks an Intune user license, enabling shared and no-user-affinity deployments without interruption.

  https://learn.microsoft.com/en-us/intune/fundamentals/licensing

- **Use Multi Admin Approval with the Microsoft Graph API**

  Updated MAA behavior for app-auth Graph calls: requests missing approval headers now return HTTP 400, and approval handshakes return HTTP 412 with details in the error payload. Clarified that HTTP 412 plus the x-msft-approval-code header indicates the approval request was created. Added guidance to store the original method, URL, and body with the approval code to resubmit the same request after approval.

  https://learn.microsoft.com/en-us/intune/fundamentals/role-based-access-control/multi-admin-approval-graph-api

- **Prerequisites the Microsoft Tunnel VPN for Microsoft Intune**

  Expanded supported platforms to include RHEL 9.8 with Podman 5.8.2+ and noted the need to manually load the ip_tables kernel module. Reiterated Podman container compatibility limits, advising creation of new containers and reinstallation of Microsoft Tunnel when moving from older Podman versions.

  https://learn.microsoft.com/en-us/intune/device-security/microsoft-tunnel/prerequisites

- **Microsoft Intune Protected Apps**

  Removed the Klaxoon for Intune entry from the protected apps list. Admins should review app protection policies and catalogs to ensure deployments and user access are adjusted accordingly.

  https://learn.microsoft.com/en-us/intune/app-management/ref-protected-apps

- **Device Action: Sync**

  Clarified that compliance policy evaluation is no longer part of on-demand device sync operations. Noted that the new device sync experience requires enabling the “Preview new device view” in the Intune admin console, and that the described behavior currently applies to Windows devices.

  https://learn.microsoft.com/en-us/intune/device-management/actions/sync