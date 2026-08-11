# Dynamics 365 Contact Center
**Date created:** 2026-07-29 UTC  
**Tags:** Administration  

## Moderate Changes

- **Configure a WhatsApp channel through Azure Communication Services**

  Restructured prerequisites with dedicated steps to set up advanced messaging to register and connect a WhatsApp Business Account via Azure Communication Services and to configure Event Grid. Emphasized required Microsoft Entra app permissions and role assignments to prevent webhook validation failures and ensure WhatsApp events are delivered, and added a pre-creation check to confirm the account is registered and connected. Corrected channel field mappings (Event grid app ID is now Microsoft Entra application or URI; Event grid app tenant ID is now Microsoft Entra tenant ID) and removed outdated Azure account/ACS resource/phone number acquisition details.

  https://learn.microsoft.com/en-us/dynamics365/contact-center/administer/configure-whatsapp-acs