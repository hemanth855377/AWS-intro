# Launching an EC2 Instance  

## Steps to Launch  

1. **Log in to AWS Console**  
   - Open the **EC2 Dashboard** from AWS Management Console.  

2. **Choose AMI (Amazon Machine Image)**  
   - Selected: **Amazon Linux 2 AMI (64-bit, x86)**  

3. **Select Instance Type**  
   - Chosen type: **t2.micro** (Free Tier Eligible)  
   - vCPU: 1 | Memory: 1 GiB  

4. **Configure Instance**  
   - Network: Default VPC  
   - Subnet: Automatically assigned  
   - Public IP: Enabled  

5. **Add Storage**  
   - Root Volume: **8 GiB General Purpose SSD (gp2)**  

6. **Add Tags**  
   - Example: `Name = MyFirstEC2`  

7. **Configure Security Group**  
   - Inbound: Allow **SSH (22)** from my IP  
   - Outbound: Allow all traffic (default)  

8. **Key Pair**  
   - Created/used existing key: `my-key.pem`  

9. **Launch Instance**  
   - Instance launched successfully.  
   - Status: **Running**  

---

## Result  

- **Instance ID:** `i-xxxxxxxxxxxx`  
- **Public IP:** `xx.xx.xx.xx`  
- Connected via SSH:  

```bash
ssh -i my-key.pem ec2-user@<public-ip>














https://github.com/hemanth855377/AWS-intro/blob/main/EC2/WhatsApp%20Image%202025-08-23%20at%2011.16.51%20AM.jpeg?raw=true
