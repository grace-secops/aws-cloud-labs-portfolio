 Lab 6: Load Balancing and Auto Scaling

 Objective

To configure a highly available and scalable application environment using Amazon EC2, an Application Load Balancer, a Launch Template, and an Auto Scaling Group.

The purpose of this lab was to understand how AWS load balancing and Auto Scaling can be used together to distribute application traffic and automatically maintain the required number of EC2 instances.

 AWS Services Used

* Amazon EC2
* Application Load Balancer (ALB)
* EC2 Launch Template
* Auto Scaling Groups
* Amazon CloudWatch
* Target Groups

 Lab Environment

The lab was completed in the AWS environment provided for the exercise.

The configuration included multiple EC2 instances behind an Application Load Balancer, with an Auto Scaling Group responsible for maintaining the desired number of instances.

 Configuration

 1. Amazon Machine Image

An existing EC2 instance was used to create an Amazon Machine Image (AMI).

The AMI provided a reusable configuration that could be used by the Auto Scaling Group when launching additional EC2 instances.

 2. Launch Template

A Launch Template was created to define the configuration used when launching EC2 instances.

The template included the required instance configuration and enabled CloudWatch monitoring.

 3. Target Group

A target group was created to register the EC2 instances that would receive traffic from the Application Load Balancer.

The target group provided a way for the load balancer to monitor the registered instances and route traffic to healthy targets.

 4. Application Load Balancer

An Application Load Balancer was configured to distribute incoming application traffic across the available EC2 instances.

This improves availability by preventing traffic from depending on a single instance.

 5. Auto Scaling Group

An Auto Scaling Group was configured using the Launch Template.

The configuration used:

* Desired capacity:** 2 instances
* Minimum capacity:** 2 instances
* Maximum capacity:** 6 instances

This configuration allows the environment to maintain at least two instances while providing the ability to scale up to six instances when required.

 Auto Scaling Configuration

The Auto Scaling Group was configured to work with the Application Load Balancer and target group.

This allows newly launched instances to be automatically registered with the load balancer and participate in serving application traffic.

CloudWatch monitoring was also enabled to support monitoring and scaling activities.

 Result

The load balancing and Auto Scaling environment was successfully configured.

Two EC2 instances were maintained as the desired capacity, with the Auto Scaling Group configured to scale between two and six instances.

The Application Load Balancer provided a single entry point for application traffic and distributed requests across the available instances.

 Security and Availability Considerations

Using a load balancer and Auto Scaling improves application resilience by reducing dependence on a single EC2 instance.

If an instance becomes unhealthy, the load balancer can stop routing traffic to it while the Auto Scaling Group can maintain the required capacity.

This approach also supports availability during periods of increased demand by allowing additional instances to be launched when scaling conditions are met.

 Key Learning

This lab helped me understand how AWS services can work together to build a more available and scalable application environment.

I learned how to create an AMI, configure a Launch Template, create an Auto Scaling Group, configure a target group, and use an Application Load Balancer to distribute traffic across EC2 instances.

The exercise also reinforced the importance of designing cloud infrastructure for availability, scalability, monitoring, and resilience rather than relying on a single server.

 Ethical and Lab Notice

This exercise was completed within the AWS lab environment provided for educational purposes. The resources were created and configured only within the authorized lab account.
