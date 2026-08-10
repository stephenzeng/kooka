# Microsoft Fabric
**Date created:** 2026-07-19 UTC  
**Tags:** Analytics, Monitoring, Programming  

## New Articles

- **Column mapping for Delta tables**

  Introduced guidance on Delta Lake column mapping to decouple logical column names from physical storage, enabling metadata-only rename and drop operations. Covers supported modes (none, id, name), when to use each, and how to enable them via SQL, PySpark, and Scala. Explains protocol requirements and reader compatibility considerations, with best practices to enable early and communicate schema changes to downstream consumers.

  https://learn.microsoft.com/en-us/fabric/data-engineering/delta-lake-column-mapping

- **Generated columns for Delta tables**

  Added documentation for generated and identity columns in Delta tables, explaining usage patterns and storage/evaluation semantics. Details runtime requirements, API support (DeltaTable builder for identity columns), and constraints such as BIGINT type and monotonicity with possible gaps. Provides SQL, Python, and Scala examples with best practices for deterministic expressions and testing.

  https://learn.microsoft.com/en-us/fabric/data-engineering/delta-lake-generated-columns

- **Variant data type for Delta tables**

  Introduced the Variant data type to store semi-structured data with schema-on-read for faster, repeated access. Details runtime and protocol requirements and shows how to create tables, load data (PARSE_JSON/parse_json), and query using path notation and helper functions (variant_get, try_variant_get, schema_of_variant). Includes guidance for filtering, aggregation, error handling, and operational best practices.

  https://learn.microsoft.com/en-us/fabric/data-engineering/delta-lake-variant

- **Best practices for Structured Streaming**

  Published end-to-end operational guidance for production streaming, including triggers, retry/await patterns, and durable checkpointing. Recommends enabling RocksDB state store and changelog checkpointing for stateful workloads, and optimizing Delta sinks with partitioning, Optimize Write, and auto-compaction. Provides schema management strategies, Event Hubs tuning tips, resilience patterns, and monitoring practices to balance latency, reliability, and cost.

  https://learn.microsoft.com/en-us/fabric/data-engineering/structured-streaming-best-practices

- **Common Structured Streaming patterns**

  Added patterns for fan-out processing with foreachBatch and idempotent writes, running independent queries with isolated checkpoints, and staging data in bronze Delta tables. Explains stream–stream joins with watermarks and time-range conditions, and shows how to monitor pipelines with StreamingQueryListener. Summarizes best practices for checkpoint isolation, idempotency, and Real-time Mode considerations.

  https://learn.microsoft.com/en-us/fabric/data-engineering/structured-streaming-common-patterns

- **Overview of Structured Streaming**

  New conceptual overview covering the streaming model, supported sources and sinks, and execution modes (micro-batch and Real-time Mode). Explains reliability via checkpoints and delivery guarantees, with a complete PySpark example from source to Delta. Provides guidance on triggers like availableNow and checkpoint compatibility, with links to deeper topics.

  https://learn.microsoft.com/en-us/fabric/data-engineering/structured-streaming-overview

- **Real-time mode in Structured Streaming**

  Introduced Real-time Mode for low-latency streaming in Fabric Runtime 2.0, including how it differs from micro-batch execution. Provides prerequisites and enablement steps, support matrices for sources/sinks and operators, and key limitations (update mode only, lakehouse/file I/O not supported). Offers design and monitoring guidance to meet strict latency goals.

  https://learn.microsoft.com/en-us/fabric/data-engineering/structured-streaming-real-time-mode

- **Stateful processing with Structured Streaming**

  Added an in-depth guide to stateful operations, including state stores, checkpointing strategy, and enabling RocksDB with changelog checkpointing to reduce heap pressure. Covers windowed aggregations, watermarks, stream–stream joins, deduplication patterns, and custom state with transformWithState. Includes state inspection tools and best practices to bound state growth and ensure stability.

  https://learn.microsoft.com/en-us/fabric/data-engineering/structured-streaming-stateful-processing

- **Triggers and output modes in Structured Streaming**

  New article explaining trigger types (processing time, available-now, Real-time Mode) and when to use each, with Python and Scala syntax. Clarifies output modes (append, update, complete), their compatibility with aggregations and watermarks, and includes practical end-to-end examples. Helps teams choose configurations that balance latency, correctness, and operational simplicity.

  https://learn.microsoft.com/en-us/fabric/data-engineering/structured-streaming-triggers-output-modes

## Moderate Changes

- **Apply liquid clustering on Delta tables**

  Added guidance to evaluate clustering quality using the Scala clusteringQuality() method, with definitions and interpretation of key metrics. Recommends monitoring quality trends and validating improvements against Spark UI files-scanned metrics, especially before and after OPTIMIZE.

  https://learn.microsoft.com/en-us/fabric/data-engineering/liquid-clustering

- **Compacting Delta tables**

  Documented OPTIMIZE FULL for liquid-clustered Delta tables to recluster all files after changing clustering keys or providers. Explains how it differs from standard OPTIMIZE, provides SQL syntax and scenarios, and cautions about higher cost relative to incremental optimization.

  https://learn.microsoft.com/en-us/fabric/data-engineering/table-compaction