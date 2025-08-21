# AWS-intro
# AWS Hands-On Practice

## Introduction
Amazon Web Services (AWS) is a leading cloud computing platform offering a wide range of services including compute, storage, networking, and security. AWS allows organizations and individuals to deploy and manage applications without maintaining physical infrastructure.

## Key Concepts

### Regions and Availability Zones
- **Region**: A geographical area with multiple, isolated data centers.
- **Availability Zone (AZ)**: Individual data centers within a region. Using multiple AZs ensures **high availability** and **fault tolerance**.

### EC2 (Elastic Compute Cloud)
- EC2 provides **scalable virtual servers** in the cloud.
- Users can launch, configure, and manage instances easily.
- Supports multiple operating systems and instance types.

## Hands-On Practice: EC2 Instance

### Steps Followed
1. Logged in to AWS Management Console.
2. Navigated to **EC2 Dashboard → Launch Instance**.
3. Selected **Amazon Linux 2 AMI**.
4. Chose **t2.micro** instance (Free Tier eligible).
5. Configured instance with default settings.
6. Added storage (default 8 GB).
7. Added tags for identification (e.g., Name: MyFirstEC2).
8. Configured **Security Group** to allow:
   - SSH (Port 22)
   - HTTP (Port 80)
9. Created a key pair (`.pem` file) and launched the instance.
10. Verified that the instance was running and accessible via public IP.

### Observations
- Instance successfully launched and accessible via SSH.
- Installed and verified web server functionality.
- Security groups controlled network access effectively.

## Conclusion
This practice helped in:
- Understanding **AWS cloud architecture**.
- Learning **regions, availability zones, and EC2 setup**.
- Gaining hands-on experience in **instance launch, security, and basic server configuration**.
