# Visual Studio
**Date created:** 2026-07-18 UTC  
**Tags:** AI, Agent, Programming  

## Moderate Changes

- **Use Agent Skills with GitHub Copilot**

  Clarified that the skills panel applies to Insiders builds and refined the creation workflow to choose workspace or personal scope with required name and description. Documented that Visual Studio generates a SKILL.md file following the agentskills.io specification and provides a template to complete.

  https://learn.microsoft.com/en-us/visualstudio/ide/copilot-agent-skills?view=visualstudio

- **Copilot Next Edit Suggestions**

  Updated settings navigation and labels: features moved under Text Editor > Inline Suggestions and providers renamed to Suggestions Providers. Added guidance for the extended-range option to surface suggestions across the current file, clarified default proximity behavior, and revised controls for disabling automatic completions (Invocation) with a new option to collapse suggestions.

  https://learn.microsoft.com/en-us/visualstudio/ide/copilot-next-edit-suggestions?view=visualstudio

- **Obtain build logs with MSBuild**

  Expanded coverage of what the binary logger captures, including diagnostic messages, imported file contents, final property values, item metadata, and task inputs/outputs. Added a performance note recommending enabling the binary logger only when needed, especially for large builds.

  https://learn.microsoft.com/en-us/visualstudio/msbuild/obtaining-build-logs-with-msbuild?view=visualstudio