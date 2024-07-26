Microsoft SQL Server Management Studio (SSMS) is a powerful tool for managing SQL Server databases, but it does not directly handle database encryption by itself. 
Instead, SQL Server, the database engine behind SSMS, provides several mechanisms for implementing encryption.
Here’s a detailed description of the main encryption features you can use with SQL Server, which you would configure through SSMS:

1. Transparent Data Encryption (TDE)
Overview:

Purpose: TDE encrypts the entire database at the storage level, protecting data at rest. 
This means the data files on disk are encrypted, which helps to protect against unauthorized physical access.
Encryption Method: TDE uses a combination of a Database Encryption Key (DEK) and a master key.
The DEK is protected by a certificate that is stored in the master database.
