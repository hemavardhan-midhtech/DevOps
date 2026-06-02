# VPC (Virtual Private Cloud)

## What is VPC?

A Virtual Private Cloud is a logically isolated network in AWS.

Allows you to control:

* IP Address Range
* Subnets
* Routing
* Security

---

# VPC Architecture

Internet
↓
Internet Gateway
↓
VPC
├── Public Subnet
└── Private Subnet

---

# CIDR Block

Defines IP Range.

Example:

```text
10.0.0.0/16
```

Provides:

65,536 IP Addresses

---

# Subnets

## Public Subnet

Has route to Internet Gateway.

Examples:

* Load Balancer
* Bastion Host

---

## Private Subnet

No direct internet access.

Examples:

* Databases
* Internal Applications

---

# Internet Gateway

Allows internet communication.

Attach to VPC.

---

# Route Table

Determines traffic flow.

Example:

Destination: 0.0.0.0/0

Target: Internet Gateway

---

# NAT Gateway

Allows private subnet access to internet.

Used for:

* Software Updates
* Package Downloads

Without exposing servers publicly.

---

# Network ACL

Subnet-level firewall.

Supports:

Allow
Deny

Rules

---

# Security Group

Instance-level firewall.

Supports:

Allow Only

---

# VPC Flow Logs

Capture network traffic.

Used for troubleshooting.

---

# AWS CLI Commands

List VPCs:

```bash
aws ec2 describe-vpcs
```

List Subnets:

```bash
aws ec2 describe-subnets
```

List Route Tables:

```bash
aws ec2 describe-route-tables
```

---

# Interview Questions

Q: What is a VPC?

A: A logically isolated virtual network in AWS.

Q: Difference between Public and Private Subnet?

A: Public subnet has internet access; private subnet does not.

Q: Why use NAT Gateway?

A: Allows outbound internet access from private subnet resources.

Q: Difference between NACL and Security Group?

A:

* NACL → Subnet Level
* Security Group → Instance Level

---

# Hands-On Lab

1. Create VPC
2. Create Public Subnet
3. Create Private Subnet
4. Attach Internet Gateway
5. Configure Route Tables
6. Launch EC2
7. Test Connectivity
