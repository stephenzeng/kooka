# Power Apps
**Date created:** 2026-08-30 UTC  
**Tags:** Best Practices, Configuration, Guidance, Monitoring, Performance, Troubleshooting  

## New Articles

- **Handle errors and enable HTTP diagnostics**

  New guidance explains the SDK’s exception hierarchy and shows recommended try/except patterns for robust error handling. It adds strategies for transient HTTP failures using is_transient and retry_after, plus a reusable retry helper. The article also documents timeout and retry configuration via DataverseConfig and how to enable secure HTTP diagnostics with LogConfig, including automatic redaction.

  https://learn.microsoft.com/en-us/power-apps/developer/data-platform/sdk-python/error-handling

## Major Changes

- **Query data**

  Added powerful new query builder capabilities, including string filters (.contains, .startswith, .endswith), .like() with safe wildcard rules, negation and set membership operators, and a raw() escape hatch for advanced OData. Introduced include_annotations() and equivalents on list/retrieve, clarified FetchXML limits (32,768-character URL-encoded) and paging via count, and significantly expanded SQL coverage with supported/unsupported features and validation behavior. These updates help developers write more expressive, performant queries while understanding platform constraints.

  https://learn.microsoft.com/en-us/power-apps/developer/data-platform/sdk-python/query

## Moderate Changes

- **Asynchronous client operations**

  Updated guidance adds the dataframe namespace and shows how to close the client without a context manager using await client.aclose(), noting behavior on repeated calls and post-close usage while recommending async with for pooling. It also clarifies async-specific exceptions (aiohttp.ClientError, asyncio.TimeoutError) and links to centralized error handling to standardize patterns.

  https://learn.microsoft.com/en-us/power-apps/developer/data-platform/sdk-python/async-client

- **Customize tables and columns**

  Expanded coverage lists supported column type strings and aliases, including how to define choice columns with Enum/IntEnum. It clarifies TableInfo and method return values for create/add/remove/get, and adds alternate keys guidance with code, status transition to Active, and the requirement to ensure activation before upserts to avoid 400 errors.

  https://learn.microsoft.com/en-us/power-apps/developer/data-platform/sdk-python/metadata

- **Relationship management**

  Added clear instructions for configuring cascade behavior with provided constants and defaults, plus details of the RelationshipInfo return object and intersect table naming. It documents optional parameters for create_lookup_field and highlights that deleting a one-to-many relationship removes its lookup field and must precede table deletion; missing tables now raise MetadataError in list_table_relationships.

  https://learn.microsoft.com/en-us/power-apps/developer/data-platform/sdk-python/relationships

- **Work with Dataverse data by using the Python SDK**

  File upload guidance now supports mime_type, mode (auto/small/chunk), and if_none_match, with size limits and behavior for large files, including async usage patterns. Batch documentation clarifies changeset rules (e.g., content-ID for intra-changeset references, no reads inside changesets), details BatchResult shapes and helpers, and notes limits (up to 1,000 operations) and when operations expand into multiple requests.

  https://learn.microsoft.com/en-us/power-apps/developer/data-platform/sdk-python/work-data