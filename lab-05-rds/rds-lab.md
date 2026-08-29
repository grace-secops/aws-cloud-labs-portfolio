 AWS RDS Lab

 Objective

To configure and connect to an Amazon Relational Database Service (RDS) database within a controlled AWS environment.

The purpose of this exercise was to understand how a managed relational database can be deployed in AWS and securely accessed by an application.

 AWS Services

* Amazon RDS
* Amazon VPC
* Security Groups
* DB Subnet Groups

 Lab Environment

* AWS Management Console
* Controlled AWS lab environment
* AWS Region: US East (N. Virginia)

 Database Security Group

A security group was created and configured for the RDS database.

The security group was used to control network traffic to the database and determine which resources were permitted to communicate with it.

 DB Subnet Group

A DB subnet group was created using subnets within the VPC.

The subnet group defines the network locations where the RDS database can be deployed and helps integrate the database with the existing VPC architecture.

 RDS Database Deployment

An RDS database instance was created using the configured networking and security settings.

The database was deployed as a managed AWS service, allowing AWS to handle underlying infrastructure tasks such as database hosting and maintenance.

 Application Connectivity

The application was configured to communicate with the RDS database.

The connection was tested successfully, demonstrating that the application could communicate with the database through the configured network and security controls.

 Security Considerations

Database access should be restricted to only the resources and ports that require connectivity.

Security groups should not unnecessarily expose database services to the public internet.

Using private networking and least-privilege access helps reduce the attack surface of database infrastructure.

 Key Learning

This exercise helped me understand how Amazon RDS integrates with VPC networking and security groups.

I gained practical experience creating a DB subnet group, configuring database access controls, deploying an RDS database, and connecting an application to the database.

The lab also reinforced the importance of protecting database resources through network segmentation and appropriate access controls.

 Conclusion

The RDS lab provided practical experience deploying and connecting to a managed relational database in AWS.

It demonstrated how RDS can be integrated with application infrastructure while using VPC networking and security groups to control database access.
