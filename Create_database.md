# Creating MySQL Databases for Pharmacy Management System

This guide provides instructions on how to install MySQL and create two databases, `pharma` and `pharmacy`, along with their respective table structures.

## Install MySQL

1. **Install MySQL**: Visit the [MySQL Downloads](https://dev.mysql.com/downloads/mysql/) page, download the MySQL Installer suitable for your operating system, and follow the installation instructions.Then use MySQL Workbench to create databases.

2. **Create the Databases**:

   ```sql
   CREATE DATABASE anyname;
  


   
### `pharma` Table

```sql
CREATE TABLE pharma (
   Ref INT NOT NULL PRIMARY KEY,
   MedName VARCHAR(45) NOT NULL
);
```



### `pharmacy` Table
 ```sql
CREATE TABLE pharmacy (
   Ref_no INT NOT NULL,
   CmpName VARCHAR(45) NOT NULL,
   Typemed VARCHAR(50) NOT NULL,
   LotNo INT NOT NULL PRIMARY KEY,
   Issuedate DATE NOT NULL,
   Expdate DATE NOT NULL,
   Sideeffect VARCHAR(45) NOT NULL,
   warning VARCHAR(45) NOT NULL,
   Dosage INT NOT NULL,
   Price INT NOT NULL,
   qty INT NOT NULL,
   medname VARCHAR(45) NOT NULL,
   uses VARCHAR(45) NOT NULL
);
