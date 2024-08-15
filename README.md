# Udagram Infrastructure

This project sets up a highly available, scalable, and secure web application infrastructure on AWS using a Virtual Private Cloud (VPC), Elastic Load Balancer (ELB), Auto Scaling, and NAT Gateways. The architecture is designed to serve an application across multiple availability zones for high availability and fault tolerance.

## Architecture Overview

The infrastructure comprises the following key components:

- **VPC**: A Virtual Private Cloud that spans multiple Availability Zones for high availability.
- **Subnets**: Public and private subnets distributed across multiple Availability Zones.
- **NAT Gateway**: Facilitates outbound internet access for instances in the private subnet.
- **Elastic Load Balancer**: Distributes incoming application traffic across multiple EC2 instances in different Availability Zones.
- **Auto Scaling Group**: Automatically adjusts the number of Amazon EC2 instances based on demand to maintain application availability and performance.
- **Security Groups**: Controls the inbound and outbound traffic to various components within the infrastructure.
- **IAM Role**: Provides permissions for EC2 instances to access AWS services securely.
- **S3 Bucket**: Used for storing static assets and backups.

![Alt text](https://github.com/mohamedfayez-7/Infrastructure-as-code-Udagram-Project/blob/41e8167c95647168dba66043b24720f9f0ac7803/Udagram%20Infrastructure%20.png)
udagr-WebAp-1QDNOJC70UQDR-81016286.us-east-1.elb.amazonaws.com

## Key Features

- **Scalability**: Automatically scales based on the application load.
- **High Availability**: Deploy instances across multiple Availability Zones to ensure application uptime.
- **Security**: Leverages Security Groups and IAM roles to enforce security best practices.

## Setup Instructions

1. **Clone the repository:**
   ```bash
   git clone https://github.com/your-username/your-repo-name.git
   cd your-repo-name
   
2. **Deploy the CloudFormation template:**
   Navigate to the AWS Management Console.
   You can go to the CloudFormation service.
   Upload the template file and deploy it.

2. **Access the Application:**
   After creating the stack, find the Load Balancer's DNS name in the CloudFormation outputs.
   Visit the DNS name in your browser to access the application

**Conclusion**
This infrastructure ensures that the web application is secure, scalable, and highly available. The use of AWS services like Auto Scaling, Load Balancer, and NAT Gateway ensures that the application can handle varying levels of traffic while maintaining performance and security.
