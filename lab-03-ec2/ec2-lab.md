# AWS EC2 Lab

## Objective

To deploy and manage an Amazon EC2 instance and gain practical experience with cloud-based compute resources.

The purpose of this exercise was to understand how EC2 instances are launched, configured, resized, and connected to persistent storage.

## AWS Services

* Amazon EC2
* Amazon EBS
* Security Groups

## Lab Environment

* AWS Management Console
* Controlled AWS lab environment
* AWS Region: US East (N. Virginia)

 EC2 Instance Deployment

An Amazon EC2 instance was launched and configured within the AWS environment.

The instance was used to explore basic compute management tasks, including installing a web server and modifying the instance configuration.

 Web Server Configuration

Apache HTTP Server was installed on the EC2 instance.

The web server was configured and tested to confirm that the instance was able to run a web application service.

This provided practical experience with deploying a service on an AWS cloud-based server.

 Instance Resizing

The EC2 instance type was changed from:

**t2.micro → t2.small**

This demonstrated how EC2 instance types can be modified to provide different levels of compute resources.

 EBS Root Volume Modification

The root EBS volume attached to the EC2 instance was increased from:

8 GiB → 10 GiB

This demonstrated how storage capacity can be adjusted as workload requirements change.

 Key Learning

This exercise helped me understand the basic lifecycle of an EC2 instance, from deployment and configuration to resource modification.

I gained practical experience installing software on a cloud server, changing instance types, and increasing attached storage capacity.

The lab also reinforced the relationship between EC2 compute resources and EBS storage.

 Security Considerations

When deploying EC2 instances, access should be controlled through appropriately configured security groups.

Only required ports and services should be exposed, and administrative access should be restricted to authorized users.

 Conclusion

The EC2 lab provided practical experience managing cloud compute resources in AWS.

I learned how to launch an EC2 instance, configure a web server, resize compute capacity, and increase attached storage to meet changing workload requirements.
