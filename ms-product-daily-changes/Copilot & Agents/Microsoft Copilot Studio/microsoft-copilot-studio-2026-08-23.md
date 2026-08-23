# Microsoft Copilot Studio
**Date created:** 2026-08-23 UTC  
**Tags:** Configuration, Governance, Guidance, Security  

## New Articles

- **Bypass connector consent cards for an agent**

  Added a how-to article for administrators to bypass connector consent cards for a specific agent using the Power Platform API and PowerShell. It outlines prerequisites (required roles and the CopilotStudio.AdminActions.Invoke delegated permission), one-time tenant setup (Microsoft Entra app registration, API permissions, role assignments), and step-by-step operations to locate environment and agent IDs, adjust execution policy, authenticate, and read or set the bypass state. The article includes a reusable PowerShell script that handles REST calls, header construction, and error handling, along with troubleshooting guidance. This enables automated deployments and governance scenarios where interactive consent prompts would otherwise block execution.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/admin-connector-consent-bypass

## Moderate Changes

- **Use a classic chatbot as an Azure Bot Service skill in an Azure Bot Service bot**

  Clarified that the Azure Bot Service skill integration applies only to classic chatbots. Copilot Studio agents using the standard or GitHub Copilot harness aren’t supported for this capability, helping prevent misconfiguration and set accurate architecture expectations.

  https://learn.microsoft.com/en-us/microsoft-copilot-studio/advanced-use-pva-as-a-skill