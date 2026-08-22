# Dynamics 365 Contact Center
**Date created:** 2026-08-22 UTC  
**Tags:** Best Practices, Configuration, Guidance  

## New Articles

- **Set up and manage planning groups**

  Introduced a new how-to article that explains planning groups and how to configure them for accurate forecasting and consistent service objectives. Covers required settings such as name, time zone, demand scope (queue/channel pairs), and service objectives, with the constraint that each queue-channel pair can belong to only one planning group. Provides step-by-step creation guidance and shows how service objectives (service level, answer time, shrinkage, concurrency, occupancy) flow into capacity plans. Details how to associate related artifacts like shift plans, forecast scenarios, and capacity plans.

  https://learn.microsoft.com/en-us/dynamics365/contact-center/use/workforce-management-use-planning-groups

## Major Changes

- **Build an Azure AI agent**

  Updated integration guidance to set activity ChannelData using a helper method (SetChannelData) instead of manually serializing JSON for deliveryMode. Reworked the escalation payload to use a command with type "Escalate" and a context dictionary, and clarified how to attach this payload to ChannelData. Added instructions and C# examples for passing context variables to a human representative during escalation, including support for an optional isDisplayable flag. Included configuration steps to define context variables on the workstream for a smoother handoff experience.

  https://learn.microsoft.com/en-us/dynamics365/contact-center/extend/build-your-azure-agent

## Moderate Changes

- **Use evaluation plan**

  Expanded the Conditions guidance to clarify that available conditions depend on the selected record type. Added practical examples, including evaluating open cases, filtering by business unit, and excluding records that were already evaluated, to help administrators design precise evaluation criteria.

  https://learn.microsoft.com/en-us/dynamics365/contact-center/use/evaluation-plan

- **Create and manage shift rotation policies**

  Reorganized and expanded instructions to clarify how rotation positions drive bookings and how to configure slots by day with different start/end times (within the 2–24 slot limit). Clarified edit, pause/resume, and delete behaviors—changes apply on the next scheduler run, and policies assigned to plans cannot be deleted—and added two assignment flows with an important note that reassigning plans requires removing existing schedules and rerunning scheduling.

  https://learn.microsoft.com/en-us/dynamics365/contact-center/use/workforce-management-shift-rotation-policies