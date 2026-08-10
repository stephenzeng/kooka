# Microsoft Entra
**Date created:** 2026-07-18 UTC  
**Tags:** Governance, Security  

## Moderate Changes

- **Passkeys by default and retirement of Microsoft-provided SMS and voice authentication**

  Updated the FAQ to confirm that B2B and internal guest users are in scope for the Microsoft-provided SMS/voice retirement, with passkey support for these users planned by end of 2026. The registration campaign steps now reference the Entra ID navigation path instead of Protection, helping admins find the correct settings and plan the guest transition timeline.

  https://learn.microsoft.com/en-us/entra/identity/authentication/concept-sms-voice-retirement

- **System-preferred authentication**

  Added guidance on how Windows Hello for Business and macOS Platform SSO are treated at first-factor sign-in under the Microsoft managed state, including when device-bound passkeys are prompted or skipped and how users can choose another method. Clarified that federated users are excluded from system-preferred at first factor, with applicability limited to second factor, enabling more precise policy planning.

  https://learn.microsoft.com/en-us/entra/identity/authentication/concept-system-preferred-authentication

- **Configure a Microsoft Entra Conditional Access policy for Explicit Forward Proxy**

  Reflected general availability by removing preview labels and disclaimers for Explicit Forward Proxy in Microsoft Entra Internet Access. This signals production readiness without changing existing configuration guidance.

  https://learn.microsoft.com/en-us/entra/global-secure-access/how-to-configure-conditional-access-policy-for-explicit-forward-proxy

- **Configure Explicit Forward Proxy**

  Removed preview markings to indicate the Explicit Forward Proxy feature is now generally available. This affirms enterprise readiness while leaving the setup instructions unchanged.

  https://learn.microsoft.com/en-us/entra/global-secure-access/how-to-configure-explicit-forward-proxy

- **What's new in Microsoft Entra RBAC documentation**

  Added a July 2026 note that the Tenant Governance Administrator role is now classified as a privileged role in the RBAC permissions reference. This elevates the role’s status and may affect governance controls and approval workflows.

  https://learn.microsoft.com/en-us/entra/identity/role-based-access-control/whats-new