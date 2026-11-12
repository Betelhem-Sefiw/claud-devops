# Amazon VPC Network Infrastructure

**Name:** Bethelehem Sefiw

**ID:** ETS 0285/17
**Department:** Software Engineering
**Year:** 3rd Year

---

## Overview
This document outlines the design and configuration of the Amazon Virtual Private Cloud (VPC) and its associated networking components.

## VPC Configuration
- **VPC Name:** `My VPC`
- **CIDR Block:** `10.0.0.0/16`

## Subnet Setup
- **Public Subnet:** `Public 1` (`10.0.1.0/24`) - Configured with auto-assign public IPv4 to host internet-facing resources like the Web Server.
- **Private Subnets:** 
  - `Private 1` (`10.0.2.0/24`) - Created in the first Availability Zone.
  - `Private 2` (`10.0.3.0/24`) - Created in the second Availability Zone for high availability.

## Internet Gateway & Routing
- **Internet Gateway:** Created `My IG` and attached it to the VPC.
- **Route Table:** Configured the public route table with a destination of `0.0.0.0/0` targeting `My IG`. Associated this route table with the `Public 1` subnet to allow external internet access.

## Status
- **VPC Setup:** Complete
- **Network Architecture:** Isolated private subnets secured, with a public subnet ready for server deployment.