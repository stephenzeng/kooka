# Microsoft Defender for IoT
**Date created:** 2026-08-12 UTC  
**Tags:** Configuration, Guidance, Security  

## Moderate Changes

- **Configure OT sensor settings from the Azure portal (Public preview)**

  Added a clear warning that deleting an OT sensor setting is permanent and must be recreated to restore, reducing the risk of accidental data loss. Renamed and anchored the settings reference section to improve navigation and linking, and clarified guidance for disconnected sensors, ICS subnet designation, backup server configuration, and handling false malware alerts. No procedural changes were introduced.

  https://learn.microsoft.com/en-us/azure/defender-for-iot/organizations/configure-sensor-settings-portal

- **Configure proxy connections from your OT sensor to Azure**

  Updated prerequisites to require outbound HTTPS (port 443) from sensors to Defender for IoT endpoints, with a pointer to provisioning guidance. Restructured prerequisites into a clear list to make networking requirements easier to validate and reduce setup failures.

  https://learn.microsoft.com/en-us/azure/defender-for-iot/organizations/connect-sensors

- **How to configure the DMI Decoder**

  Clarified SMBIOS requirements for dmidecode and reorganized alternatives with better headings and anchors. Refined module twin and JSON-based configuration guidance, replacing an incorrect example with a valid payload and correcting the SystemInformation_FirmwareVersion property name. Updated the closing section to Related content to surface more relevant references.

  https://learn.microsoft.com/en-us/azure/defender-for-iot/device-builders/how-to-configure-dmi-decoder