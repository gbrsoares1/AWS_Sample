# AWS Sample - Full Stack Application on ECS with Terraform

## Overview

This project demonstrates the provisioning and deployment of a containerized full-stack application on AWS using Infrastructure as Code (Terraform) and CI/CD automation with GitHub Actions.

The environment includes a frontend application, a backend API, container image repositories, load balancers, networking resources and automated deployment pipelines.

## Architecture

The infrastructure is provisioned entirely through Terraform and includes:

* Amazon ECS Fargate
* Amazon ECR
* Application Load Balancer (ALB)
* VPC
* Public and Private Subnets
* Security Groups
* IAM Roles and Policies
* GitHub Actions CI/CD Pipeline

### Deployment Flow

1. Developer pushes code to GitHub
2. GitHub Actions pipeline is triggered
3. Docker images are built
4. Images are pushed to Amazon ECR
5. ECS services pull updated images
6. Application is exposed through Application Load Balancers

## Technologies Used

### Cloud

* AWS ECS Fargate
* AWS ECR
* AWS ALB
* AWS IAM
* AWS VPC

### Infrastructure as Code

* Terraform

### CI/CD

* GitHub Actions

### Containers

* Docker

### Application

* Node.js
* Nginx

## Repository Structure

```text
.
├── Code
│   ├── client
│   └── server
│
├── Infrastructure
│   ├── Modules
│   ├── Templates
│   └── Terraform configuration
│
└── .github
    └── workflows
```

## Skills Demonstrated

* Infrastructure as Code (Terraform)
* AWS Cloud Architecture
* Containerization with Docker
* ECS Fargate Deployments
* Load Balancing with ALB
* Networking Design (VPC, Subnets, Routing)
* IAM Permissions Management
* Continuous Integration
* Continuous Delivery
* GitHub Actions Automation
* Troubleshooting Cloud Deployments

## Results

Successfully provisioned and deployed a full-stack application in AWS using a fully automated workflow.

The project includes:

* Automated infrastructure provisioning
* Automated Docker image build process
* Automated image publication to ECR
* ECS service deployment
* Application exposure through Load Balancers
* End-to-end CI/CD pipeline

## Future Improvements

* HTTPS with ACM and Route 53
* Monitoring with CloudWatch
* Prometheus and Grafana integration
* Blue/Green Deployments
* ECS Auto Scaling
* Kubernetes migration (EKS)
* ArgoCD GitOps workflow

## Author

Gabriel Soares

Mechanical and Systems Engineering Student with focus on Cloud Computing, Infrastructure, DevOps and Site Reliability Engineering (SRE).

