# 🏗️ Elastic WordPress Evolution – AWS Architecture Lab

This project demonstrates how to deploy a **highly available**, **scalable**, and **secure WordPress environment** on AWS using core services such as EC2, RDS (Multi-AZ), S3, and CloudFormation. It is ideal for learning and showcasing real-world cloud architecture for hosting dynamic web applications.

---

## 📌 Table of Contents
- [Architecture Overview](#architecture-overview)
- [Key Features](#key-features)
- [AWS Services Used](#aws-services-used)
- [Deployment Steps](#deployment-steps)
- [Security Practices](#security-practices)
- [Challenges Faced](#challenges-faced)
- [Author](#author)

---

## 🏛️ Architecture Overview

```
User ↔️ Route 53 (DNS)
     ↕
ALB (Load Balancer)
     ↕
Auto Scaling Group
     ↕
EC2 Instances (Apache + WordPress + PHP)
     ↕
Amazon RDS (MySQL, Multi-AZ)
     ↕
Amazon S3 (shared media content)
```

All components are inside a custom **VPC** with public and private subnets, NAT Gateway, and Internet Gateway.

---

## ✨ Key Features
- High availability using **Multi-AZ RDS**
- Auto-scaling and fault tolerance with **EC2 + ALB**
- Shared media storage on **S3**
- Infrastructure as Code using **CloudFormation**
- Monitoring via **CloudWatch**
- Fine-grained access control with **IAM** and **Security Groups**

---

## 🧰 AWS Services Used
- EC2 (Amazon Linux 2)
- RDS (MySQL, Multi-AZ)
- S3 (static file hosting)
- CloudFormation (infrastructure provisioning)
- IAM (permissions & roles)
- VPC (custom networking)
- Security Groups (firewall rules)
- Route 53 (optional DNS)
- CloudWatch (logs & monitoring)

---

## 🚀 Deployment Steps (High Level)
1. Launch RDS with MySQL, enable Multi-AZ.
2. Create S3 bucket for media storage.
3. Deploy EC2 instance with Apache + WordPress via user data script.
4. Configure ALB and Auto Scaling Group via Launch Template.
5. Use CloudFormation to automate infrastructure provisioning.
6. Edit wp-config.php to connect WordPress to RDS.
7. Access WordPress via browser and complete the setup.

---

## 🔒 Security Practices
- Restricted inbound rules via Security Groups
- Private subnets for RDS
- Password-based authentication for DB
- IAM role policies scoped to least privilege
- Lifecycle rules for S3 cleanup

---

## 🧗 Challenges Faced
- Troubleshooting “Error establishing database connection”
- Editing `wp-config.php` correctly for external RDS
- Configuring user data for Apache + PHP
- Granting MySQL user permissions via terminal

---

## 👩‍💻 Author

**Sonali Gupta**  
GitHub: [Sonalii3129](https://github.com/Sonalii3129)  
LinkedIn: [linkedin.com/in/sonalii3129](https://linkedin.com/in/sonalii3129)  
