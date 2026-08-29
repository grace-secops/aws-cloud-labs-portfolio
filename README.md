 AWS Cloud Labs Portfolio

Hands-on AWS cloud labs demonstrating practical experience with identity and access management, networking, compute, storage, databases, load balancing, and Auto Scaling.

 About

This repository documents my hands-on work with Amazon Web Services (AWS) through practical cloud infrastructure labs.

The labs focus on configuring AWS services, understanding how different cloud components work together, applying access controls, and building infrastructure designed for availability and scalability.

 AWS Services and Skills Demonstrated

* AWS Identity and Access Management (IAM)
* Amazon VPC
* Amazon EC2
* Amazon EBS
* Amazon RDS
* Application Load Balancer
* EC2 Launch Templates
* Auto Scaling Groups
* Amazon CloudWatch
* Security groups
* IAM policies and permissions
* Cloud infrastructure configuration
* High availability and scalability

 Labs

 1. AWS IAM

Explored IAM users, groups, managed policies, and inline policies, then assigned users to groups according to their job responsibilities.

Key activities:

* Examined IAM users and groups
* Reviewed IAM policies and permissions
* Assigned users to appropriate groups
* Tested permissions using different IAM users
* Verified read-only and administrative access

[View IAM Lab](./01-iam/iam-lab-report.md)

---

 2. VPC and Web Server

Configured a virtual network environment and deployed an EC2 web server within the AWS environment.

Key activities:

* Configured VPC networking
* Worked with subnets and security groups
* Launched an EC2 instance
* Configured web server access
* Tested connectivity to the deployed server

[View VPC and Web Server Lab](./02-vpc-web-server/vpc-web-server-report.md)

---

 3. Amazon EC2

Worked with Amazon EC2 to launch and configure a virtual server.

Key activities:

* Launched an EC2 instance
* Installed and configured Apache
* Modified the EC2 instance type
* Increased the root EBS volume size
* Verified the running web server

[View EC2 Lab](./03-ec2/ec2-lab-report.md)

---

 4. Amazon EBS

Configured Elastic Block Store (EBS) storage and attached it to an EC2 instance.

Key activities:

* Created an EBS volume
* Attached the volume to an EC2 instance
* Formatted and mounted the volume
* Configured persistent mounting
* Created and restored an EBS snapshot

[View EBS Lab](./04-ebs/ebs-lab-report.md)

---

 5. Amazon RDS

Configured a relational database environment using Amazon RDS and connected an application to the database.

Key activities:

* Created a database security group
* Configured an RDS subnet group
* Created an RDS database
* Configured database connectivity
* Connected the application to the database

[View RDS Lab](./05-rds/rds-lab-report.md)

---

 6. Load Balancing and Auto Scaling

Configured an application environment using an Application Load Balancer, EC2 Launch Template, Target Group, and Auto Scaling Group.

Key activities:

* Created an Amazon Machine Image (AMI)
* Created an EC2 Launch Template
* Configured a Target Group
* Created an Application Load Balancer
* Configured an Auto Scaling Group
* Set desired capacity to 2 instances
* Configured minimum capacity of 2 and maximum capacity of 6
* Enabled CloudWatch monitoring

[View Load Balancing and Auto Scaling Lab](./06-load-balancing-auto-scaling/load-balancing-auto-scaling.md)

---

 Cloud Infrastructure Workflow

Together, these labs demonstrate a practical progression through core AWS infrastructure concepts:

1. Identity and Access Management** — Control access to AWS resources using IAM users, groups, and policies.
2. Networking — Build and configure a virtual network environment using Amazon VPC.
3. Compute — Deploy and configure EC2 instances to host applications and services.
4. Storage — Attach and manage persistent EBS storage and snapshots.
5. Databases — Deploy and connect to a managed relational database using Amazon RDS.
6. Availability and Scalability — Distribute traffic and automatically manage EC2 capacity using an Application Load Balancer and Auto Scaling.

 Key Learning

These labs strengthened my practical understanding of AWS infrastructure and how individual cloud services work together.

I gained hands-on experience configuring access controls, networking, compute resources, storage, managed databases, load balancing, and Auto Scaling.

The exercises also reinforced important cloud concepts including **least-privilege access, resource availability, scalability, monitoring, and infrastructure resilience**.

 Lab Environment

The work documented in this repository was completed in an authorized AWS lab environment for practical learning and experimentation.

Resources were created and configured within the provided AWS environment.

 Repository Structure

```text
aws-cloud-labs-portfolio/
│
├── README.md
│
├── 01-iam/
│   └── iam-lab-report.md
│
├── 02-vpc-web-server/
│   └── vpc-web-server-report.md
│
├── 03-ec2/
│   └── ec2-lab-report.md
│
├── 04-ebs/
│   └── ebs-lab-report.md
│
├── 05-rds/
│   └── rds-lab-report.md
│
└── 06-load-balancing-auto-scaling/
    └── load-balancing-auto-scaling.md
```


