# Visual Studio
**Date created:** 2026-09-05 UTC  
**Tags:** Automation, Configuration, Guidance  

## Major Changes

- **Browse Git repositories and compare branches in Visual Studio**

  Expanded pull request review with options to open PRs in a dedicated tab, view timeline updates, and react to comments with emojis, improving review flow and feedback. Added the ability to set PRs to autocomplete or auto-merge after required checks and approvals, streamlining merges. Introduced procedures to compare a file with the working tree from file history for faster diagnostics. Added guidance on reviewing commits with GitHub Copilot, including inline comments, supported repository types, and how to enable the feature in settings.

  https://learn.microsoft.com/en-us/visualstudio/version-control/git-browse-repository?view=visualstudio

## Moderate Changes

- **Use Agent Skills with GitHub Copilot**

  Added guidance on built-in .NET and Azure skills that ship with corresponding workloads, noting they are disabled by default. Explained how to review and manage skills in the Copilot Chat tool picker, including viewing descriptions, file paths, and inspecting files/folders, with recommendations to enable only what’s relevant and links to the skills repositories.

  https://learn.microsoft.com/en-us/visualstudio/ide/copilot-agent-skills?view=visualstudio

- **Customize chat responses**

  Introduced the Review Selection Copilot Action that provides inline review comments and suggested fixes for selected code. Updated behavior details and usage steps so developers can apply inline feedback efficiently without opening the full chat for certain actions.

  https://learn.microsoft.com/en-us/visualstudio/ide/copilot-chat-context?view=visualstudio

- **Create a pull request in Visual Studio**

  Updated guidance to open PRs in a dedicated tab, track updates via the Overview timeline, and configure autocomplete/auto-merge once approvals and policies are satisfied in both GitHub and Azure DevOps. Clarified how to add and remove emoji reactions in a dedicated subsection to streamline feedback.

  https://learn.microsoft.com/en-us/visualstudio/version-control/git-create-pull-request?view=visualstudio

- **Make a Git commit in Visual Studio**

  Expanded instructions for using Copilot Chat to review uncommitted local changes and provided links for reviewing a selected block, a single commit, or a commit range. This helps catch issues earlier and refine changes before committing.

  https://learn.microsoft.com/en-us/visualstudio/version-control/git-make-commit?view=visualstudio