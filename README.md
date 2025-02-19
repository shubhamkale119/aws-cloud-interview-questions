# aws-cloud-interview-questions

# How do you ensure high availability and scaling in the cloud?
  - Multi availability zone 


# What is RDS instance
- RDS Instance provide a compute power to setup, run and maintain the database on aws public cloud

# RDS instances types:
- General Purpose: used when there is modrate traffic on compute engine
- Memory optimize: This instance is designed for when you require high memory usage
- Storage optimize: It is used when we require the high storage capacity

# What is Ec2 user data
- The commands Start when ec2 instnce get launch
- This is basically script which run when ec2 instance get launch
- Bootstraping means launching commands when ec2 instance get launch

# EBS (Elastic Block Storage)

- EBS is the storage use for the ec2 instance it is like hard disk storage
- EBS can attach to only region wise cannot attach in other region to the ec2 instance
- We can attach EBS to different region by taking EBS snapshot and attach that restore that EBS snapshot and attach that snapshot to the other zone

# EFS Elatic File System
- This is the network file system can be attached to multiple ec2 instance

# Amazon fsx for windows File Server

# Load Balancing 
- Load balancer distribute load to multiple ec2 instances

# Elastic Load Balancer
- It is a managed load balancer
- It distribute traffic to multiple instances

# Auto Scaling Group
- Create first launch template for AMI which has took backup from ec2 instance
- Create ASG and then add that launch template and define desired maximum and minimum instance number

# S3 (Simple Storage Service)
 S3 Security
- User based
  - IAM Policy
- Resource Based
  - Bucket policy
  - Object Access Control List (ACL)
  - Bucket Access Control List (ACL)
 
- For accessing the data present in the bucket you need to disable public access and and add bucket policy to the bucket
- We can host a static website on s3 bucket 
