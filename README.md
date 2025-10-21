# CDK Website Lab: EC2 + RDS Deployment

This project uses AWS Cloud Development Kit (CDK) in TypeScript to deploy a simple web application architecture. It includes a VPC with public and private subnets, EC2 instances for web servers, and an RDS MySQL database—all provisioned across two availability zones.

## 📦 Stack Overview

### ✅ Network Configuration
- VPC with:
  - public subnets (1 per AZ)
  - private subnets (1 per AZ)

### ✅ Server Configuration
- EC2 Instances:
  - web server in each public subnet
  - Amazon Linux 2 AMI
  - Security group allows HTTP (port 80) from anywhere
- RDS Instance:
  - MySQL engine (version 8.0)
  - Deployed in private subnets
  - Security group allows MySQL (port 3306) only from EC2 security group

## 🚀 Deployment Instructions

### 1. Clone the Repository
```bash

https://github.com/Makarious20/CDK-ec2-rds-lib.git

cd cdk-website-lab
