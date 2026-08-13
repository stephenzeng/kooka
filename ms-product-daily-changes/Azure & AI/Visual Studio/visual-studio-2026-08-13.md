# Visual Studio
**Date created:** 2026-08-13 UTC  
**Tags:** Best Practices, Compliance, Configuration, Consumption, Guidance, Monitoring, Performance, Security  

## New Articles

- **Microsoft.CodeCoverage.Console telemetry**

  Introduced documentation detailing telemetry for dotnet-coverage and Microsoft.CodeCoverage.Console, covering what data is collected and how it’s handled to support transparency and compliance. Explained how to disable telemetry via DOTNET_COVERAGE_TELEMETRY_OPTOUT and DOTNET_CLI_TELEMETRY_OPTOUT, and how to suppress first-run disclosure with DOTNET_COVERAGE_NOLOGO. Clarified that no personal data or code content is collected and that data is transmitted via Azure Monitor, with examples of collected points such as tool/version, OS/architecture, runtime, CI usage, partial IP, timestamps, command/options usage, output format, log level, and timeout. Included context on Application Insights correlation and links for further reference.

  https://learn.microsoft.com/en-us/visualstudio/test/microsoft-code-coverage-console-tool-telemetry?view=visualstudio

## Moderate Changes

- **GitHub Copilot usage and models**

  Updated guidance for managing and using Copilot models in Visual Studio, including pinning in the model picker, a new model management view, and adding custom models from supported providers using API keys. Added instructions to monitor context window usage with a donut indicator and suggested actions as limits approach. Clarified “thinking effort” configuration, its impact on cost and response time, and when to adjust it for complex versus simple prompts.

  https://learn.microsoft.com/en-us/visualstudio/ide/copilot-usage-and-models?view=visualstudio

- **Secure MSBuild usage best practices**

  Added guidance noting that MSBuild’s use of machine-wide named pipes and mutexes on Windows can be blocked by other local accounts, causing a denial-of-service risk (not data access). Recommended running on trusted machines or using isolated sessions, containers, or VMs to mitigate availability issues.

  https://learn.microsoft.com/en-us/visualstudio/msbuild/msbuild-security-best-practices?view=visualstudio