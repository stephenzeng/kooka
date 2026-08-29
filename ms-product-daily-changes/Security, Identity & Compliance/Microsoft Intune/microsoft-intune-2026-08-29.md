# Microsoft Intune
**Date created:** 2026-08-29 UTC  
**Tags:** Configuration  

## Moderate Changes

- **Prerequisites the Microsoft Tunnel VPN for Microsoft Intune**

  Updated supported Linux distributions to include Red Hat Enterprise Linux (RHEL) 10.1 with Podman 5.8.2 (default). Clarified that RHEL 10.1 requires manually loading the ip_tables kernel module before installing Microsoft Tunnel, and noted incompatibility between containers created with Podman v3 or earlier and Podman v4.2 or later, recommending creating new containers and reinstalling Microsoft Tunnel during upgrades.

  https://learn.microsoft.com/en-us/intune/device-security/microsoft-tunnel/prerequisites