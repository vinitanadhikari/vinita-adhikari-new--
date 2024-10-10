# EC2 Auto-Scaling Group Setup with Terraform

## Overview
This section adds an Auto-Scaling Group to the previously created VPC.

Key components in this setup:
Launch Configuration: Defines the instance configuration.
Auto-Scaling Group: Manages the scaling of instances.
Load Balancer (Application Load Balancer): Distributes incoming traffic.
Target Group: Registers instances for receiving traffic.
Security Group: Controls traffic to instances.

## Requirements
- Ensure the VPC is created as described in Task 1.

## Setup Instructions

1. Navigate to the repository:
   ```bash
   cd <repository-name>

2. Initialize Terraform:
terraform init
3.	Plan the deployment:
terraform plan
4.	Apply the deployment:
terraform apply

Assumptions
•The EC2 instances will be using a public subnet for web traffic.
•Auto-scaling is configured to scale between 1 and 3 instances based on demand.

Best Practices
•Use lifecycle blocks to prevent disruptions during updates.
•Implement scaling policies to maintain performance during traffic fluctuations.

Note :-

This setup ensures scalability and high availability of your application.
ensure your AWS credentials are properly set up. 