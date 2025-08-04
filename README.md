# aws-cloud-interview-questions

# How do you ensure high availability and scaling in the cloud?
  - Multi availability zone 


# What is RDS instance
- RDS is a RElational Database Service which provides a compute power to store the relational database or process the database for the real time applications
-  

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
- After uploading the index.html we need to enable statis website hosting which present in the properties of aws


# S3 storage classes
- Amazon S3 Standard - general purpose
- Amazon S3 standard  - infrequent access
- Amazon S3 One Zone-Infrequent Access (IA)
- Amazon S3 intelligent Tiering
- Amazon Glacier
- Amazon Glacier Deep Archive

# S3 Durability and Availability
- Durability : Durability means how often we lose a file
- 99.999999999% High availabilty objects across multiple avalilabilty zone

Availability on s3 standard 
- 99.99 % availability which means in a year for 53 minutes the the data will not available 

![image](https://github.com/user-attachments/assets/8d5aa31e-c229-4bec-b184-d599220b9def)




# AWS Database

Amazon RDS
- Automated Provisioning, OS patching
- Continuos backup and restore to speicific timestamp(Point to Restore)
- Monitoring dashboard
- Read replicas for improved read performance
- Multi AZ setup for DR(Disaster recovery)
- Scaling capability
- **But cannot SSH into your instance**

# Amazon Aurora
- Amazon Aurora is not open source



# coroebus

coroebus

[![Built with Cookiecutter Django](https://img.shields.io/badge/built%20with-Cookiecutter%20Django-ff69b4.svg?logo=cookiecutter)](https://github.com/cookiecutter/cookiecutter-django/)
[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)

## Settings

Moved to [settings](https://cookiecutter-django.readthedocs.io/en/latest/1-getting-started/settings.html).

## Basic Commands

### Setting Up Your Users

- To create a **normal user account**, just go to Sign Up and fill out the form. Once you submit it, you'll see a "Verify Your E-mail Address" page. Go to your console to see a simulated email verification message. Copy the link into your browser. Now the user's email should be verified and ready to go.

- To create a **superuser account**, use this command:

      $ python manage.py createsuperuser

For convenience, you can keep your normal user logged in on Chrome and your superuser logged in on Firefox (or similar), so that you can see how the site behaves for both kinds of users.

### Type checks

Running type checks with mypy:

    $ mypy coroebus

### Test coverage

To run the tests, check your test coverage, and generate an HTML coverage report:

    $ coverage run -m pytest
    $ coverage html
    $ open htmlcov/index.html

#### Running tests with pytest

    $ pytest

### Live reloading and Sass CSS compilation

Moved to [Live reloading and SASS compilation](https://cookiecutter-django.readthedocs.io/en/latest/2-local-development/developing-locally.html#using-webpack-or-gulp).

## Deployment

