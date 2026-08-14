# Visual Studio
**Date created:** 2026-08-14 UTC  
**Tags:** Best Practices, Configuration, Guidance  

## Moderate Changes

- **Visual Studio Theme Color Tokens**

  Expanded guidance on customizing Fluent theme color tokens, including a new “Edit theme colors” command and a searchable grid showing tokens for the active theme. Clarified immediate application of changes, per-token reset, and per-theme overrides that persist across theme switches, along with areas affected such as editor colors, tool windows, and shell chrome. Updated sharing guidance to require theme-matching JSON filenames and noted that overrides apply after restarting Visual Studio.

  https://learn.microsoft.com/en-us/visualstudio/extensibility/ux-guidelines/theme-color-token-reference?view=visualstudio

- **VSIX Color Editor**

  Updated guidance on when to use the VSIX Color Editor for authoring and distributing theme resources versus using in-IDE personal overrides via the “Edit theme colors” command. Clarified that personal overrides take precedence over theme values and added recommended testing steps (adjust tokens, switch themes, reset) to ensure readability and usability, with a reference to the theme color tokens documentation.

  https://learn.microsoft.com/en-us/visualstudio/extensibility/internals/vsix-color-editor?view=visualstudio