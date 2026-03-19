# Lab 4 – Working with Amazon Elastic Block Store (EBS)

## Author

* **Name**:THARSHINI M
* **Register Number**: 212224230287
* **Date of Submission**: 17.03.2026

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

1. Logged into the AWS Management Console and navigated to the EC2 dashboard to explore Amazon EBS volume types and features.
2. Created a new EBS volume by selecting size, type (gp2/gp3), and ensured it was in the same Availability Zone as the EC2 instance.
3. Attached the created EBS volume to the running EC2 instance as an additional device.
4. Connected to the EC2 instance using SSH and checked the attached volume using lsblk command.
5. Formatted the new volume using mkfs -t ext4 and created a mount directory (e.g., /mnt/ebs).
6. Mounted the volume to the directory and verified using df -h command.
7. Stored sample data by creating files inside the mounted directory.
8. Rebooted the EC2 instance and confirmed that the data persisted after restart.
---

## Output Screenshots (Attach 3)

### Screenshot 1: EBS Volume Created

<img width="1920" height="1080" alt="Screenshot 2026-02-27 090024" src="https://github.com/user-attachments/assets/00525c94-7284-4799-985a-ea3558cb0bdd" />


---

### Screenshot 2: EBS Volume Attached to EC2

<img width="1920" height="1080" alt="Screenshot 2026-02-27 090225" src="https://github.com/user-attachments/assets/03ce9ae4-a0e6-4cd2-972c-03b29c74b685" />


---

### Screenshot 3: Mounted Volume with Data

<img width="1920" height="1080" alt="Screenshot 2026-02-27 094051" src="https://github.com/user-attachments/assets/f9ee3933-4ae5-4fad-81a5-05dff55657d4" />


---

## Result / Conclusion

This experiment demonstrated how Amazon EBS provides persistent storage for EC2 instances. By creating, attaching, formatting, and mounting an EBS volume, and by verifying data after reboot, the concept of durable block storage in the cloud was clearly understood.
