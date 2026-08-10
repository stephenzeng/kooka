# Power Apps
**Date created:** 2026-07-16 UTC  
**Tags:** Agent, AI, Programming  

## Moderate Changes

- **Analyze plug-in performance**
  Clarified that the 2-minute Dataverse operation time limit applies to both synchronous and asynchronous plug-ins, ensuring consistent performance expectations. Updated guidance recommends using asynchronous execution for plug-ins that take more than 2 seconds, helping improve reliability and user experience.  
  https://learn.microsoft.com/en-us/power-apps/developer/data-platform/analyze-performance

- **Customize Microsoft 365 Copilot with an agent**
  Expanded and aligned content to Microsoft 365 Copilot terminology, added a new “Set a default agent” section to make a custom agent the starting experience in the side pane, and removed redundant sections. Enhanced Xrm.Copilot API documentation to highlight bidirectional interactions with the side pane (including sendPromptToM365Copilot, openM365CopilotPanel, updateContext (preview), getCurrentAgent, and addActionHandler), with updated examples for clearer implementation.  
  https://learn.microsoft.com/en-us/power-apps/maker/model-driven-apps/customize-microsoft-365-copilot-chat