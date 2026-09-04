# Microsoft Intune
**Date created:** 2026-09-04 UTC  
**Tags:** Configuration  

## Moderate Changes

- **Prerequisites the Microsoft Tunnel VPN for Microsoft Intune**

  Updated the supported Linux distributions to include Red Hat Enterprise Linux (RHEL) 10.2 with Podman 5.8.2 for Microsoft Tunnel deployments. Clarified that admins must manually load the ip_tables kernel module before installing Tunnel and that Podman v3 and earlier are incompatible with Podman 4.2+ container images. These updates help plan compliant deployments and avoid setup issues.

  https://learn.microsoft.com/en-us/intune/device-security/microsoft-tunnel/prerequisites