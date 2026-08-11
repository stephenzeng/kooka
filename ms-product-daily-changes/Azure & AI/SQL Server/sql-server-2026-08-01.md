# SQL Server
**Date created:** 2026-08-01 UTC  
**Tags:** Administration, Azure, Other  

## New Articles

- **Deprecation of AMQP Protocol for Change Event Streaming**

  Announced deprecation of AMQP for Change Event Streaming and introduced Kafka as the supported protocol. Added the new destination_type AzureEventHubs (Kafka) for new stream groups starting Aug 15, 2026, with existing AMQP groups supported until April 2027. Provided migration guidance to recreate stream groups, move tables without losing events, and handle changes for both publishers and consumers. Clarified authentication updates (use Microsoft Entra or service key; SAS no longer supported) and network requirements (use port 9093 instead of 5671/5672). Included an error reference for invalid destination_type values and links to relevant procedures and DMVs.

  https://learn.microsoft.com/en-us/sql/relational-databases/track-changes/change-event-streaming/amqp-deprecation?view=sql-server-ver17

## Moderate Changes

- **Configure change event streaming (preview) to Azure Event Hubs**

  Added AMQP deprecation notices in prerequisites and example sections to guide customers planning or maintaining Event Hubs integrations. Updated guidance to align with the move to Kafka, helping readers choose supported options and avoid deprecated configurations.

  https://learn.microsoft.com/en-us/sql/relational-databases/track-changes/change-event-streaming/configure?view=sql-server-ver17

- **JSON message format - change event streaming**

  Added a notice about AMQP deprecation to alert readers that Kafka-based integrations are the forward path. No other content changes were made.

  https://learn.microsoft.com/en-us/sql/relational-databases/track-changes/change-event-streaming/message-format?view=sql-server-ver17

- **What is change event streaming (preview)?**

  Introduced an AMQP deprecation notice and aligned terminology with the CES acronym for consistency. Minor formatting updates improve readability while signaling the protocol shift toward Kafka.

  https://learn.microsoft.com/en-us/sql/relational-databases/track-changes/change-event-streaming/overview?view=sql-server-ver17