# Microsoft Defender XDR
**Date created:** 2026-09-02 UTC  
**Tags:** Analytics, Best Practices, Compliance, Governance, Guidance, Security  

## Major Changes

- **DataSecurityBehaviors**

  Marked the article as generally available by removing Preview labels and prerelease notices. Added PolicyInfo (dynamic) and Policies (string) to the DataSecurityBehaviors schema to include policy context for each behavior. These fields improve correlation with insider risk management policies, enabling stronger analytics and investigations. Guidance now reflects production readiness.

  https://learn.microsoft.com/en-us/defender-xdr/advanced-hunting-datasecuritybehaviors-table

- **DataSecurityEvents**

  Announced general availability by removing Preview indicators and prerelease disclaimers. Expanded the schema with new fields for PhysicalAccessPointInfo, RemovableMediaInfo, and multiple RiskyAIUsage attributes, while removing several URL, email, file path, and workload fields. The updated design deepens coverage for physical access, removable media, and AI usage scenarios and streamlines legacy attributes. Customers should update queries and analytics to use the new fields and retire removed columns.

  https://learn.microsoft.com/en-us/defender-xdr/advanced-hunting-datasecurityevents-table

## Moderate Changes

- **Create custom detection rules in Microsoft Defender XDR**

  Updated guidance to include both DeviceId and ReportId for Defender for Endpoint tables to ensure correct device group scoping and reliable process tree construction. This improves rule accuracy and investigation fidelity.

  https://learn.microsoft.com/en-us/defender-xdr/custom-detection-rules

- **Before you begin using Defender Experts Hunting**

  Clarified data residency and retention: hunting and report data remain in the customer’s Defender storage, with operational data stored in the US for GCC, in the EU for EU Data Boundary customers, and worldwide for others; retention includes up to 90 days grace after expiration and 30 days deletion after termination. Updated availability to align with Microsoft 365/Office 365 international availability, including commercial public cloud availability, a Gov offering for GCC customers not requiring FedRAMP, and unavailability for GCC-H, DoD, and sovereign clouds.

  https://learn.microsoft.com/en-us/defender-xdr/defender-experts/defender-experts-hunting-prerequisites

- **Before you begin using Defender Experts MDR**

  Restructured data collection and retention guidance to explicitly define data residency per customer segment (US for GCC Plan 1 for Gov, EU for EU Data Boundary, worldwide for others) and clarify retention (up to 90-day grace and 30-day deletion on termination). Updated availability to match Microsoft 365/Office 365 international availability, including commercial public cloud availability, a Plan 1 for Gov option for GCC customers not requiring FedRAMP, and no availability in GCC-H, DoD, or sovereign clouds.

  https://learn.microsoft.com/en-us/defender-xdr/defender-experts/defender-experts-mdr-prerequisites