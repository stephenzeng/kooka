# Microsoft Intune
**Date created:** 2026-08-25 UTC  
**Tags:** Configuration, Governance, Security, Troubleshooting  

## New Articles

- **IDispatch error 3603 during content distribution**

  Introduced a troubleshooting guide for Configuration Manager that explains why content distribution to a distribution point can fail with IDispatch error 3603. The article identifies missing IIS 6 Metabase Compatibility and IIS 6 WMI Compatibility role services as the root cause. It provides clear remediation steps via Server Manager and PowerShell and includes log examples to verify progress. Guidance also links to prerequisites and escalation steps to streamline resolution.

  https://learn.microsoft.com/en-us/troubleshoot/mem/configmgr/content-management/content-distribution-idispatch-error

- **Azure web app doesn't have the Contributor role at the subscription level**

  Added guidance for CMG deployments with Azure Resource Manager where the web app is intentionally not granted Contributor at the subscription level. The article clarifies that Contributor should be scoped to the resource group and only Read at subscription scope. It includes verification steps and instructions to remove any unnecessary subscription-level Contributor assignment. A caution not to delete the web app helps prevent service disruption.

  https://learn.microsoft.com/en-us/troubleshoot/mem/configmgr/cloud-services/contributor-role-not-assigned-for-web-app

- **Device displays non-debug deployment for a task sequence instead of a debug deployment**

  Published troubleshooting steps for scenarios where a device shows a non-debug task sequence deployment instead of the intended debug deployment. The behavior is by design because only one deployment per task sequence is shown, often the oldest. The article outlines options to ensure a debug experience, including using a copied task sequence, leveraging TSDebugMode, or removing older deployments. It also clarifies that with TSDebugMode enabled, a non-debug deployment is sufficient.

  https://learn.microsoft.com/en-us/troubleshoot/mem/configmgr/os-deployment/debug-deployment-not-displayed

- **Get network captures from a task sequence in Windows PE**

  Introduced a procedural guide to capture network traces during task sequences in Windows PE. It explains WinPE limitations and shows how to add the Network Monitor 3 driver and binaries into the boot image, set appropriate permissions, and bind the driver. After distribution of the updated boot image, admins can run NetMon in WinPE to collect traces. The article notes that parsers are unavailable in WinPE and recommends analyzing captures on another machine.

  https://learn.microsoft.com/en-us/troubleshoot/mem/configmgr/os-deployment/get-network-captures-from-task-sequence

- **Migrating a driver package fails because the SMS Provider has insufficient permissions**

  Added a troubleshooting article for driver package migrations that fail due to insufficient permissions on the package source path. It helps identify the issue using migmctrl.log and explains the difference in behavior between driver packages and regular packages. The guidance directs admins to grant full control on the source and clarifies why distribution might later fail for regular packages. Links to driver management docs provide additional context.

  https://learn.microsoft.com/en-us/troubleshoot/mem/configmgr/os-deployment/insufficient-permissions-to-migrate-driver-package

- **Invalid data error when you import a MOF file in Configuration Manager**

  Published instructions to resolve “Invalid data” errors when importing MOF files to extend hardware inventory. The article points to MOF syntax or unparseable data as the cause and recommends validating with mofcomp.exe -check. It outlines an iterative approach to fix errors before importing the corrected MOF. Related links help admins follow best practices for inventory extensions.

  https://learn.microsoft.com/en-us/troubleshoot/mem/configmgr/client-management/invalid-data-error-import-mof-file

- **DP installations or upgrades take longer than expected**

  Released guidance for slow distribution point installations or upgrades caused by Distribution Manager reaching its concurrent upgrade thread limit. The article shows how to confirm the condition in DistMgr.log, explains the default limit, and details the DPUpgradeThreadLimit site-control setting. It provides steps to adjust or remove the custom limit and cautions about site-control changes. References to relevant WMI classes support safe operations.

  https://learn.microsoft.com/en-us/troubleshoot/mem/configmgr/content-management/slow-dp-installation-upgrade

- **Configuration Manager client uses a neighbor boundary group DP first**

  Added troubleshooting content explaining why a client may prefer a neighbor boundary group DP when it shares the client’s subnet and becomes eligible after fallback. The behavior stems from subnet-based sorting that prioritizes same-subnet DPs even if they’re in a neighbor group. The article recommends avoiding placement of neighbor DPs on client subnets of the current boundary group and links to configuration guidance.

  https://learn.microsoft.com/en-us/troubleshoot/mem/configmgr/content-management/use-neighbor-boundary-group-dp

- **Windows Installer source list update fails because of HTTPS distribution points**

  Published a fix for error 0x87D00226 when clients update Windows Installer source lists in environments with HTTPS-only distribution points. The article explains the protocol mismatch that results in CCM_E_INVALIDPROTOCOL and offers two secure workarounds: enable package share access for packages or add the application source to the Windows Installer source list in the registry. It advises against enabling HTTP and links to source management documentation.

  https://learn.microsoft.com/en-us/troubleshoot/mem/configmgr/content-management/windows-installer-source-list-update-fails

## Moderate Changes

- **Create a custom role in Intune**

  Updated Remote Help app permissions and renamed Unattended control to Android unattended control with clear requirements for dedicated, Intune‑enrolled Android devices. Added a new Windows unattended control remote sign-in permission for corporate-owned Windows devices, with guidance to explicitly assign and scope permissions to eligible devices. These changes improve clarity and help admins avoid overprivileging.

  https://learn.microsoft.com/en-us/intune/fundamentals/role-based-access-control/create-custom-role

- **Network endpoints for Microsoft Intune**

  Added dependencies for Remote Help Remote Sign-in on Azure Virtual Desktop session host endpoints. Clarified which Azure cloud endpoints to use for commercial versus US Government (GCC) customers to ensure successful connectivity.

  https://learn.microsoft.com/en-us/intune/fundamentals/endpoints

- **Prerequisites for the Microsoft Tunnel in Intune**

  Removed the powerlift-frontdesk.acompli.net diagnostic endpoint from the required network endpoints list. This change simplifies firewall and proxy configurations by excluding an endpoint that’s no longer needed.

  https://learn.microsoft.com/en-us/intune/device-security/microsoft-tunnel/prerequisites