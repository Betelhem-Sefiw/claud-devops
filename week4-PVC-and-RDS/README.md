# Week 4: Cloud Infrastructure Setup

**Status:** ✅ Complete

---

## Part 1: VPC & Network Infrastructure
- Created a custom Virtual Private Cloud (VPC) with CIDR `10.0.0.0/16`.
- Set up a **Public Subnet** (for the Web Server) and two **Private Subnets** in different Availability Zones (for the Database).
- Attached an **Internet Gateway** and configured Route Tables to route public traffic.
- Associated the public route table with the `Public 1` subnet to allow internet access.

---

## Part 2: Amazon RDS Database
- Created a **DB Subnet Group** linking the two private subnets.
- Deployed a **MySQL 8.0** RDS instance (`myDB`) using `db.t3.micro`.
- Disabled public access (set to "No") to keep the database isolated.
- Configured **Security Groups**: Database (port 3306) only accepts traffic from the Web Server Security Group.

**Result:** Secure AWS environment ready for backend connection.nano 
