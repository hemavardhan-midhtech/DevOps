
1. VPC Public/Private Architecture
Internet
    │
    ▼
Internet Gateway
    │
    ▼
┌──────────────────────────┐
│          VPC             │
│                          │
│ Public Subnet            │
│ ┌─────────────────────┐  │
│ │ ALB / Bastion Host  │  │
│ └─────────────────────┘  │
│                          │
│ Private Subnet           │
│ ┌─────────────────────┐  │
│ │ EC2 Application     │  │
│ └─────────────────────┘  │
│                          │
│ Private DB Subnet        │
│ ┌─────────────────────┐  │
│ │ RDS MySQL           │  │
│ └─────────────────────┘  │
└──────────────────────────┘

2. S3 Static Website
User
  │
  ▼
Route53
  │
  ▼
CloudFront
  │
  ▼
S3 Bucket

3. CloudWatch Monitoring

EC2
RDS
Lambda
  │
  ▼
CloudWatch
  │
  ▼
Alarm
  │
  ▼
SNS
  │
  ▼
Email Alert
