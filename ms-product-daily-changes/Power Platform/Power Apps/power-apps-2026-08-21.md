# Power Apps
**Date created:** 2026-08-21 UTC  
**Tags:** Configuration, Get Started, Guidance  

## Major Changes

- **How to: Connect your code app to data**

  The article was retitled and comprehensively rewritten to center on the Power Apps CLI (pa) instead of PAC CLI and portal-based steps. It now provides end-to-end CLI workflows for creating connections, adding both tabular and non-tabular data sources, refreshing data sources, and working with connection references using updated command syntax. Guidance consolidates discovery of datasets, tables, and stored procedures via list-* commands and updates SQL and SharePoint examples. These changes streamline setup, standardize command usage, and make automation and repeatable deployments easier.

  https://learn.microsoft.com/en-us/power-apps/developer/code-apps/how-to/connect-to-data

- **How to: Create a Connection from the Power Apps CLI**

  The article was refocused into a concise how-to that shows how to discover connectors and create a connection using the Power Apps CLI. It adds prerequisites, clear step-by-step commands, search and JSON output options, and explains interactive pagination behavior. By removing broader management and data-source content, the page makes it faster for developers to complete the core task of creating connections with reliable, scriptable commands.

  https://learn.microsoft.com/en-us/power-apps/developer/code-apps/how-to/create-connection

## Moderate Changes

- **Power Apps CLI command reference**

  Expanded reference details for pa connection create with a full parameters table, aliases, required flags, examples, and output including the returned connection ID. Added output behavior and examples for pa connector list, covering interactive pagination, default columns, JSON fields, and search and JSON output options. These enhancements improve clarity and make it easier to script and validate CLI operations.

  https://learn.microsoft.com/en-us/power-apps/developer/code-apps/reference/cli