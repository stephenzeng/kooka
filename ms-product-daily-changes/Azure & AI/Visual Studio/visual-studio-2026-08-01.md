# Visual Studio
**Date created:** 2026-08-01 UTC  
**Tags:** Programming  

## Major Changes

- **VSTest.Console.exe command-line options**

  Reorganized the options overview to highlight the most common switches and streamlined guidance throughout. Expanded platform targeting and framework selection, including additional architectures and support for short TFMs, and enhanced diagnostics and logging options such as Blame crash/hang dumps, trace level control, and LogFilePrefix. Introduced environment variable injection via /Environment and support for response files, while removing deprecated commands to reduce clutter. Added practical guidance on exit codes, escaping TestCaseFilter expressions across shells, recognized environment variables, and refreshed examples to improve reliability and ease of use.

  https://learn.microsoft.com/en-us/visualstudio/test/vstest-console-options?view=visualstudio

## Moderate Changes

- **Configure unit tests with a .runsettings file**

  Added guidance for overriding run settings from the command line for both vstest.console.exe and dotnet test, including syntax after --, precedence over /Settings, and examples for MSTest and TestRunParameters. Provided cross-shell quoting and escaping tips for Command Prompt, PowerShell (including native argument handling and --%), Bash, and zsh, plus an XML example for complex values to help avoid parsing errors.

  https://learn.microsoft.com/en-us/visualstudio/test/configure-unit-tests-by-using-a-dot-runsettings-file?view=visualstudio