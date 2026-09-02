# Microsoft Agent 365
**Date created:** 2026-09-02 UTC  
**Tags:** Automation, Best Practices, Configuration, Get Started, Guidance, Identity, Security, Troubleshooting

## Major Changes

- **Custom Client App Registration for Agent 365 CLI**

  Expanded guidance separates the Microsoft-managed Agent 365 CLI enterprise application from a tenant-owned custom app, with clear scenarios, cautions, and an updated five-step workflow that begins with running the setup requirements. Updated instructions cover fallback behavior, automatic redirect URI handling, delegated permissions (including beta AgentIdentityBlueprint.* scopes), and two configuration methods via Entra admin center or Graph API. Added a section explaining what the CLI auto-configures for custom apps and reaffirmed that the Microsoft-managed app is only validated, not modified. Clarified wids claim behavior and streamlined troubleshooting to align with the new flow.

  https://learn.microsoft.com/en-us/microsoft-agent-365/developer/custom-client-app-registration

## Moderate Changes

- **Install and Use the Agent 365 CLI**

  Added Microsoft Entra authentication guidance, including use of the Microsoft-managed CLI enterprise application, its client ID, verification steps, behavior around service principals and delegated scopes, and fallback logic to tenant-owned apps with environment-specific sign-in methods. Expanded troubleshooting for common auth errors (such as AADSTS530035 and AADSTS70007) with recommended mitigations and validation of delegated scopes. Clarified section headings without changing core install, update, or uninstall steps.

  https://learn.microsoft.com/en-us/microsoft-agent-365/developer/agent-365-cli

- **Quickstart: Connect an Existing Agent to Agent 365**

  Clarified that setup prefers the Microsoft-managed CLI enterprise application and falls back to a tenant-owned app of the same name, with continued support for a custom client app. Added a link to detailed custom client app registration guidance.

  https://learn.microsoft.com/en-us/microsoft-agent-365/developer/get-started

- **Agent 365 CLI Setup Command Reference**

  Introduced a clear client application selection order: prefer the Microsoft-managed CLI enterprise application, then a tenant-owned “Agent 365 CLI” app, or prompt for/create a custom app as needed. Clarified that for the Microsoft-managed app the CLI verifies service principal presence and delegated scopes without modifying Microsoft’s registration or creating tenant-wide grants, and refined prompts, wids handling for custom apps, config-free setup, and admin consent behavior accordingly.

  https://learn.microsoft.com/en-us/microsoft-agent-365/developer/reference/cli/setup

- **Agent 365 Troubleshooting Guide**

  Added a dedicated section for CLI authentication issues, explaining Entra sign-in behavior, common errors (AADSTS530035, AADSTS70007), fallback to a tenant-owned custom app, required scopes, and recommended fixes such as updating the CLI and using WAM on Windows. Updated the troubleshooting table and strengthened best practices to favor the Microsoft-managed CLI enterprise application or a correctly configured custom client app.

  https://learn.microsoft.com/en-us/microsoft-agent-365/developer/troubleshooting