# Lab 6 – Scale and Load Balance Your Architecture

## Title

Scale and Load Balance Your Architecture
Author : THARSHINI M
Reg no :212224230287
Date :17.03.2026

---

## Objective

The objective of this lab is to understand how to design a scalable and highly available architecture on AWS using Auto Scaling and Elastic Load Balancing. This experiment focuses on distributing incoming traffic across multiple EC2 instances, automatically scaling resources based on demand, and validating fault tolerance.

---

## Prerequisites

* Basic knowledge of Amazon EC2 and VPC
* Completion of previous labs (IAM, EC2, EBS, Database Server)
* AWS Academy Lab access
* Stable internet connection

---

## Tools Used

* AWS Management Console
* Amazon EC2
* Elastic Load Balancer (ELB / ALB)
* Auto Scaling Groups (ASG)
* Amazon CloudWatch

---

## Tasks Performed

### Task 1: Review Existing Architecture

Students review the existing EC2-based application architecture created in previous experiments.

### Task 2: Create a Launch Template

Students create a launch template that defines the EC2 instance configuration including AMI, instance type, security group, and user data.

### Task 3: Create an Auto Scaling Group

Students create an Auto Scaling Group using the launch template and configure minimum, maximum, and desired instance capacity.

### Task 4: Configure an Application Load Balancer

Students create an Application Load Balancer and configure target groups for routing traffic to EC2 instances.

### Task 5: Register Auto Scaling Group with Load Balancer

Students attach the Auto Scaling Group to the target group of the load balancer.

### Task 6: Configure Scaling Policies

Students configure scaling policies based on CPU utilization using Amazon CloudWatch alarms.

### Task 7: Test Load Balancing and Scaling

Students test the setup by generating traffic and observing automatic scaling and load distribution.

---

## Workflow (To be filled by Student)

1. Logged into the AWS Management Console and reviewed the existing EC2 architecture created in previous labs.
2. Created a Launch Template by selecting an AMI, instance type, key pair, security group, and added user data for application setup.
3. Configured an Auto Scaling Group (ASG) using the launch template and set minimum, desired, and maximum number of instances.
4. Created an Application Load Balancer (ALB) and configured listeners and a target group.
5. Attached the Auto Scaling Group to the target group so that traffic is distributed across instances.
6. Set up scaling policies using CloudWatch alarms based on CPU utilization (scale out and scale in conditions).
7. Generated traffic to test the system and observed automatic scaling and load balancing across EC2 instances.
8. Verified fault tolerance by stopping an instance and confirming that the ASG launched a new instance automatically.

## Output Screenshots 
<img width="1920" height="1080" alt="Screenshot 2026-03-12 110211" src="https://github.com/user-attachments/assets/c9d3bc1c-245d-4678-8db9-159da4915053" />

<img width="1920" height="1080" alt="Screenshot 2026-03-12 110602" src="https://github.com/user-attachments/assets/5ae2e351-c6fd-463f-956b-5ee145e464d2" />

<img width="1920" height="1080" alt="Screenshot 2026-03-12 111737" src="https://github.com/user-attachments/assets/2b99bd4c-c30f-45f2-b477-5b3db3b8cae0" />

<img width="1920" height="1080" alt="Screenshot 2026-03-12 112640" src="https://github.com/user-attachments/assets/b4116d53-071a-465f-8adf-76f84f2f13a1" />

<img width="1920" height="1080" alt="Screenshot 2026-03-12 113838" src="https://github.com/user-attachments/assets/e235b33f-655d-4eb6-a09f-6d743645366d" />

<img width="1920" height="1080" alt="Screenshot 2026-03-12 115021" src="https://github.com/user-attachments/assets/38869efc-c16a-4c38-9676-e0b2cd7123f7" />






---


## Result

This experiment demonstrated how to build a scalable and fault-tolerant cloud architecture using Auto Scaling Groups and Elastic Load Balancing. The system automatically adjusted resources based on workload and ensured continuous service availability by distributing traffic across multiple instances.
