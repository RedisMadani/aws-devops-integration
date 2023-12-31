# AWS DevOps Integration

## Introduction

This project encapsulates the integration of DevOps practices on AWS, featuring the deployment of a high-availability Jenkins setup, service discovery with Consul and Nginx, scalable Java application management using Terraform, and comprehensive monitoring through a Prometheus Observability Stack.

---

## Project 1: Deploying Jenkins on AWS for High Availability

### Overview
This project involves setting up a highly available Jenkins environment on AWS using an Auto Scaling Group. 

### Architecture
![image](https://github.com/RedisMadani/aws-devops-integration/assets/136177376/e3072bfb-3c5d-4daf-9970-675c2c2fa67b)

### Setup Process
- **AWS Account:** A valid AWS account is required.
- **Tools:** AWS CLI, Ansible, and Terraform installed on a workstation or AWS instance.
- **Provisioning with Terraform:** Customize `terraform.tfvars` with your AWS credentials and desired configurations. Initialize Terraform and apply configurations to provision the instances.
- **Configuration with Ansible:** Set up inventory files with instance IP addresses and execute Ansible playbooks for configuration.

---

## Project 2: Implementing Service Discovery with Consul and Nginx

### Overview
This project focuses on setting up Nginx load balancing using Consul for service discovery.

### Architecture
![image](https://github.com/RedisMadani/aws-devops-integration/assets/136177376/a705c38e-b138-4d6b-8053-0395e8848d8a)

### Manual Setup
- **Practical Guide:** Follow the guide for a hands-on approach to learn about the components and workflows involved.
- **Configuration:** Use provided scripts and Ansible playbooks to configure Consul servers and Nginx load balancers.

---

## Project 3: Scalable Java Application Deployment on AWS Using Terraform

### Overview
Deploy an open-source Java application (e.g., Spring PetClinic) on AWS, leveraging Autoscaling Groups, RDS, and other AWS services.

### Architecture
![image](https://github.com/RedisMadani/aws-devops-integration/assets/136177376/98110a8a-b3f0-4684-86c6-a8f21d711254)

### Workflow
- **Build and Package:** Build the Java application and use Packer & Ansible for AMI creation.
- **AWS Setup:** Utilize Terraform for provisioning RDS instances, Application Load Balancers, and setting up Autoscaling Groups.
- **Observation and Management:** Verify application functionality and monitor logs via Cloudwatch.

---

## Project 4: Setting Up Prometheus Observability Stack Using Docker

### Overview
Configure and deploy a Prometheus Observability Stack, providing insights into the health and performance of your applications and infrastructure.

### Architecture
![image](https://github.com/RedisMadani/aws-devops-integration/assets/136177376/f6dbab34-f649-4bed-b48f-48bb446b38fb)

### Setup Process
- **Docker Configuration:** Deploy Prometheus, Grafana, and other observability tools using Docker.
- **Monitoring and Alerts:** Configure metrics collection, dashboards, and alerting rules.
