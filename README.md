# AWS Infrastructure Provisioning with Terraform (VPC & Subnet)

This repository contains Infrastructure as Code (IaC) written in Terraform to provision a secure and scalable networking environment on Amazon Web Services (AWS).

## 🚀 Project Overview
The goal of this project is to automate the creation of a custom Virtual Private Cloud (VPC) along with a Public Subnet using Terraform, following Infrastructure as Code best practices.

## 🛠️ Architecture Components
1. **AWS Provider:** Configured to deploy resources in the `us-east-1` region.
2. **Custom VPC (`Ibrahim-Cloud-VPC`):** 
   - CIDR Block: `10.0.0.0/16`
   - Enabled DNS Hostnames and Support for seamless instance naming and resolution.
3. **Public Subnet (`Ibrahim-Public-Subnet`):** 
   - CIDR Block: `10.0.1.0/24`
   - Automatically assigns public IP addresses to resources launched within it (`map_public_ip_on_launch = true`).

## ⚙️ Prerequisites & Tools
- Ubuntu on WSL2
- Terraform (v1.17.1+)
- AWS CLI (v2.x)

## 📦 How to Run
1. Clone the repository:
   ```bash
   git clone <your-repo-url>
   cd terraform-aws-vpc
