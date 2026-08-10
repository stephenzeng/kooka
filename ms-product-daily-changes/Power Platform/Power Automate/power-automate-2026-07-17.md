# Power Automate
**Date created:** 2026-07-17 UTC  
**Tags:** Governance, Security  

## New Articles

- **PGP cryptography reference for Power Automate for desktop**

  Introduced a new reference page for PGP cryptography actions in Power Automate for desktop. The article documents Encrypt file with PGP and Decrypt file with PGP, detailing inputs (file paths, key sources as files or ASCII‑armored text), supported algorithms (AES‑128/192/256, Triple DES, CAST5), compression (ZIP/ZLIB/BZIP2/None), ASCII armor, and passphrase handling. It also lists expected exceptions (for missing files, invalid keys, or incorrect passphrases) and clarifies that no variables are produced. This guidance helps teams implement secure file encryption and decryption workflows with predictable behavior and robust error handling.

  https://learn.microsoft.com/en-us/power-automate/desktop-flows/actions-reference/pgp

## Moderate Changes

- **Flow checker**

  Expanded rule management to cover both Solution checker in the Power Platform admin center and Flow checker configuration in the Power Automate portal, with clear precedence for admin center enforcement and environment‑level setup steps. Added support for parameterized rules and documented required Analysis Override privileges (Read, Write, Create), while clarifying inheritance and precedence across environments and groups to prevent misconfiguration.

  https://learn.microsoft.com/en-us/power-automate/desktop-flows/static-analysis