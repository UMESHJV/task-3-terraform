# Task 3: Infrastructure as Code (IaC) with Terraform

## Objective
Provision and manage a local Docker container using Terraform.

## Tools Used
- Terraform 1.14.8
- Docker Desktop 29.4.0
- Docker provider for Terraform
- Nginx Alpine image

## Project Overview
This project demonstrates Infrastructure as Code (IaC) by using Terraform to manage a Docker image and container.

Terraform downloads the Nginx Alpine image if required and creates a Docker container named `task3-nginx`. Port 8080 on the host is mapped to port 80 inside the container.

## Implementation Steps
1. Created the `main.tf` configuration.
2. Initialized Terraform using `terraform init`.
3. Validated the configuration using `terraform validate`.
4. Reviewed the proposed changes using `terraform plan`.
5. Created the resources using `terraform apply`.
6. Verified the running container using `docker ps`.
7. Accessed the Nginx welcome page at `http://localhost:8080`.
8. Inspected Terraform resources using state commands.
9. Removed the infrastructure using `terraform destroy`.

## Resources Managed
- `docker_image.nginx`
- `docker_container.nginx`

## Verification
The Nginx welcome page was displayed successfully in the browser. The container was subsequently removed using Terraform.

## Cleanup
Executed `terraform destroy` successfully. Two Terraform-managed resources were destroyed.

## Learning Outcomes
- Understanding Infrastructure as Code.
- Using Terraform providers and resources.
- Initializing, validating, planning, and applying Terraform configurations.
- Inspecting Terraform state.
- Destroying infrastructure safely.
