# VPC Setup with Terraform

## Overview
This repository contains Terraform code to create a Virtual Private Cloud (VPC) in AWS with a CIDR block of `10.42.0.0/16`.


# vpc.tf file contains these set of instruction-
Subnets for isolating resources and improving security.
Internet Gateway and Route Tables for routing internet traffic.
NAT Gateway for internet access from private subnets.


## Requirements
- Terraform installed on your local machine
- AWS CLI configured with appropriate credentials

## Setup Instructions

1. Clone the repository:
   ```bash
   git clone <repository-url>
   cd <repository-name>

2. Initialize Terraform:
terraform init
3.	Plan the deployment:
terraform plan
4.	Apply the deployment:
terraform apply
5.	Review the output for VPC and subnet IDs.

Assumptions

•This setup assumes a single Availability Zone for simplicity.
Subnets: Divided into public and private subnets to segregate resources.
Internet Gateway: For routing internet traffic from the public subnet.
NAT Gateway: Allows outbound internet access from the private subnet.
Security Groups: For controlling inbound and outbound traffic to ensure secure access.
Tags: Included for resource identification and management.

Best Practices
•	Use meaningful names for resources.
•	Structure your code in a modular format for scalability.
