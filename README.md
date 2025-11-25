AWS Project Report 

Title: Auto-Scaling and Load Balancing using AWS

Project Overview

This project demonstrates how to build a scalable and highly available application using Amazon Web Services (AWS). Although the project is not live, it showcases the design, architecture, implementation steps, and performance testing conducted on a simulated environment.

Objective

To understand and implement Auto Scaling for handling varying traffic.

To use an Elastic Load Balancer (ELB) for distributing incoming requests.

To analyze server performance under different loads using AWS tools.

To gain hands-on experience in deploying an application on cloud infrastructure.

Architecture Used

The architecture includes the following AWS services:

EC2 Instances – For hosting the application.

Application Load Balancer (ALB) – To distribute traffic across instances.

Auto Scaling Group (ASG) – To automatically increase or decrease the number of EC2 instances based on load.

CloudWatch – To monitor performance and trigger Auto Scaling policies.

IAM – For secure access management.

VPC – To run all resources in a secure network.

Key Features

Automatic Scaling: EC2 instances scale up when CPU usage increases and scale down during low traffic.

High Availability: Load balancer ensures no single point of failure.

Performance Testing: Stress testing is done using tools like Apache Benchmark (ab) / JMeter to observe scaling in action.

Cost Optimization: Auto Scaling helps reduce unnecessary cost by deallocating idle resources.

Implementation Steps
1. Launch EC2 Instances

Created AMI-based instances.

Installed the required application and server environment.

2. Configure Load Balancer

Created an Application Load Balancer.

Added EC2 instances to the Target Group.

3. Create Auto Scaling Group

Set desired, minimum, and maximum number of instances.

Configured scaling policies based on CPU Utilization.

4. Monitoring and Alerts

Used CloudWatch Alarms to monitor CPU, RAM, and traffic.

Set triggers for scale-in and scale-out.

5. Performance Testing

Applied load on the server.

Observed instance creation and termination based on load.

Monitored load distribution via ALB.

Results

The system automatically scaled from 1 instance to multiple instances under heavy load.

When traffic reduced, instances were automatically removed, reducing cost.

Load Balancer successfully distributed traffic without downtime.

Dashboard graphs (CPU vs Time, Instance count vs Load) showed correct scaling operations.

Conclusion

This project demonstrates an effective use of AWS Auto Scaling and Load Balancer to create a scalable, fault-tolerant, and cost-efficient application infrastructure.
Even though the project is not deployed live, the implementation and testing validate the architecture and functionality.

Future Enhancements

Deploy the application using CI/CD pipelines (CodePipeline, CodeDeploy).

Add RDS / DynamoDB for database integration.

Use Route 53 for DNS management.

Integrate CloudFront for content delivery.
