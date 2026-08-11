# Azure Monitor
**Date created:** 2026-07-30 UTC  
**Tags:** AI, Agent, Monitoring  

## New Articles

- **Create an Azure Monitor Health Model with the Azure CLI (Preview)**

  Introduced an end-to-end tutorial for building and operating a health model using the Azure CLI health-models extension (preview). Covers environment setup, deploying a sample App Service, enabling a system-assigned managed identity, and assigning Reader permissions. Guides you through defining a metric-based signal (Http4xx thresholds), creating entities, generating traffic, and connecting components. Demonstrates querying metrics and health state/history, adding annotations, ingesting external health reports, and performing cleanup. Includes schema references and next steps to accelerate adoption.

  https://learn.microsoft.com/en-us/azure/azure-monitor/health-models/cli

## Moderate Changes

- **Action groups**

  Clarified OTP verification requirements: Email Azure Resource Manager role addresses no longer require OTP, while standard email recipients must verify (with resend behavior noted) and will not receive alerts if unverified after enforcement. Updated the managed identity support table to show Azure Function support with Function App authorization (Microsoft Entra ID), and marked role fields as N/A where not applicable (ITSM, Secure Webhook, Webhook). These updates help ensure reliable alert delivery and correct authentication configuration.

  https://learn.microsoft.com/en-us/azure/azure-monitor/alerts/action-groups

- **Create Query-Based Metric Alerts (Preview)**

  Expanded and reorganized the how-to with consistent CLI/PowerShell/REST/Bicep/ARM examples, parameterized placeholders, and correct provider/ID casing, plus collapsible JSON payload samples. Added end-to-end deployment steps, clarified portal resource-type selection, and strengthened guidance on managed identities, permissions, PromQL criteria, and for-duration behavior. Improved instructions for viewing fired alerts and managing rules to streamline operations.

  https://learn.microsoft.com/en-us/azure/azure-monitor/alerts/alerts-create-query-based-metric-alerts

- **Mirror Azure Monitor Data in Microsoft Fabric (Preview)**

  Added onboarding via an AI-driven Fabric skill to mirror Azure Monitor data, covering item creation, Eventhouse shortcuts, schema checks, and Operations Agent setup. Included a related link to Skills for Fabric overview to speed discovery and adoption.

  https://learn.microsoft.com/en-us/azure/azure-monitor/fundamentals/monitor-cross-domain-fabric