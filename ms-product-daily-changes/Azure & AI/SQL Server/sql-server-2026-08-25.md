# SQL Server
**Date created:** 2026-08-25 UTC  
**Tags:** Best Practices, Get Started, Guidance, Monitoring, Security  

## Major Changes

- **Appliance installation and configuration for Analytics Platform System**

  Reworked the closing guidance by replacing the Next steps section and removing a detailed post-installation task table. The page now focuses on a concise Related content section that links to Admin Console monitoring and component health state documentation. This streamlines the article and directs readers to current monitoring resources.

  https://learn.microsoft.com/en-us/sql/analytics-platform-system/appliance-installation-and-configuration-overview?view=aps-pdw-2016-au7

## Moderate Changes

- **ALTER TABLE (Transact-SQL)**

  Added a tip recommending TRUNCATE TABLE with the WITH (PARTITIONS (...)) clause to clear rows from specific partitions without dropping or switching partitions. This provides a simpler alternative to certain ALTER TABLE scenarios and helps reduce risk during partition maintenance.

  https://learn.microsoft.com/en-us/sql/t-sql/statements/alter-table-transact-sql?view=sql-server-ver17

- **Deploy a Model Deployment Package by Using the Wizard**

  Consolidated Next Steps and See also into a single Related content section and updated links. Removed a prior note stating that file attributes and user/group permissions aren’t included in model deployment packages. The revised layout makes related guidance easier to find.

  https://learn.microsoft.com/en-us/sql/master-data-services/deploy-a-model-deployment-package-by-using-the-wizard?view=sql-server-ver16

- **Email a Shortcut Query File (MDS Add-in for Excel)**

  Removed Next steps guidance about recipients needing the MDS Excel add-in and opening files by double-clicking. Replaced See also with a streamlined Related content section while retaining the link to Shortcut Query Files, improving consistency and navigation.

  https://learn.microsoft.com/en-us/sql/master-data-services/microsoft-excel-add-in/email-a-shortcut-query-file-mds-add-in-for-excel?view=sql-server-ver16

- **Microsoft Drivers for PHP for SQL Server**

  Reworked the “Choose your starting point” section from a table to a concise, task-oriented bullet list. Removed the Quick connect section, including the PDO end-to-end sample and guidance on passwordless connections (Authentication DSN options) and local TLS handling (TrustServerCertificate). The page now emphasizes clearer navigation and a production-focused starting point.

  https://learn.microsoft.com/en-us/sql/connect/php/microsoft-php-driver-for-sql-server?view=sql-server-ver17

- **RENAME (Transact-SQL)**

  Corrected the RENAME DATABASE syntax by adding a missing closing bracket in the signature. This fix improves the accuracy and reliability of the reference.

  https://learn.microsoft.com/en-us/sql/t-sql/statements/rename-transact-sql?view=aps-pdw-2016-au7

- **Install Machine Learning Server (Standalone) or R Server (Standalone) using SQL Server Setup**

  Reorganized closing sections by replacing Next steps with a moniker-scoped Related tasks section (SQL Server 2017+) highlighting Python tutorials, and added a separate Related content section with updated R resources. Link texts were refreshed for clarity to help readers find the right tutorials faster.

  https://learn.microsoft.com/en-us/sql/machine-learning/install/sql-machine-learning-standalone-windows-install?view=sql-server-ver15

- **Deploy the R model and use it in SQL Server (walkthrough)**

  Replaced the Next steps section with a concise Related content list. Removed narrative suggestions for creating additional models and broader sample links, and added direct links to Python tutorials for SQL machine learning and an R tutorial on NYC taxi fare prediction. This improves discoverability of the most relevant, up-to-date tutorials.

  https://learn.microsoft.com/en-us/sql/machine-learning/tutorials/walkthrough-deploy-and-use-the-model?view=sql-server-ver17