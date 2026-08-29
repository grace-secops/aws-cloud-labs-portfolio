 AWS Cloud Labs Portfolio

This repository documents my hands-on experience working with Amazon Web Services (AWS) through practical cloud infrastructure labs.

The labs were completed in a controlled AWS training environment and focused on core AWS services, cloud infrastructure, identity and access management, storage, databases, networking, and application scalability.

The purpose of this portfolio is to demonstrate my practical understanding of AWS services and my ability to configure, manage, troubleshoot, and document cloud infrastructure.

---

 Skills Demonstrated

* AWS Identity and Access Management (IAM)
* User and group management
* IAM policies and permissions
* Amazon VPC networking
* Amazon EC2 instance management
* Amazon EBS storage management
* Amazon RDS database configuration
* Load balancing
* Auto Scaling
* Security groups
* AMI creation
* Launch templates
* CloudWatch monitoring
* Cloud infrastructure troubleshooting
* Cloud security and least-privilege principles

---

 AWS Services Covered

* IAM — Identity and Access Management
* VPC — Virtual Private Cloud
* EC2 — Elastic Compute Cloud
* EBS — Elastic Block Store
* RDS — Relational Database Service
* Elastic Load Balancing
* Auto Scaling
* CloudWatch

---

 Completed Labs

 1. AWS IAM — Identity and Access Management

Explored IAM users, groups, managed policies, inline policies, and permission-based access.

Key Activities

* Explored pre-created IAM users and groups
* Inspected IAM managed policies
* Inspected inline policies
* Added users to appropriate IAM groups
* Tested permissions using different IAM users
* Used the IAM user sign-in URL
* Verified access restrictions between AWS services
* Demonstrated the principle of least privilege

 Business Scenario

Different users were assigned permissions based on their job responsibilities:

| User   | Group       | Permissions                         |
| ------ | ----------- | ----------------------------------- |
| user-1 | S3-Support  | Read-only Amazon S3 access          |
| user-2 | EC2-Support | Read-only Amazon EC2 access         |
| user-3 | EC2-Admin   | View, start, and stop EC2 instances |

 Key Learning

This lab demonstrated how IAM groups and policies can be used to control access to AWS resources according to a user's responsibilities.

[View IAM Lab](./lab-01-iam/iam-lab.md)

---

 2. Amazon VPC — Networking and Web Server

Configured networking infrastructure within an Amazon Virtual Private Cloud.

 Key Activities

* Worked with VPC networking
* Configured subnets
* Configured route tables
* Worked with security groups
* Configured internet connectivity
* Launched a web server within the VPC
* Tested network connectivity

 Key Learning

This lab improved my understanding of how AWS networking components work together to provide secure connectivity to cloud resources.

[View VPC Lab](./lab-02-vpc/vpc-lab.md)

---

 3. Amazon EC2 — Compute Infrastructure

Worked with Amazon EC2 to deploy and manage virtual servers in AWS.

 Key Activities

* Launched an EC2 instance
* Connected to the instance
* Installed and configured Apache
* Resized an EC2 instance
* Modified the root EBS volume
* Increased the root volume from **8 GiB to 10 GiB**
* Verified the running web server

 Key Learning

This lab provided practical experience managing cloud-based compute resources and understanding how instance types and storage configurations affect an EC2 workload.

[View EC2 Lab](./lab-03-ec2/ec2-lab.md)**

---

 4. Amazon EBS — Elastic Block Store

Configured persistent block storage for an EC2 environment.

 Key Activities

* Created an EBS volume
* Attached the volume to an EC2 instance
* Formatted the volume
* Mounted the volume
* Configured persistent mounting using `/etc/fstab`
* Created an EBS snapshot
* Restored storage from a snapshot

 Key Learning

This lab demonstrated how EBS provides persistent storage for EC2 instances and how snapshots can be used for backup and recovery.

[View EBS Lab](./lab-04-ebs/ebs-lab.md)

---

 5. Amazon RDS — Relational Database Service

Configured a relational database environment using Amazon RDS.

 Key Activities

* Created a database security group
* Configured an RDS subnet group
* Created an RDS database
* Configured database connectivity
* Connected an application to the database
* Verified database communication

 Key Learning

This lab demonstrated how Amazon RDS simplifies the deployment and management of relational databases while integrating with other AWS infrastructure.

[View RDS Lab](./lab-05-rds/rds-lab.md)

---

 6. Load Balancing and Auto Scaling

Configured an application environment designed for availability and scalability.

 Key Activities

* Created an Amazon Machine Image (AMI)
* Created a target group
* Configured an Application Load Balancer
* Created a launch template
* Created an Auto Scaling Group
* Configured desired capacity
* Configured minimum and maximum capacity
* Enabled CloudWatch monitoring
* Configured scaling policies
* Tested load balancing and instance scaling

 Auto Scaling Configuration

* Desired capacity: 2 instances
* Minimum capacity: 2 instances
* Maximum capacity: 6 instances

 Key Learning

This lab demonstrated how load balancing and Auto Scaling can be combined to improve application availability, distribute traffic, and automatically adjust compute capacity based on demand.

[View Load Balancing & Auto Scaling Lab](./lab-06-load-balancing/load-balancing-lab.md)**

---

 AWS Learning Journey

These six labs provided practical exposure to the major building blocks of AWS cloud infrastructure.

The progression followed this structure:

```text
IAM
 │
 ├── Identity and Access Management
 │
 ▼
VPC
 │
 ├── Networking and Security
 │
 ▼
EC2
 │
 ├── Compute
 │
 ▼
EBS
 │
 ├── Persistent Storage
 │
 ▼
RDS
 │
 ├── Managed Database
 │
 ▼
Load Balancing & Auto Scaling
     │
     └── Availability and Scalability
```

Together, these exercises helped me understand how AWS services can be combined to build, secure, manage, and scale cloud infrastructure.

---

 Security and Cloud Concepts

Throughout these labs, I gained practical exposure to important cloud security concepts including:

* Least-privilege access
* IAM policy management
* Network security
* Security groups
* Resource isolation
* Controlled access to cloud services
* Monitoring
* Availability
* Backup and recovery
* Infrastructure scalability

---

 Key Learning

These hands-on exercises strengthened my understanding of AWS infrastructure beyond theoretical learning.

I gained practical experience configuring AWS services, troubleshooting cloud resources, managing permissions, working with networking and storage, deploying databases, and designing infrastructure for availability and scalability.

The labs also reinforced the importance of security, least privilege, monitoring, backup strategies, and proper infrastructure configuration when working in a cloud environment.

---

 Lab Environment

The labs were completed using an AWS-provided training environment.

Primary platform: Amazon Web Services (AWS)

Region used during the labs: US East (N. Virginia / `us-east-1`)

Training platform: Vocareum

---

 Ethical and Training Notice

These labs were completed in an authorized AWS training environment provided for educational purposes.

All resources and activities documented in this repository were performed as part of hands-on cloud learning and experimentation.

