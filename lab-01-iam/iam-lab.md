 AWS IAM Lab

 Objective

To explore AWS Identity and Access Management (IAM) and understand how users, groups, and policies can be used to control access to AWS resources.

The exercise focused on applying permissions according to different user responsibilities and testing how IAM policies affect access to AWS services.

 AWS Service

Amazon Web Services — Identity and Access Management (IAM)

 Lab Environment

* AWS Management Console
* AWS IAM
* Pre-created IAM users and groups
* Controlled AWS lab environment

 IAM Users

The lab provided three IAM users:

* `user-1`
* `user-2`
* `user-3`

Each user was assigned a different role based on the business scenario.

 IAM Groups

The following groups were provided:

* S3-Support
* EC2-Support
* EC2-Admin

 Policies Examined

 S3-Support

The AmazonS3ReadOnlyAccess managed policy was attached to this group.

This policy provides read-only access to Amazon S3 resources.

 EC2-Support

The AmazonEC2ReadOnlyAccess managed policy was attached to this group.

This policy allows users to view information about EC2 and related resources without making changes.

 EC2-Admin

This group used an inline policy that allowed users to view EC2 information and start or stop EC2 instances.

 User-to-Group Assignment

The users were assigned to groups according to their responsibilities:

| IAM User | Group       | Access                              |
| -------- | ----------- | ----------------------------------- |
| `user-1` | S3-Support  | Read-only S3 access                 |
| `user-2` | EC2-Support | Read-only EC2 access                |
| `user-3` | EC2-Admin   | View, start, and stop EC2 instances |

 Permission Testing

The permissions were tested by signing in as each IAM user.

 User-1 — S3 Support

`user-1` was able to access Amazon S3 and view the available bucket.

When attempting to access EC2 resources, the user received an authorization error because the assigned policy did not provide EC2 permissions.

 User-2 — EC2 Support

`user-2` was able to view EC2 resources because the user had read-only EC2 permissions.

An attempt was made to stop an EC2 instance, but the operation was denied.

This demonstrated that read-only permissions allow users to view resources without modifying them.

 User-3 — EC2 Administrator

`user-3` was assigned to the EC2-Admin group.

The user was able to access EC2 resources and successfully stop the designated EC2 instance.

 Security Concept Demonstrated

This lab demonstrated the principle of least privilege.

Instead of giving every user full access to the AWS account, permissions were assigned according to each user's responsibilities.

This reduces the potential impact of unauthorized or accidental actions.

 Key Learning

This exercise helped me understand how AWS IAM controls access to cloud resources through users, groups, and policies.

I learned the difference between managed policies and inline policies and how permissions can be tested by attempting authorized and unauthorized actions.

The lab also reinforced the importance of applying least-privilege access when managing cloud environments.

 Conclusion

The IAM lab provided practical experience with identity and access management in AWS.

I successfully explored IAM users and groups, examined policies, assigned users to appropriate groups, and tested how different permission levels affected access to AWS services.
