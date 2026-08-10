# Microsoft Entra
**Date created:** 2026-07-22 UTC  
**Tags:** Administration, Governance, Security  

## Major Changes

- **CSS reference guide for customizing company branding**
  Announced deprecation of custom CSS positioning and related properties in Microsoft Entra ID company branding as part of the Secure Future Initiative. Added a phased timeline: after July 21, 2026, new use of these properties is blocked, followed by global deprecation and eventual retirement of custom CSS. Documented the affected properties and provided step-by-step guidance to audit, export, and update configurations using Microsoft Graph Explorer, the tenant branding inspector tool, and the Entra admin center. This helps tenants proactively remove risky CSS and maintain reliable sign-in experiences.
  https://learn.microsoft.com/en-us/entra/fundamentals/reference-company-branding-css-template

- **Customize the sign-in experience for your application with branding themes**
  Added an IMPORTANT notice signaling the retirement of custom CSS positioning properties in branding themes, including restrictions for new use after July 21, 2026, and a subsequent global deprecation leading to full retirement. Linked to the CSS template guide and a related blog post to help admins identify deprecated properties and plan remediation. This change improves security and consistency across sign-in experiences and calls for updating any themes that rely on these properties.
  https://learn.microsoft.com/en-us/entra/fundamentals/how-to-customize-branding-themes-apps

## Moderate Changes

- **Add company branding to your organization's sign-in page**
  Added an IMPORTANT deprecation notice for custom CSS positioning properties in company branding, outlining restrictions after July 21, 2026 and the later global retirement. Provided guidance to remove these properties and references to the CSS template guide and a related blog post so admins can update branding safely.
  https://learn.microsoft.com/en-us/entra/fundamentals/how-to-customize-branding

- **Passkeys by default and retirement of Microsoft-provided SMS and voice authentication**
  Added a new FAQ clarifying that external MFA methods aren't affected; only Microsoft-provided SMS and voice method policies and legacy MFA policies are retiring. Noted that on September 1, 2026, users enabled for SMS or voice will be auto-enabled for passkeys and prompted to register, while external MFA users remain out of scope unless they’re also enabled for SMS or voice.
  https://learn.microsoft.com/en-us/entra/identity/authentication/concept-sms-voice-retirement

- **Assign Azure Role-based access control (RBAC) Roles - Entitlement management**
  Removed the “(Preview)” label throughout to reflect general availability, including title, headings, and UI references. No procedural changes were made.
  https://learn.microsoft.com/en-us/entra/id-governance/entitlement-management-azure-role-assignments

- **Turn on universal tenant restrictions**
  Reorganized content to clarify where and how tenant restrictions are evaluated, splitting scenarios for Microsoft Entra ID and Microsoft Graph and explaining token replay blocking. Streamlined the enablement steps and consolidated validation into a single flow using My Apps with the Global Secure Access client, improving setup clarity and user guidance.
  https://learn.microsoft.com/en-us/entra/global-secure-access/how-to-universal-tenant-restrictions

- **Administrative relationships in Microsoft Entra Agent ID (Owners, sponsors, and managers)**
  Clarified the difference between sponsors for an agent’s user account versus the agent identity, blueprint, and blueprint principal, noting user sponsorship is primarily for B2B guests. Recommended designating the agent identity sponsor as the primary responsible party when both objects exist, and provided guidance on aligning sponsors and using access packages for access requests on behalf of the sponsored identity.
  https://learn.microsoft.com/en-us/entra/agent-id/agent-owners-sponsors-managers

- **How to configure Global Secure Access web content filtering**
  Simplified and standardized source traffic type filtering, consolidating multiple categories into two and updating terminology across tables, notes, and examples. Guidance and examples were refreshed to clearly differentiate agent traffic from user/non-agent traffic, including scenarios such as blocking AI agents while allowing user traffic.
  https://learn.microsoft.com/en-us/entra/global-secure-access/how-to-configure-web-content-filtering