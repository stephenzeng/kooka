# Dev and Admin for Dynamics 365 Business Central
**Date created:** 2026-09-03 UTC  
**Tags:** Best Practices, Configuration, Guidance  

## Moderate Changes

- **CameraOptions Overview for Business Central**
  Updated defaults and parameter behavior for camera operations: Quality now defaults to 50 when a CameraOptions object is provided, while calling RequestPictureAsync without options uses 100. Clarified SourceType, MediaType, and AllowEdit definitions (including correct boolean casing and valid values) to help developers set predictable image quality and behavior.
  https://learn.microsoft.com/en-us/dynamics365/business-central/dev-itpro/developer/devenv-camera-options

- **Implementing the Camera in AL for Business Central**
  Added a prominent note that the sample’s .NET interoperability is supported only for on-premises deployments and requires "target": "OnPrem" in app.json; online environments should use the System Application Camera codeunit. Text clarifications improve guidance without changing functionality, helping teams choose the correct approach per environment.
  https://learn.microsoft.com/en-us/dynamics365/business-central/dev-itpro/developer/devenv-implement-camera-al

- **Implementing Location in AL for Business Central**
  Clarified that the example’s .NET interoperability is on-premises only and requires "target": "OnPrem"; online implementations should use the System Application Geolocation codeunit. Updated the sample to correctly create LocationOptions, set EnableHighAccuracy via property assignment, and pass options to RequestLocationAsync(LocationOptions), aligning with current API usage.
  https://learn.microsoft.com/en-us/dynamics365/business-central/dev-itpro/developer/devenv-implement-location-al

- **Random Test Data for Application Tests**
  Modernized testing guidance to use LibraryRandom (RandInt/RandDec) and the Assert codeunit, replacing older RandomNumberGenerator patterns. Added clear examples for seeding with LibraryRandom.SetSeed(1) to reproduce runs and refined examples to improve deterministic tests and effective fuzzing.
  https://learn.microsoft.com/en-us/dynamics365/business-central/dev-itpro/developer/devenv-random-test-data

- **Application Testing Example: Testing Purchase Invoice Discounts**
  Updated the test to current APIs and coding conventions: switched to LibraryRandom, replaced an Option with the "Purchase Document Type" enum, adjusted data types, and standardized method calls and boolean casing. These changes improve reliability and maintainability of the purchase invoice discount test.
  https://learn.microsoft.com/en-us/dynamics365/business-central/dev-itpro/developer/devenv-test-application-example-purchase-invoice-discounts

- **Testing with Permission Sets in Business Central**
  Corrected API and enum usage and ensured proper initialization of PermissionTestHelper to make the sample compile and run as intended. Streamlined method calls and removed unused variables, improving accuracy when applying permission sets during tests.
  https://learn.microsoft.com/en-us/dynamics365/business-central/dev-itpro/developer/devenv-testing-with-permission-sets

- **Create Test Runner Codeunits in AL**
  Updated examples to current patterns: use Codeunit.Run, the AllObj record for object access, FindSet()/Next(), and proper statement terminators. Renamed the second example to EnabledTestRunnerCodeunit, aligning guidance with modern AL conventions for executing tests reliably.
  https://learn.microsoft.com/en-us/dynamics365/business-central/dev-itpro/developer/devenv-testrunner-codeunits