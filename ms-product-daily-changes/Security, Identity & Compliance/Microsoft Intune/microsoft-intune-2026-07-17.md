# Microsoft Intune
**Date created:** 2026-07-17 UTC  
**Tags:** Administration, Monitoring  

## Moderate Changes

- **Device Action: Delete**

  Added a new “Delete action status” section detailing what happens after you delete a device. The article clarifies that deleted devices are immediately hidden in the admin center, the Device actions report shows the status as Completed, and for MDM devices, Delete also triggers a Retire. It explains that Completed reflects server-side processing and does not guarantee the client has finished the Retire.

  https://learn.microsoft.com/en-us/intune/device-management/actions/delete

- **Device Actions - Wipe, Lock, Locate, and More**

  Updated the overview with a clarification for MDM devices: deleting a device hides it right away and also initiates a Retire. It also clarifies that a Completed status indicates server-side completion, not confirmation that the device has completed the Retire process.

  https://learn.microsoft.com/en-us/intune/device-management/actions/