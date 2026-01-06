# What is EC2?

Amazon EC2 (Elastic Compute Cloud) is a virtual server service in AWS that provides scalable compute power using virtualization technology.
It allows users to create virtual machines with different CPU, RAM and storage configurations to run applications, websites and databases.
EC2 follows a pay-as-you-go model and supports auto scaling and load balancing.


🚀 My First AWS EC2 Server Launch
📌 Objective
To launch and access my first cloud server using AWS EC2 and understand how remote servers work using SSH.

🛠️ Steps I Followed to Launch My First EC2
Step 1 – Login to AWS Console
Logged in to AWS Management Console and navigated to:
Services → EC2 → Instances → Launch Instance
<img width="2559" height="763" alt="image" src="https://github.com/user-attachments/assets/48d186ef-5b51-4fbd-95ad-a0a3de701d42" />

Step 2 – Configure Instance
Setting	Value
Name	MyFirstEC2
AMI	Amazon Linux 2023
Instance Type	t3.micro
Key Pair	Created a new key pair
Network	Default VPC
Auto-assign Public IP	Enabled
<img width="1354" height="939" alt="image" src="https://github.com/user-attachments/assets/30ef3748-7090-49b9-b7d5-3b9053424832" />
<img width="957" height="705" alt="image" src="https://github.com/user-attachments/assets/8cda5504-c9f3-4cb3-a2e2-6e8741a646c3" />
🔐 Checking Security Group & Network Access Rules

After launching the EC2 instance, I verified its network security rules to ensure secure remote access.
EC2 Dashboard → Instances → Select Instance → Security Tab
<img width="2555" height="1253" alt="image" src="https://github.com/user-attachments/assets/f66d8700-51a0-411c-83e4-d9e32a164838" />

🔗 Connecting to the EC2 Server Using SSH

After the instance was in Running state, I connected to the server using EC2 Instance Connect (browser-based SSH).
<img width="2473" height="888" alt="image" src="https://github.com/user-attachments/assets/e5d706f6-97e0-4f1c-93a7-bfcfe751011e" />


🌐 EC2 Public IP vs Private IP Behavior

By default, an Amazon EC2 instance is assigned both a public IP and a private IP address.

Public IP Address

The public IP is temporary.

When an EC2 instance is stopped and started again, AWS automatically releases the existing public IP and assigns a new public IP.

This happens because public IPs are managed from a shared AWS pool and are not permanent by default.

Private IP Address

The private IP is permanent within the VPC.

It remains the same even after stop/start or reboot operations.

This ensures stable internal communication between services inside the AWS network.

