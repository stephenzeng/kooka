# Microsoft Fabric
**Date created:** 2026-08-18 UTC  
**Tags:** Analytics, Best Practices, Configuration, Guidance, Performance  

## New Articles

- **Closing forecast period**

  Introduced guidance on closing completed forecast periods to finalize values, prevent further edits, and extend the planning horizon. Provides a step-by-step workflow for reviewing and closing periods at appropriate times (for example, after month-end actuals). Explains how reforecasting can populate newly opened periods with copied values and updated assumptions, supporting continuous planning. Highlights the shift from forecast to actuals as periods progress, enabling more reliable rolling forecasts.

  https://learn.microsoft.com/en-us/fabric/iq/plan/planning-concept-closing-forecast-period

- **Rule-Based Optimization and Derived Measure Optimization**

  Added a how-to article on using Optimize for derived measures and allocation rules in planning sheets. Details how to maximize an objective (such as Margin %) by adjusting dependent measures, configuring variables to update, and setting thresholds and aggregation. Introduces rule-based optimization with locking, distribution, and min–max rules, including a scenario that protects specific regions while meeting a target through other inputs. This helps planners systematically tune forecasts while honoring business constraints.

  https://learn.microsoft.com/en-us/fabric/iq/plan/planning-optimize/planning-how-to-optimize-derived-measures

## Major Changes

- **Allocate Plans with a Cube**

  Expanded conceptual guidance on allocating plans across unrelated dimensions using cubes and driver-based allocations. Added explanations and diagrams showing how allocation drivers can live in the semantic model and not the planning sheet, with a weighted allocation example and refined workflow steps. Updated hierarchies (for example, Region > City) and clarified how to distribute at granular levels and aggregate back to consolidated dimensions. Enhanced use cases demonstrate enterprise budgeting and aligning assumptions entered at different levels for consistent reporting.

  https://learn.microsoft.com/en-us/fabric/iq/plan/planning-concept-cube

## Moderate Changes

- **Dataflow Gen2 cost and performance: capability benchmarks and CU costs**

  Updated the benchmark summary by removing the “CU consumed” column and adjusting headers and rows across scenarios. This streamlines the tables to emphasize scenario descriptions and execution times, reducing confusion around consumption metrics without altering other content.

  https://learn.microsoft.com/en-us/fabric/data-factory/dataflow-gen2-cost-performance-benchmarks