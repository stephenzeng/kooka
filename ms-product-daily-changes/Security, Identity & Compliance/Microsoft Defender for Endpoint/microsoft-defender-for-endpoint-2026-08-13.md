# Microsoft Defender for Endpoint
**Date created:** 2026-08-13 UTC  
**Tags:** Automation, Configuration, Guidance  

## Major Changes

- **Offboard device from Defender for Endpoint.**
  
  Expanded API support to include Linux, aligning offboarding across platforms. The article was restructured into a table for clearer OS coverage and removed the previous Linux limitation. It also clarifies that on Windows, the API stops the sensor service but does not remove onboarding registry information, helping admins plan complete device offboarding workflows.

  https://learn.microsoft.com/en-us/defender-endpoint/api/offboard-machine-api

## Moderate Changes

- **Offboard or uninstall Microsoft Defender for Endpoint on Linux**
  
  Added an API-based option to offboard Linux servers, complementing existing script and JSON methods. The new section links to the Offboard machine API, enabling automated and scalable device retirement from Defender for Endpoint.

  https://learn.microsoft.com/en-us/defender-endpoint/linux-off-board-endpoints

- **Offboard devices**
  
  Updated guidance to include Linux in the supported platforms and introduced API-based offboarding as a documented method. This streamlines cross-platform operations and enables automation through direct links to the API procedure.

  https://learn.microsoft.com/en-us/defender-endpoint/offboard-machines