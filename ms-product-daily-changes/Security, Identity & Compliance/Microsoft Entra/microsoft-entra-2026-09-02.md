# Microsoft Entra
**Date created:** 2026-09-02 UTC  
**Tags:** Configuration, Guidance, Identity, Security, Troubleshooting  

## New Articles

- **Configure TLS inspection with a Microsoft-managed certificate**

  Introduced preview support to configure TLS inspection using a Microsoft-managed, tenant-specific root CA for Microsoft Entra Internet Access. The article provides step-by-step setup in the admin center, including creating the managed certificate and deploying the public root CA to client devices (for example, via Intune). It explains how to enable the certificate for TLS inspection and manage lifecycle actions such as enable, disable, delete, and rotation. Links to related configuration and troubleshooting guidance help streamline rollout and maintenance.

  https://learn.microsoft.com/en-us/entra/global-secure-access/how-to-transport-layer-security-settings-managed-certificate

## Moderate Changes

- **Protect enterprise generative AI apps with prompt injection protection**

  Clarified TLS inspection setup by directing admins to choose either a Microsoft-managed certificate or a customer-managed certificate before configuring inspection policies. This guidance makes the options and step sequence explicit, reducing misconfiguration and improving deployment reliability.

  https://learn.microsoft.com/en-us/entra/global-secure-access/how-to-ai-prompt-injection-protection

- **Configure Transport Layer Security Inspection Policies**

  Updated prerequisites to require an active, enabled certificate authority and added clear guidance to configure either a Microsoft-managed or customer-managed certificate, with direct links to both. Related content was split into targeted articles for each certificate option, streamlining navigation and setup.

  https://learn.microsoft.com/en-us/entra/global-secure-access/how-to-transport-layer-security

- **Configure TLS inspection with your own certificate**

  Retitled and refocused the article on bring-your-own-certificate, adding step-by-step instructions to create a CSR, sign it with a CA, and upload the signed certificate and chain. Added a self-signed root CA testing path with OpenSSL (including a sample configuration and commands) and an instructional video summarizing setup steps. Reorganized examples and cross-links to improve discoverability and point to the Microsoft-managed certificate alternative.

  https://learn.microsoft.com/en-us/entra/global-secure-access/how-to-transport-layer-security-settings

- **Troubleshoot Microsoft Entra hybrid joined devices**

  Expanded guidance for error AADSTS50034, noting it can appear as STATUS_ACCOUNT_DISABLED on Windows clients when the client sends a SAM account name instead of a UPN to the Entra STS. The update highlights that this often coincides with loss of communication to on-prem domain controllers in hybrid environments and doesn’t impact Entra-native deployments.

  https://learn.microsoft.com/en-us/entra/identity/devices/troubleshoot-hybrid-join-windows-current