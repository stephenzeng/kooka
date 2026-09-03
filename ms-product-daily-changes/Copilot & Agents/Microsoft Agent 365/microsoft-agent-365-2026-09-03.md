# Microsoft Agent 365
**Date created:** 2026-09-03 UTC  
**Tags:** Configuration, Guidance, Monitoring, Troubleshooting  

## Major Changes

- **Integrate Agent Observability Using Direct OTel**

  Added a tenant eligibility check for S2S integrations to validate licensing and readiness before sending data, including required permissions, token constraints, and clear response handling for common status codes. Clarified ingestion responses so a 200 OK no longer implies routing success; per-span results now indicate sent, rejected, or not_routed with reasons like tenant_not_licensed. Updated guidance directs engineers to evaluate both partialSuccess and results, with refined verification steps to confirm end-to-end delivery. Also clarified URL parameter and encoding requirements and explained outcomes when tenants lack eligibility or licenses.

  https://learn.microsoft.com/en-us/microsoft-agent-365/developer/direct-open-telemetry-integration

## Moderate Changes

- **Troubleshoot Direct OTel Observability**

  Expanded troubleshooting to validate per-span results and understand partialSuccess limitations, adding targeted fixes for tenant_not_licensed and a clearer “No data in Defender” decision path. Added common pitfall resolutions (for example, identity mismatches, invoke_agent requirements, trace/parent IDs, and attribution) and introduced a tenant eligibility preflight with guidance for 200 enabled:false, 403, 429 with Retry-After, and 503 retry handling.

  https://learn.microsoft.com/en-us/microsoft-agent-365/developer/direct-open-telemetry-troubleshooting

- **Agent 365 Observability Data Model and Concepts**

  Introduced optional tenant eligibility preflight guidance for onboarded third-party S2S scenarios and clarified retry behavior for service unavailability. Updated licensing behavior so requests may return 200 OK while spans are marked rejected with tenant_not_licensed, emphasizing that engineers must inspect results and follow the verification flow rather than relying on HTTP status alone.

  https://learn.microsoft.com/en-us/microsoft-agent-365/developer/observability-concepts