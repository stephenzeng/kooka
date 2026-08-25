# Dynamics 365 Customer Service
**Date created:** 2026-08-25 UTC  
**Tags:** Automation, Best Practices, Configuration, Guidance  

## Major Changes

- **Configure routing to preferred or previously engaged representatives in Dynamics 365 Contact Center**

  Added detailed guidance for keeping the same expert on returning asynchronous chats using representative affinity with presence checks and active conversation limits. Clarifies applicability rules—identify the previous representative, verify presence, evaluate conversation limit, then choose fallback—so routing behaves predictably. Provides prerequisites and step-by-step configuration via conversation orchestration playbooks, including selecting queues, allowed presences, enabling active conversation limits, and choosing fallback options. This improves continuity for customers while helping manage representative workload and routing reliability.

  https://learn.microsoft.com/en-us/dynamics365/customer-service/administer/configure-preferred-agent

## Moderate Changes

- **Create and manage workstreams**

  Updated terminology from “agent” to “representative” across the article and UI references for consistency with the product. Renamed “Agent affinity” to “Representative affinity” and clarified behavior and scope, including that affinity applies only to push work distribution. These changes align the guidance with current UI labels and reduce ambiguity.

  https://learn.microsoft.com/en-us/dynamics365/customer-service/administer/create-workstreams

- **Manage overflow of work items in queues**

  Removed the preview label and banner from the natural language playbooks section, indicating the capability is now generally available. This signals production readiness so organizations can adopt overflow automation with confidence.

  https://learn.microsoft.com/en-us/dynamics365/customer-service/administer/manage-overflow

- **Create and manage users and user profiles**

  Removed swarming-related instructions and views to reflect current feature scope. Introduced a new bulk action to update conversation limits (1–100) with guidance on starting conservatively and increasing over time to strengthen affinity. Renamed the bulk action to “Update capacity profiles” and refreshed view labels for clarity.

  https://learn.microsoft.com/en-us/dynamics365/customer-service/administer/users-user-profiles