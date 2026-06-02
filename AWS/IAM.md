# EC2 (Elastic Compute Cloud)

## What is EC2?

Amazon EC2 provides scalable virtual servers in the cloud.

Used to host:

* Applications
* APIs
* Jenkins
* Docker
* Kubernetes Nodes

---

# EC2 Architecture

User
↓
Internet
↓
Security Group
↓
EC2 Instance

---

# Key Components

## AMI

Amazon Machine Image

Templates used to launch instances.

Examples:

* Ubuntu
* Amazon Linux
* RedHat

---

## Instance Types

General Purpose:

t2.micro

Compute Optimized:

c5.large

Memory Optimized:

r5.large

---

## Security Groups

Virtual Firewall.

Controls:

* Inbound Traffic
* Outbound Traffic

Example:

SSH → Port 22

HTTP → Port 80

HTTPS → Port 443

---

## Key Pair

Used for SSH access.

Public Key

Private Key

---

## Elastic IP

Static Public IP.

---

## EBS

Elastic Block Storage

Persistent storage attached to EC2.

---

# EC2 Lifecycle

Pending
↓
Running
↓
Stopping
↓
Stopped
↓
Terminated

---

# AWS CLI Commands

Launch Instance:

```bash
aws ec2 run-instances
```

List Instances:

```bash
aws ec2 describe-instances
```

Stop Instance:

```bash
aws ec2 stop-instances
```

Start Instance:

```bash
aws ec2 start-instances
```

Terminate Instance:

```bash
aws ec2 terminate-instances
```

---

# SSH Access

```bash
ssh -i key.pem ubuntu@public-ip
```

---

# Interview Questions

Q: Difference between Security Group and NACL?

A: Security Group is instance-level. NACL is subnet-level.

Q: What is AMI?

A: Template used to launch EC2 instances.

Q: What is EBS?

A: Persistent block storage for EC2.

---

# Hands-On Lab

1. Launch EC2
2. Create Key Pair
3. Configure Security Group
4. SSH into Instance
5. Install Nginx
6. Create AMI
