1. Explore & Understand AWS
Algorithm:

Sign up for AWS

Visit AWS Console and create an account.
Set up IAM roles and users with appropriate permissions.
Navigate AWS Services

Log in to the AWS Management Console.
Explore EC2, S3, IAM, RDS, VPC, and other key services.
Understand AWS Free Tier Limits

AWS offers a free tier with limited services.
Ensure services used do not exceed free limits.
Use AWS CLI

Install AWS CLI using pip install awscli or download from AWS.
Configure AWS CLI using aws configure.
Practice with AWS Documentation
![image](https://github.com/user-attachments/assets/287c6583-9671-4533-bceb-33c73b3be672)

Visit the AWS Documentation for hands-on learning.
2. Create & Manage Amazon EC2 Instances
Algorithm:

Log in to AWS Console

Navigate to EC2 Dashboard.
Launch an EC2 Instance

Click Launch Instance.
Choose an Amazon Machine Image (AMI) (e.g., Ubuntu, Amazon Linux).
Select an Instance Type (e.g., t2.micro for Free Tier).
Configure Instance Details

Set up Networking (VPC, Subnet).
Enable Auto-assign Public IP if needed.
Add Storage

Set root volume size (e.g., 8GB default).
Configure Security Group

Allow SSH (port 22), HTTP (port 80), or other required ports.
Create & Download Key Pair

Select Create a new key pair and download .pem file.
Launch the Instance

Click Launch and wait for initialization.
Connect to the Instance

Open Terminal/Command Prompt.
Run ssh -i your-key.pem ec2-user@your-instance-ip.
Result:
![image](https://github.com/user-attachments/assets/ce1adef0-8bbc-4393-bd50-3cb69b6e52e6)

Successfully launched and connected to an EC2 instance.
3. Install OpenStack
(OpenStack is an open-source cloud platform for managing virtualized resources.)

Algorithm:

Prepare Ubuntu Server (20.04/22.04)

Use a clean Ubuntu Linux environment (preferably a VM or EC2).
Update & Install Dependencies

bash
Copy
Edit
sudo apt update && sudo apt upgrade -y
sudo apt install -y software-properties-common
sudo add-apt-repository cloud-archive:wallaby -y
sudo apt update
Install OpenStack Services

bash
Copy
Edit
sudo apt install -y openstack-client
sudo apt install -y keystone glance nova-api nova-conductor nova-novncproxy nova-scheduler
Configure Keystone (Identity Service)

Initialize Keystone, set up an admin user, and configure API endpoints.
Install Glance (Image Service)

Enable support for OpenStack virtual machine images.
Configure Nova (Compute Service)

Manage virtual instances inside OpenStack.
Verify Installation

bash
Copy
Edit
openstack --version
openstack service list
Launch OpenStack Dashboard

Access Horizon Dashboard using http://<your-server-ip>/dashboard.
Log in with admin credentials.
Result:
![image](https://github.com/user-attachments/assets/bb800dc6-856d-45e8-b41f-00ddce216cd2)
![image](https://github.com/user-attachments/assets/10c40b19-5a9c-4153-b80a-14f1ab942cbe)

Successfully installed OpenStack and accessed the Horizon Dashboard.
