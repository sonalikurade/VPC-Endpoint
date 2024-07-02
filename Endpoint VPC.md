# VPC Endpoint

- VPC endpoint enables creation of a private connection between VPC to supported AWS services
- Traffic between VPC and AWS service does not leave the Amazon network.
## There are two types of VPC endpoints:

1. Interface endpoint 
2. Gateway endpoint
## Step1: Login into your AWS Console

## Step2: Create Infrastructure

- Create VPC
- Create 2 Subnet in that one is public and other is Private.
- Make One Public by Enabling in Setting
- Create one IGW for Public Subnet
- Attach that subnet to VPC
- Create public Route Table  to Public Subnet and add Route of Internet Gateway
- Create private Route Table for private subnet. Don't add any route in it. Because when we create Endpoint at that we are giving this private RT.
- In Private RT Route get added automatically after creating Endpoint
- Create S3 bucket
- Create Role for S3 bucket
- Create Endpoint to access the resources like s3 bucket.

## Step 3:

- In the AWS Management Console search bar, enter VPC, and click the VPC result under Services:
- To start creating VPC, in the left down side, Click on **Your VPC** to Create VPC:
- Create one IGW for Public Subnet
- Attach Internet Gateway to VPC
- Create Public Subnet
- Create private subnet
- Make your subnet public by enabling the setting
- Create one Route for public subnet
- Do subnet Association with public subnet.
- Add Route of internet gateway to the Route Table
- Create private RT for private subnet.
- Do subnet Association with public subnet.
- Launch the public Instance
- Launch private instance and select private subnet
- Create s3 Bucket
- Do scp and copy your key in virtual machine
- Do ssh to private ec2 instance
- View the list of bucket using below command .you will not get any output here . because of that you need to create VPC endpoint.
- Create VPC Endpoint
Create  Role for output
