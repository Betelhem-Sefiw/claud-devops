# Amazon RDS Database Deployment

**Name:** Bethelehem Sefiw
**ID:** ETS 0285/17
**Class:** Software Engineering
**Year:** 3rd Year

---

## Overview
This document outlines the deployment and configuration of an Amazon RDS (Relational Database Service) MySQL instance.

## Database Configuration
- **Engine:** MySQL 8.0
- **DB Instance Identifier:** `myDB`
- **Instance Class:** `db.t3.micro` (Burstable class)
- **Master Username:** `admin`
- **Initial Database Name:** `myDB`
- **Public Access:** Disabled (No)

## Network & Security Setup
- **Subnet Group:** Created `my subnet group` to place the database in private subnets across multiple Availability Zones.
- **Security Group:** Assigned the `Database` security group.
- **Inbound Rules:** Configured to allow traffic only on port `3306` (MySQL/Aurora) originating exclusively from the Web Server's security group. This ensures the database remains isolated from public internet access.

## Status
- **Deployment:** Complete (Status: Available)
- **Endpoint:** `mydb.cq9g1tqphzx4.us-west-2.rds.amazonaws.com`