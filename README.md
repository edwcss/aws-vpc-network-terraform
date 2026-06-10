# AWS VPC Network Infrastructure (Terraform)

This project builds a clean, production‑style Virtual Private Cloud (VPC) on AWS using Terraform.  
It focuses entirely on networking — no EC2 instances — making it an ideal first cloud portfolio project.

##  Architecture Overview

This Terraform configuration deploys:

- A custom **VPC** (10.0.0.0/16)
- **Public subnet** (10.0.1.0/24)
- **Private subnet** (10.0.2.0/24)
- **Internet Gateway** for outbound internet access
- **NAT Gateway** for private subnet egress
- **Public route table** (IGW route)
- **Private route table** (NAT route)
- **Security groups** for public and private layers

This mirrors a real production network layout used by cloud engineers.

##  Architecture Diagram
VPC (10.0.0.0/16)
- ── Public Subnet (10.0.1.0/24)
-      ├── Internet Gateway
-      └── Public Route Table (0.0.0.0/0 → IGW)
- 
- └── Private Subnet (10.0.2.0/24)
- ├-── NAT Gateway
- └── Private Route Table (0.0.0.0/0 → NAT)


##  How to Deploy
terraform init
terraform apply


## How to Destroy
terraform destroy


This removes all resources created by the project.
##  Project Structure
aws-vpc-network-terraform/
- ── main.tf
- ── variables.tf
- ── outputs.tf
- ── providers.tf
- ── README.md


##  Why This Project Matters

This project demonstrates:

- Infrastructure as Code (IaC)
- AWS networking fundamentals
- Clean Terraform structure
- Production‑style VPC design
- Ability to build cloud infrastructure from scratch

Perfect for junior cloud engineer portfolios.

##  Author

Edmund Wan Chunsing — Cloud Engineer in training  


