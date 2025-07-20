# Elastic WordPress Evolution – AWS Architecture Lab

## 📌 Project Summary
This project demonstrates the design and deployment of a highly available, auto-scaling WordPress application on AWS. It simulates a real-world cloud infrastructure for hosting web applications using services like EC2, RDS (Multi-AZ), Elastic Load Balancer, S3, and CloudFormation.

## 🔧 Tools & Technologies Used
- Amazon EC2 (Amazon Linux 2)
- Elastic Load Balancer (ALB)
- Amazon RDS (MySQL, Multi-AZ)
- Amazon S3
- Virtual Private Cloud (VPC)
- IAM Roles & Security Groups
- CloudFormation
- Auto Scaling Groups
- Route 53
- CloudWatch
- Bash Scripts

## ⚙️ Architecture Overview
1. Custom VPC with public and private subnets.
2. EC2 instances launched with User Data scripts for automated WordPress installation.
3. Application Load Balancer to manage traffic across EC2 instances.
4. RDS Multi-AZ MySQL for high availability database.
5. S3 used for shared content storage with lifecycle management policies.
6. CloudFormation templates for infrastructure automation.
7. IAM roles for secure access and resource permissions.
8. Route 53 for DNS routing and CloudWatch for performance monitoring.

## 📁 Project Files (What’s Included)
- Word documents explaining the full implementation.
- CloudFormation scripts (optional if uploaded).
- Screenshots of key configuration steps and dashboard views.
- `README.md` to guide users on the setup and usage.

## ✅ Key Learning Outcomes
- Understanding of AWS infrastructure design for web hosting.
- Real-world WordPress deployment architecture.
- Integration between EC2 and RDS via secure configuration.
- Troubleshooting Linux server issues and configuring services.
- Writing reusable infrastructure-as-code using CloudFormation.

## 📸 Recommended Additions
To make this repository even more helpful for viewers:
- Add `screenshots/` folder with terminal, EC2, WordPress dashboard images
- Include the bash script used in EC2 User Data
- Add example `cloudformation-template.yaml` (if available)
