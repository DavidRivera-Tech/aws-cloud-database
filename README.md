# AWS Cloud Database Deployment

Infrastructure Project | AWS Cloud | RDS Database

## Project Overview

This project demonstrates the deployment and configuration of a cloud-based relational database using Amazon RDS. The project includes database provisioning, network access configuration, and successful connection to the database using a client tool to execute SQL queries.

## Technologies and Services Used

- Amazon RDS (MySQL)
- AWS Security Groups
- Amazon VPC (default networking)
- MySQL Workbench
- SQL (Structured Query Language)

## Objectives

- Deploy a managed relational database in AWS using RDS
- Configure secure access to the database
- Connect to the database using a client tool
- Create tables, insert data, and retrieve results using SQL

## Deployment Summary

An RDS MySQL database instance was created using the AWS free tier configuration. The database was configured with public access and secured using a security group allowing inbound traffic on port 3306 from a specific IP address.

A connection was established using MySQL Workbench, where SQL commands were executed to create a table, insert data, and retrieve records successfully.

## Skills Demonstrated

- RDS database provisioning
- Cloud networking and security configuration
- Database connectivity setup
- SQL query execution (CREATE, INSERT, SELECT)
- Cloud database validation and testing

## Architecture

The diagram below illustrates the architecture used in this project. A user connects from a local machine to an Amazon RDS MySQL database instance over port 3306. Access is controlled through an AWS Security Group that restricts inbound traffic to a specific IP address.

![AWS RDS Architecture](https://chatgpt.com/c/architecture/aws-rds-architecture-diagram.png)

## Screenshots

### 1. RDS Database Created

Shows the deployed RDS database instance with status available.

![RDS Database](https://chatgpt.com/c/screenshots/rds-database-created.png)

### 2. Database Configuration

Shows the database endpoint, port, networking configuration, and public accessibility settings.

![RDS Configuration](https://chatgpt.com/c/screenshots/rds-configuration.png)

### 3. Security Group Configuration

Shows the inbound rule allowing MySQL access on port 3306 from a specific IP address.

![Security Group](https://chatgpt.com/c/screenshots/security-group-mysql.png)

### 4. SQL Query Result

Shows successful execution of SQL commands including table creation, data insertion, and data retrieval.

![SQL Query Result](https://chatgpt.com/c/screenshots/sql-query-result.png)

## Repository Structure

```text
aws-cloud-database
├── README.md
├── screenshots
│   ├── rds-database-created.png
│   ├── rds-configuration.png
│   ├── security-group-mysql.png
│   └── sql-query-result.png
└── architecture
    └── aws-rds-architecture-diagram.png
```

## Outcome

This project demonstrates the successful deployment and use of a cloud-hosted relational database using AWS RDS. It validates the ability to configure secure access, establish connections, and perform database operations in a cloud environment.

## Future Improvements

Potential enhancements to this infrastructure include:

- integrating the database with a web application
- implementing automated backups and snapshots
- enabling Multi-AZ deployment for high availability
- managing infrastructure using Terraform or AWS CloudFormation