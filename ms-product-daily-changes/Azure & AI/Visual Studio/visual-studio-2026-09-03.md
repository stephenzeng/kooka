# Visual Studio
**Date created:** 2026-09-03 UTC  
**Tags:** Guidance, Troubleshooting  

## Moderate Changes

- **Developer Community guidelines**

  Added a new section with step-by-step instructions for changing your Developer Community display name via Profile and Preferences. Clarifies the navigation path and includes a UI screenshot to reduce confusion and speed profile updates.

  https://learn.microsoft.com/en-us/visualstudio/ide/developer-community-guidelines?view=visualstudio

- **Create a pull request in Visual Studio**

  Updated guidance to open pull requests in dedicated tabs for easier multitasking across multiple PRs. Documented attaching a Git branch as Copilot Chat context directly from the Git Repository window and noted emoji reactions support in PR comments for GitHub and Azure DevOps to improve collaboration.

  https://learn.microsoft.com/en-us/visualstudio/version-control/git-create-pull-request?view=visualstudio

- **MSB3821 diagnostic code**

  Added troubleshooting for projects on virtual disks (such as Dev Drive backed by .vhd/.vhdx) marked with the internet zone, which can trigger MSB3821. Explains unblocking the backing virtual disk file via File Properties or the Unblock-File PowerShell cmdlet to restore normal builds.

  https://learn.microsoft.com/en-us/visualstudio/msbuild/errors/msb3821?view=visualstudio

- **What is GitHub Copilot Chat for Visual Studio?**

  Documented how to add a Git branch as chat context from the Git Repository window using Add to Chat. This improves response relevance and streamlines Copilot Chat workflows when discussing code changes tied to a branch.

  https://learn.microsoft.com/en-us/visualstudio/ide/visual-studio-github-copilot-chat?view=visualstudio