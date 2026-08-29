# Dynamics 365 Finance
**Date created:** 2026-08-29 UTC  
**Tags:** Analytics, Best Practices, Configuration, Guidance, Performance  

## New Articles

- **Use Cube navigator in Business performance planning**

  Introduced a new article describing Cube navigator (v1.16), which replaces the legacy Draft/Published lists and organizes planning models with folders and subfolders. It explains selecting and auto-selecting cubes, drag-and-drop organization, moving and reordering cubes, and cube actions such as open, rename (drafts only), view properties, move, and reorder. Folder actions include create, rename, reorder, and delete—with cubes returned to the root if a folder is deleted. Search covers cube names, tags, descriptions, and folder names, with filters for All, Draft, and Published. The guidance recommends a simple hierarchy, using folders over naming conventions, and grouping models by planning domain.

  https://learn.microsoft.com/en-us/dynamics365/finance/business-performance-planning/cube-navigator

## Major Changes

- **Create a cube from Excel (preview)**

  Substantially updated guidance introduces the Cubes (preview) workflow to build planning cubes directly from Excel, including creating dimensions and the cube simultaneously. The process clarifies table selection and explicit primary key choice, improves fact-to-dimension mapping with driver designation and validation, and reuses existing dimensions while flagging disconnected ones during review. A new Auto data load after publish (preview) adds status monitoring and blocking rules to prevent fact loads when dimension issues occur, with thresholds that disable auto-load for large files. Post-publish enhancements enable adding drivers, provide calculated column examples, and rename the performance option to “Enable fast analytics index” (NCCI on by default in v1.17). Known limitations are expanded, including the need to sync cubes after external dimension changes and caps for large member counts.

  https://learn.microsoft.com/en-us/dynamics365/finance/business-performance-planning/bpp-cube-Excel