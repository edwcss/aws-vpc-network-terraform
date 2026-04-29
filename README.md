# AWS VPC Infrastructure (Terraform)
This project demonstrates the deployment of a custom Virtual Private Cloud (VPC) in the Tokyo region.

## Architecture
* **VPC:** 10.0.0.0/16 (Private isolated network)
* **Subnet:** Public Subnet with Auto-IP enabled
* **Gateway:** Internet Gateway (IGW) for external connectivity

## Usage
1. `terraform init`
2. `terraform plan`
3. `terraform apply`

## Learning Notes
This lab focused on establishing the networking foundation for cloud-native applications. By defining a custom VPC instead of using the default, I gained hands-on experience with CIDR block allocation and network isolation.
