# Power Query
**Date created:** 2026-07-31 UTC  
**Tags:** Analytics, Programming  

## New Articles

- **Developing an ADBC-based Power Query connector**

  Introduced comprehensive guidance for building ADBC-based connectors, including when to choose ADBC over ODBC and how to configure Adbc.Connection and driver settings. Explained credential handling, driver discovery, catalog/schema support, and native-to-M type mapping. Clarified supported authentication options and how to design efficient navigation tables with query folding. Included references for advanced patterns, SQL generator architecture, and transitioning from ODBC to ADBC.  
  https://learn.microsoft.com/en-us/power-query/adbc

- **Implement Query Folding and Advanced Patterns in ADBC-based connectors**

  Added advanced implementation patterns that show how to enable query folding with SqlView.Generator using a two-layer SQL dialect (SQL92 base plus source-specific overrides). Detailed how to surface keys from information_schema, enable DirectQuery and foldable native queries via NativeQueryProperties, and adapt the sample to other FlightSQL sources by updating connector files. Linked to related guidance on fundamentals, SQL generator architecture, and enabling ODBC DirectQuery and native queries.  
  https://learn.microsoft.com/en-us/power-query/adbc-advanced-patterns

- **SQL generator for ADBC connectors**

  Introduced a structured approach for implementing folding with a layered SQL generator built on a reusable SQL92 base and dialect-specific overrides. Covered configuring SqlView.Generator, merging capability and function overrides, and extending the AstVisitor for typed literals and LIMIT/OFFSET handling. Provided practical steps to adapt the generator for other backends by adjusting type facets, casting rules, function remappings, and literal formatting.  
  https://learn.microsoft.com/en-us/power-query/adbc-sql-generator

## Moderate Changes

- **List of Samples**

  Added an ADBC section featuring a DuckDB (FlightSQL) connector sample that uses Adbc.Connection and demonstrates query folding with SqlView.Generator. Included a link to the DataConnectors repository and pointed to the ADBC connector development guide to help authors get started quickly.  
  https://learn.microsoft.com/en-us/power-query/samples-directory

- **Snowflake**

  Updated DateTimePrecision behavior so a null value now defaults to microseconds (instead of nanoseconds) for ADBC timestamp handling. Clarified guidance on avoiding overflow for dates outside 1677–2262 and recommended using ODBC when higher precision is required.  
  https://learn.microsoft.com/en-us/power-query/connectors/snowflake