# Dynamics 365 Commerce
**Date created:** 2026-09-03 UTC  
**Tags:** Configuration, Guidance  

## Major Changes

- **DOM processing**

  Overhauled inventory lookup guidance to reflect version-specific behavior and broadened capabilities. Starting with version 10.0.46, DOM natively considers the sales order line’s inventory status when determining availability and documents supported dimensions (configuration, size, color, style, version, site, warehouse, batch/serial). The article clarifies that advanced warehouse management dimensions like location and license plate, as well as custom dimensions, require extensibility, and explains that quantities reserved during a DOM run are temporarily added back to avoid self-reduction of availability. It also adds a legacy behavior subsection and a direct link to the legacy on-hand entity for historical reference.

  https://learn.microsoft.com/en-us/dynamics365/commerce/dom-processing

## Moderate Changes

- **DOM considerations and limitations**

  Updated guidance adds an advanced warehouse management compatibility section and clarifies that from version 10.0.46, DOM considers inventory status on sales order lines during availability checks. It provides extensibility guidance for handling other advanced warehouse dimensions, clarifies warehouse reassignment behavior when loads/works/shipments exist, and points to relevant customization hooks. The article is streamlined to highlight key profile differences, cloud-only availability, and a consolidated resources list.

  https://learn.microsoft.com/en-us/dynamics365/commerce/dom-limitations