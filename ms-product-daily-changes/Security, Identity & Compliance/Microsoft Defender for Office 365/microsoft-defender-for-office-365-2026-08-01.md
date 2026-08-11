# Microsoft Defender for Office 365
**Date created:** 2026-08-01 UTC  
**Tags:** Security  

## New Articles

- **Inventory delegated From addresses for outbound spam policies**

  Introduced a step-by-step guide to inventory delegated From addresses that affect outbound spam policies, helping admins prevent unexpected sending restrictions. Provides commands to list Send As assignments and a complete PowerShell script to enumerate Send on behalf permissions across mailboxes and group types, with export guidance. Includes a function to expand and review group-based permissions (including nested groups) to identify effective senders. Explains how to map effective delegates to applicable outbound spam policies, with links to related configuration and troubleshooting topics.

  https://learn.microsoft.com/en-us/defender-office-365/outbound-spam-delegated-from-addresses-inventory

- **Outbound spam limits with Send As and Send on behalf permissions**

  Describes how outbound spam policy limits are evaluated in delegated scenarios, clarifying that policy selection is based on the 5322.From address while recipient counts accrue to the authenticated sender. Offers concrete examples of how switching From addresses and policy changes affect limit accrual, plus planning guidance for shared mailboxes and Microsoft 365 Groups. Provides troubleshooting steps for unexpected restrictions, security considerations for potential compromise, and an FAQ on recipient counting and delegate behavior.

  https://learn.microsoft.com/en-us/defender-office-365/outbound-spam-policies-send-as-send-on-behalf

## Major Changes

- **Bulk email detection and bulk complaint level (BCL) in cloud organizations**

  Shifted guidance from header-based tagging to policy-driven Promotions tagging for bulk messages, removing the prior requirement to add a mail flow header. Clarified that all identified bulk mail receives the Promotions tag, and enabling Bulk moves redirects such messages to the Promotions folder with learning based on user actions. Added an optional mail flow rule to suppress Promotions tagging for specific senders or recipients and updated feature matrices and rule references from Bulk to Promotions. Refined folder behavior and opt-in/opt-out policy guidance, simplifying enablement steps and clarifying delivery outcomes.

  https://learn.microsoft.com/en-us/defender-office-365/anti-spam-bulk-complaint-level-bcl-about

## Moderate Changes

- **What's new in Microsoft Defender for Office 365**

  Added a July 2026 entry noting localized default “Mark as” and notification email templates that automatically send in the user’s preferred Outlook language. Confirmed that custom admin-defined templates are unaffected.

  https://learn.microsoft.com/en-us/defender-office-365/defender-for-office-365-whats-new

- **Manage quarantined messages and files as an admin**

  Updated permissions to include Security Operator with read-only access for all users and clarified which reader roles can preview and download quarantined messages. Aligned guidance across the Microsoft 365 Defender portal and Microsoft Entra permissions to support least-privilege administration.

  https://learn.microsoft.com/en-us/defender-office-365/quarantine-admin-manage-messages-files

- **Admin review for user reported messages**

  Clarified that default automatic notification templates are localized to each user’s preferred Outlook language when automatic notifications are enabled. Confirmed that localization does not change verdicts, classifications, or automated investigations, and that custom templates remain unchanged.

  https://learn.microsoft.com/en-us/defender-office-365/submissions-admin-review-user-reported-messages