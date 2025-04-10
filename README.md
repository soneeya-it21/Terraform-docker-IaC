# 🚀 Terraform Docker IaC

This project demonstrates using **Terraform** as Infrastructure as Code (IaC) to provision a **Docker container** running an NGINX web server. The container is launched on an **AWS EC2 instance**.

---

## 🛠️ Tech Stack

- **Terraform** – Infrastructure provisioning
- **Docker** – Container management
- **NGINX** – Lightweight web server (default image)
- **AWS EC2** – Host environment (Ubuntu instance)

---

## 📁 Files in This Repo

- `main.tf` – Terraform configuration to spin up a Docker container
- `execution_log.txt` – Sample Terraform command outputs (init, plan, apply, destroy)
- `README.md` – Project documentation

---

## ✅ What This Project Does

1. Initializes the Docker provider using Terraform.
2. Pulls the latest NGINX image.
3. Creates a Docker container and exposes port `8080`.
4. The container can be accessed via `http://<EC2_PUBLIC_IP>:8080`.

---

## 🚀 How to Run This Project

### 1. Install Required Tools

- Docker
- Terraform
- AWS EC2 instance with Docker installed (SSH via MobaXTerm or terminal)

---

### 2. Terraform Steps

bash
terraform init          # Initialize Terraform
terraform plan          # Review the execution plan
terraform apply         # Create the container
terraform destroy       # Tear down the container
terraform state list    # View Terraform-managed resources
