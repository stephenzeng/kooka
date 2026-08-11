# Microsoft Intune
**Date created:** 2026-07-25 UTC  
**Tags:** Administration  

## New Articles

- **Choose the right targeting method in Microsoft Intune**

  Introduced a concept article that explains when to use groups versus assignment filters, how evaluation timing works, and how to move from broad to targeted assignments. Outlines group types (virtual, static, dynamic) and Intune-specific options like assignment filters and enrollment-time grouping. Provides best practices and cautions, including replacing Intune-only dynamic device groups with assignment filters to simplify targeting and improve performance. Includes a mapping from common dynamic group rules to equivalent filter conditions and links to related guidance.

  https://learn.microsoft.com/en-us/intune/fundamentals/choose-targeting-method

## Moderate Changes

- **Manage Apple mobile devices and tokens for automated device enrollment**

  Updated the procedures to reflect the “Apple” tab in the Intune admin center and refined steps for syncing, renewing, and deleting tokens. Expanded token renewal guidance to align with current Apple Business/School Manager navigation and where to download the token, reducing confusion and improving task success.

  https://learn.microsoft.com/en-us/intune/device-enrollment/apple/manage-devices-tokens-apple

- **Assignment Filter Performance Tips for Intune**

  Added guidance to avoid using memberOf in dynamic group rules due to performance costs and unpredictable outcomes. Recommends using direct property comparisons or assignment filters instead, with examples, and reinforces using assignment filters when only Intune consumes the group to improve reliability and speed.

  https://learn.microsoft.com/en-us/intune/fundamentals/filters/performance-recommendations

- **Known Issues for Endpoint Privilege Management**

  Documented that the built-in Endpoint Privilege Manager role and the custom Endpoint Privilege Management Policy Authoring role don’t support scope tags. Provides a workaround to grant Read permission for Device configurations to limit what admins can see via scope tags.

  https://learn.microsoft.com/en-us/intune/epm/troubleshoot-known-issues