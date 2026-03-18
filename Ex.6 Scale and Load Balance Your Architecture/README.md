# Lab 6 – Scale and Load Balance Your Architecture

## Title

Scale and Load Balance Your Architecture
 Author : JANSI RANI A A
 Reg no : 212224040130
 Date   : 18.03.2026

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

1.Launch multiple servers.

2.Deploy the application on each server.

3.Create a load balancer.

4.Add servers to the load balancer.

5.Configure auto-scaling.

---

## Output Screenshots 
![WhatsApp Image 2026-03-18 at 10 00 56 PM](https://github.com/user-attachments/assets/170a073f-e80f-4ef7-b93e-350921b135a3)

![WhatsApp Image 2026-03-18 at 10 01 13 PM](https://github.com/user-attachments/assets/4adb1711-c310-4e1f-a86a-9942be392823)


![WhatsApp Image 2026-03-18 at 10 01 26 PM](https://github.com/user-attachments/assets/f135ef37-17d2-430d-91bb-0a1c2ce7c84d)

![WhatsApp Image 2026-03-18 at 10 01 47 PM](https://github.com/user-attachments/assets/ea18ff0d-75dd-4566-82d2-5496f357c7e9)

![WhatsApp Image 2026-03-18 at 10 02 15 PM](https://github.com/user-attachments/assets/b01ff339-86b2-4943-b446-9390aee5f443)

![WhatsApp Image 2026-03-18 at 10 02 31 PM](https://github.com/user-attachments/assets/1c348655-be34-472b-b257-c7db5c31005a)


---


## Result

This experiment demonstrated how to build a scalable and fault-tolerant cloud architecture using Auto Scaling Groups and Elastic Load Balancing. The system automatically adjusted resources based on workload and ensured continuous service availability by distributing traffic across multiple instances.
