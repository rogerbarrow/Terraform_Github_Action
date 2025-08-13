# Terraform_Github_Action
# Creating VPC Using Terraform and Deploying Via GitHub Actions
<img width="800" height="422" alt="image" src="https://github.com/user-attachments/assets/88b510fe-15a6-4189-a74b-576fce1e3669" />

# Overview
In today's cloud-driven world, the ability to design and deploy infrastructure quickly and securely is a must-have skill. Mastering Terraform for infrastructure as code and GitHub Actions for automation gives you the power to streamline deployments, ensure consistency, and scale with ease. These skills are vital in DevOps and Cloud Engineering, where speed, reliability, and collaboration are key. In this guide, we'll create a Virtual Private Cloud (VPC) with Terraform and automate its deployment using GitHub Actions.

This guide will help creating a Virtual Private Cloud (VPC) infrastructure using Terraform and then automating the deployment of your Terraform code using GitHub Actions.

<img width="800" height="406" alt="image" src="https://github.com/user-attachments/assets/d0a79552-1bd6-4a90-a725-39be33a980cf" />

# What is an VPC?

A VPC (Virtual Private Cloud) is your own private section of the cloud where you control networking, security, and connectivity. You choose IP ranges, create subnets, set traffic rules, and decide which resources can communicate

# What is a Subnet?

A subnet (short for "subnetwork") is like dividing your VPC into smaller, organized neighborhoods.
Each subnet is a section of your VPC's IP address range where you can place specific resources - like servers, databases, or load balancers. You can make them public (connected to the internet) or private (only accessible inside your network).


# Internet Gateway-
An Internet Gateway (IGW) lets your VPC connect to the public internet. After attaching it to your VPC, update your route tables with a default route (0.0.0.0/0) to enable traffic in and out-without both steps, your VPC remains isolated.

# Router-
A VPC router directs traffic using route tables to decide where it goes - whether to the internet, between subnets, or to other networks. You control its behavior by updating route tables; without proper routes, traffic can't move.
Load Balancer-
A load balancer is a tool that distributes incoming traffic across multiple servers or resources so no single one gets overwhelmed.
In the cloud, it improves availability, scalability, and performance by making sure requests are sent to healthy resources. If one server fails, the load balancer automatically routes traffic to the others.
