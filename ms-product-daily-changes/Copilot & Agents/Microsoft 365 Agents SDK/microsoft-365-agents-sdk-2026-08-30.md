# Microsoft 365 Agents SDK
**Date created:** 2026-08-30 UTC  
**Tags:** Best Practices, Configuration, Guidance, Security  

## New Articles

- **Secure your agent for production**

  Introduced a comprehensive production hardening guide for Microsoft 365 Agents SDK. Details defense-in-depth controls including inbound JWT validation, caller authorization with allow lists, service URL validation, and an outbound host allow list to mitigate SSRF and token exfiltration. Provides step-by-step, language-specific setup for Python (FastAPI/aiohttp), Node.js (Express), and .NET (ASP.NET), covering middleware/decorators, configuration, pipeline ordering, and OutboundHostValidator usage. Clarifies issuer/audience checks, tenant and sovereign cloud settings, serviceUrl claim validation, and Microsoft host suffix defaults, with guidance on toggling features for dev vs. production. Includes a consolidated security checklist and links to authentication configuration to help teams ship secure agents faster.

  https://learn.microsoft.com/en-us/microsoft-365/agents-sdk/secure-your-agent