# Lab 4 – Working with Amazon Elastic Block Store (EBS)

## Author

* **Name**: JANSI RANI A A
* **Register Number**: 212224040130
* **Date of Submission**: 10.03.2026
---

## Objective

The objective of this experiment is to understand how Amazon Elastic Block Store (EBS) provides persistent block-level storage for EC2 instances. This lab focuses on creating and attaching an EBS volume, formatting and mounting it on an EC2 instance, storing data, and verifying data persistence after instance reboot.

---

## Prerequisites

* Basic understanding of cloud computing concepts
* AWS account or AWS Academy Lab access
* An existing EC2 instance (Amazon Linux 2 preferred)
* Basic knowledge of Linux commands

---

## Tools Used

* AWS Management Console
* Amazon EC2
* Amazon EBS
* SSH Client (Terminal / PuTTY)

---

## Tasks Performed

### Task 1: Explore Amazon EBS

Explore the Amazon EBS service through the EC2 dashboard. Observe different volume types such as General Purpose SSD (gp2/gp3), Provisioned IOPS SSD, Throughput Optimized HDD, and Cold HDD.

---

### Task 2: Create an EBS Volume

Create a new EBS volume in the same Availability Zone as the EC2 instance. Choose an appropriate size and volume type.

---

### Task 3: Attach EBS Volume to EC2 Instance

Attach the created EBS volume to the running EC2 instance as an additional block device.

---

### Task 4: Format the EBS Volume

Connect to the EC2 instance using SSH and format the attached volume with a file system (for example, ext4).

---

### Task 5: Mount the EBS Volume

Mount the formatted volume to a directory in the EC2 instance (for example, /data or /mnt/ebs).

---

### Task 6: Store Data in EBS Volume

Create files and directories inside the mounted EBS volume and store sample data.

---

### Task 7: Verify Data Persistence

Reboot the EC2 instance and verify that the data stored in the EBS volume is still available after reboot.

---

## Workflow (Student Explanation)

1.Create Volume: I created a new EBS Volume in the same Availability Zone (e.g., us-east-1a) as my EC2 instance.

2.Attach Volume: I used the Actions menu in the EC2 console to Attach the volume to my running instance.

3.Format and Mount: I logged into the instance and used the mkfs command to format the disk and the mount command to make it ready for use.

4.Create Snapshot: I created a Snapshot of the volume, which acts as a point-in-time backup of my data in Amazon S3.

5.Restore Data: Finally, I created a new volume from the snapshot to verify that my data could be successfully recovered.

---

## Output Screenshots (Attach 3)

### Screenshot 1: EBS Volume Created

<img width="1366" height="768" alt="Screenshot (850)" src="https://github.com/user-attachments/assets/a8bf5ded-c588-426d-a9d6-b916307bdf90" />



### Screenshot 2: EBS Volume Attached to EC2

<img width="1366" height="768" alt="Screenshot (856)" src="https://github.com/user-attachments/assets/c96d4053-a5bc-4cdd-8d68-78ad0ea056c0" />


### Screenshot 3: Mounted Volume with Data

<img width="1366" height="768" alt="Screenshot (864)" src="https://github.com/user-attachments/assets/19aea6bf-8626-4092-8947-4fbc605e48ca" />

## Result / Conclusion

This experiment demonstrated how Amazon EBS provides persistent storage for EC2 instances. By creating, attaching, formatting, and mounting an EBS volume, and by verifying data after reboot, the concept of durable block storage in the cloud was clearly understood.
