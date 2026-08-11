# Visual Studio
**Date created:** 2026-08-06 UTC  
**Tags:** Programming  

## Moderate Changes

- **Colors and Styling for Visual Studio**

  Updated guidance on customizing Fluent theme color tokens via the Theme colors options, including per-theme persistence and per-token reset. Advised extension authors to bind UI to VSColor or ThemeResourceKey tokens and validate under non-default tokens to avoid hardcoded colors. Added support for sharing overrides through theme-named JSON files and clarified when to use Fonts and Colors vs. Theme colors.

  https://learn.microsoft.com/en-us/visualstudio/extensibility/ux-guidelines/colors-and-styling-for-visual-studio?view=visualstudio

- **Modernize Visual Studio theme colors**

  Added coverage of new Fluent semantic tokens to enable more granular styling of shell areas like tab and window headers. Introduced a section on the Theme colors options page with live customization, per-theme persistence, reset behavior, and instructions for sharing overrides via theme-named JSON files.

  https://learn.microsoft.com/en-us/visualstudio/extensibility/migration/modernize-theme-colors?view=visualstudio

- **Visual Studio Theme Color Tokens**

  Documented the in-product Theme colors page, including access path, live application of changes, per-token reset, and per-theme persistence. Added guidance for sharing overrides via theme-named JSON files and noted the addition of more Fluent tokens as shell areas become more granular.

  https://learn.microsoft.com/en-us/visualstudio/extensibility/ux-guidelines/theme-color-token-reference?view=visualstudio

- **VSIX Color Editor**

  Clarified when to use the built-in Theme colors options versus the VSIX Color Editor, highlighting live-apply behavior, per-theme persistence, and per-token reset. Documented how to share theme overrides using theme-named JSON files applied after restart.

  https://learn.microsoft.com/en-us/visualstudio/extensibility/internals/vsix-color-editor?view=visualstudio