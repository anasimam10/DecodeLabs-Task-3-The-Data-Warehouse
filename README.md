# DecodeLabs-Project-3-The-Data-Warehouse

## Overview

A cloud database project using **AWS RDS MySQL** to store and manage intern records. The project demonstrates database creation, table management, data insertion, and data persistence.

## Technologies

* AWS RDS (MySQL)
* Ubuntu Linux (VirtualBox)
* MySQL Command-Line Client

## Database Structure

**Database:** `internsdb`
**Table:** `Interns`

| Column | Data Type                  |
| ------ | -------------------------- |
| Name   | VARCHAR(100)               |
| Role   | VARCHAR(100)               |
| Email  | VARCHAR(255) — Primary Key |

## SQL Commands

```sql
CREATE DATABASE internsdb;
USE internsdb;

CREATE TABLE Interns (
    Name VARCHAR(100) NOT NULL,
    Role VARCHAR(100) NOT NULL,
    Email VARCHAR(255) PRIMARY KEY
);

INSERT INTO Interns (Name, Role, Email) VALUES
('Ali Khan', 'Cloud Intern', 'ali@example.com'),
('Sara Ahmed', 'Database Intern', 'sara@example.com'),
('Ahmed Raza', 'DevOps Intern', 'ahmed@example.com');

SELECT * FROM Interns;
```

## Key Learning Outcomes

* Provisioning a managed cloud database.
* Connecting to AWS RDS from Ubuntu.
* Creating tables and inserting records.
* Verifying data persistence after reconnecting.

## Screenshots

See the `screenshots` folder for project evidence.

**Note:** Database credentials and AWS secrets are not included in this repository.
