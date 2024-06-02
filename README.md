# PersonalWebsite

## What Did I Learn:
What problem did I solve by completing this project? 

- Learning how to create my own personal website, including all the html, css, and js assets, while fully hosting it on a well designed, highly avaliable, and scalable cloud architecture.
  
What issues arose and what did I do to overcome those issues?
- One issue that came up was exceeding the free tier limit of AWS while using these resources and having 2 ec2 instances up at all times. To overcome this issue, I took advantage of AWS alarms and formatted it so that the min number of instances, one instance, would stay up while idle and unaccessed. 


## Hosting a WordPress Website on AWS

This repository contains the resources and scripts used to deploy a WordPress website on Amazon Web Services (AWS). The project leverages various AWS services to ensure high availability, scalability, and security for the WordPress application.

## Architecture Overview

The WordPress website is hosted on EC2 instances within a highly available and secure architecture that includes:

- A Virtual Private Cloud (VPC) with public and private subnets across two Availability Zones (AZs) for fault tolerance and high availability.
- An Internet Gateway to allow communication between instances in the VPC and the internet.
- Security Groups acting as a virtual firewall to control inbound and outbound traffic.
- Public Subnets used for the NAT Gateway and Application Load Balancer, facilitating external access and load balancing.
- Private Subnets for web servers to enhance security.
- EC2 Instance Connect Endpoint for secure SSH access.
- An Application Load Balancer with a target group to distribute incoming web traffic across multiple EC2 instances.
- An Auto Scaling Group to automatically adjust the number of EC2 instances based on traffic, ensuring scalability and resilience.
- Amazon RDS for a managed relational database service.
- Amazon EFS for a scalable, elastic file storage system.
- AWS Certificate Manager for managing SSL/TLS certificates.
- AWS Simple Notification Service (SNS) for notifications related to the Auto Scaling Group activities.
- Amazon Route 53 for domain name registration and DNS management.
  
## Architecture Layout
![2 _Host_a_WordPress_Website_on_AWS](https://github.com/RohanSkaria/PersonalWebsite/assets/100239078/c345702c-da4c-4f31-9859-db8989d3c1b2)
