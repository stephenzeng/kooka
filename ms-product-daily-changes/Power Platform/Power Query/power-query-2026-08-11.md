# Power Query
**Date created:** 2026-08-11 UTC  
**Tags:** Guidance, Performance  

## Moderate Changes

- **Working with duplicate values**

  Updated guidance notes that removing duplicates can use significantly more memory when the operation doesn’t fold to the data source. Highlights the importance of query folding to offload work to the backend, helping avoid local memory pressure. Encourages optimizing steps to maintain folding or perform de-duplication at the source for better performance and reliability.

  https://learn.microsoft.com/en-us/power-query/working-with-duplicates