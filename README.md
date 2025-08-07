# Terraform IaC Demo

A simple Infrastructure as Code project using Terraform to create local files simulating container deployment.

## What I Built

I created a Terraform configuration that provisions:
- Application configuration file
- Dockerfile for containerization
- Startup script for deployment

## Prerequisites

- Terraform installed
- Basic terminal knowledge

## How I Did It

### 1. Initialize Terraform
```bash
terraform init
```
![Architecture Diagram](images/init.png)

### 2. Plan the Infrastructure
```bash
terraform plan
```
![Architecture Diagram](images/plan.png)

### 3. Apply the Configuration
```bash
terraform apply
```
Type `yes` when prompted.

![Architecture Diagram](images/apply.png)


### 4. View Terraform State
```bash
terraform state list
terraform state show local_file.config
```
![Architecture Diagram](images/state.png)


### 5. Verify Infrastructure (if using Docker)
```bash
docker ps
```
![Architecture Diagram](images/docker.png)

### 6. Clean Up Infrastructure
```bash
terraform destroy
```
Type `yes` when prompted.

![Architecture Diagram](images/destroy.png)



## Outputs

## Demo App Running on Localhost
![Architecture Diagram](images/localhost.png)

The Terraform configuration provides:
- Paths to all created files
- Application info with port and timestamp



## What I Learned

- How to write Terraform configurations
- Managing infrastructure state
- Using local providers for development

