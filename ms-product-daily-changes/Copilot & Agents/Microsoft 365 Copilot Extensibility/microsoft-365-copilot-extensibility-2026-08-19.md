# Microsoft 365 Copilot Extensibility
**Date created:** 2026-08-19 UTC  
**Tags:** Configuration, Guidance  

## New Articles

- **retrievalThumbnail resource type**

  Introduced a new preview resource defining thumbnails returned by the Retrieval API to give visual context for results. It specifies Base64-encoded content, mediaType, and pageNumber to align images with extracted text. The page includes a clear JSON representation and notes there are no relationships, helping developers parse and display thumbnails consistently.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/extensibility/api/ai-services/retrieval/resources/retrievalthumbnail

- **sharePointEmbeddedConfiguration resource type**

  Added a new reference that enables configuring the Retrieval API to access SharePoint Embedded containers. The resource defines the containerTypeId property and provides a JSON payload to streamline setup. It links to billing and container type requirements, helping teams correctly provision and govern SharePoint Embedded usage.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/extensibility/api/ai-services/retrieval/resources/sharepointembeddedconfiguration

## Major Changes

- **Retrieve grounding data**

  Introduced version pivots separating stable graph-v1 and graph-preview behaviors for clearer API guidance. Added a preview-only includeThumbnails parameter that can return page numbers and thumbnail metadata in retrieval responses. Included a dedicated preview example showing request/response with pageNumbers and thumbnails to accelerate adoption and testing. Other clarifications improve readability without changing stable behavior.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/extensibility/api/ai-services/retrieval/copilotroot-retrieval

- **dataSourceConfiguration resource type**

  Refactored documentation into graph-v1 and graph-preview pivots to better distinguish stable and preview capabilities. In v1, externalItem is now optional, simplifying configurations and providing a JSON example. In preview, added sharePointEmbedded and clarified that configurations must include either externalItem or sharePointEmbedded, with updated examples to guide correct setup.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/extensibility/api/ai-services/retrieval/resources/datasourceconfiguration

## Moderate Changes

- **retrievalExtract resource type**

  Organized content into versioned pivots and documented properties for each. The preview now returns pageNumbers when includeThumbnails is true, with separate JSON examples for v1 and preview to ensure accurate parsing.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/extensibility/api/ai-services/retrieval/resources/retrievalextract

- **retrievalHit resource type**

  Expanded guidance with pivoted sections and detailed property tables for v1 and preview. The preview adds a thumbnails collection, and separate JSON examples clarify differences so developers can handle stable and preview payloads correctly.

  https://learn.microsoft.com/en-us/microsoft-365/copilot/extensibility/api/ai-services/retrieval/resources/retrievalhit