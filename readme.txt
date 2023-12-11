3-Tier Web Application Architecture on AWS

Overview
This repository contains an AWS CloudFormation template for deploying a 3-tier web application architecture. The architecture is designed to be scalable, highly available, and secure, suitable for running production-grade web applications on AWS.

Architecture
The CloudFormation template deploys the following resources:

VPC: A Virtual Private Cloud for isolated network infrastructure.

Subnets:
Web Tier Subnets: 2 public subnets for hosting web servers or front-end services.
Application Tier Subnets: 2 private subnets for application logic layers such as backend servers.
Database Tier Subnets: 2 private subnets for database servers.

Internet Gateway: To provide internet access to instances in public subnets.

Route Tables and Associations: For managing network traffic flow.

Security Groups: To secure access to instances in each tier.

Elastic Load Balancer (ELB): For distributing incoming web traffic across multiple web servers.

Auto Scaling Groups: For the web and application tiers to automatically scale the resources.

RDS Database Instance: An Amazon RDS instance for database needs, placed in private subnets.

Deployment
Prerequisites
An AWS account.
AWS CLI installed and configured.
Basic understanding of AWS CloudFormation.