# SQL Server
**Date created:** 2026-08-29 UTC  
**Tags:** Configuration, Guidance, Identity, Security, Troubleshooting  

## Major Changes

- **COPY INTO (Transact-SQL)**

  Updated guidance for Fabric Data Warehouse to add Azure Blob Storage as a supported source and clarify loading from Azure Storage and OneLake. Clarified execution context (runs as the current user) and introduced expanded use of Fabric Workspace Identity for source authorization, including a new section on required permissions and sensitivity label considerations. Revised CREDENTIAL syntax to use (IDENTITY, SECRET), detailed supported credential types (Microsoft Entra ID, SAS, Storage Account Key, Workspace Identity), and reorganized path/wildcard content. Strengthened firewall and permission prerequisites, refined control-plane vs. data-plane requirements, updated OneLake limitations to support Workspace Identity, and added new examples for ADLS Gen2 and OneLake.

  https://learn.microsoft.com/en-us/sql/t-sql/statements/copy-into-transact-sql?view=azure-sqldw-latest

- **Check OLE DB Driver Installation for SQL Server**

  Major rewrite improves end-to-end troubleshooting for OLE DB drivers. Added PowerShell-driven discovery of installed providers via registry with guidance to interpret InstalledVersion and compare against current GA builds, and clarified side-by-side installs of MSOLEDBSQL (18) and MSOLEDBSQL19. Expanded UDL testing with step-by-step creation/opening, 32-bit vs. 64-bit dialog tips, and troubleshooting aids; clarified extracting connection strings from UDL content. Deepened registry tracing to map ProgID to provider/CLSID/DLL, corrected 32-bit/64-bit paths (including SQLNCLI11.1), and added explicit regsvr32 registration steps and notes for non-Microsoft providers. Included important notes that older providers (SQLNCLI/SQLOLEDB) aren’t shipped with newer SQL Server/SSMS and aren’t recommended for new development, plus links to related troubleshooting.

  https://learn.microsoft.com/en-us/troubleshoot/sql/database-engine/install/windows/oledb-driver-install-check

## Moderate Changes

- **Troubleshoot SQL Server installation errors**

  Reorganized and expanded guidance for setup failures due to corrupted or damaged media, with clearer symptoms (wizard and log errors), supported platforms (SQL Server 2022 x64), and a structured solution path: re-download media, install from a local drive, and rename Setup.rll with updated examples. Added cautions for localized and mixed-language setups, and a follow-on section for deeper diagnostics (review Summary.txt, check disk sector sizes, verify OS support, repair/remove partial installs, and resolve CU/SP update failures) with updated references.

  https://learn.microsoft.com/en-us/troubleshoot/sql/database-engine/install/windows/error-install-sql-server