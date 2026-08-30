# Microsoft Foundry
**Date created:** 2026-08-30 UTC  
**Tags:** Configuration, Get Started, Guidance  

## Moderate Changes

- **Deploy a crash-resilient long-running agent (preview)**

  Updated guidance to use curl and Azure CLI for invoking and monitoring agents, replacing azd invoke/monitor commands. Clarified local runs with azd ai agent run --no-client and driving requests via curl, and simplified crash recovery testing with inline JSON. Added steps to capture the Responses endpoint from azd up, obtain an access token, and perform authenticated REST calls, improving reliability and transparency of end-to-end testing.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/deploy-resilient-agent

- **Deploy a steerable agent (preview)**

  Reworked the workflow to use direct REST calls with curl and Azure CLI, replacing azd agent invoke/monitor and JSON request files. Introduced explicit use of conversation IDs to steer in-flight turns and streamlined monitoring by streaming a specific response by ID, enabling more precise control and observability of agent behavior.

  https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/deploy-steerable-agent