# Dynamics 365 Customer Service
**Date created:** 2026-08-13 UTC  
**Tags:** Configuration, Guidance  

## Moderate Changes

- **Assignment methods for queues**

  Added guidance on using pick-based assignment by selecting the No auto assignment method. The update explains that items are routed to a queue without auto-assignment so agents can pick from their Inbox or supervisors can assign from the ongoing conversation dashboard in Copilot Service workspace, with a recommendation to monitor queues to prevent unattended items.

  https://learn.microsoft.com/en-us/dynamics365/customer-service/administer/assignment-methods

- **Configure assignment methods for queues**

  Updated configuration steps to help admins select an assignment method for a queue, including Highest capacity, Advanced round robin, Least active, and No auto assignment. The creation flow was reorganized so method selection precedes rule creation, with clearer sequencing and labels in the rule dialog (name, conditions, order by, create).

  https://learn.microsoft.com/en-us/dynamics365/customer-service/administer/configure-assignment-rules