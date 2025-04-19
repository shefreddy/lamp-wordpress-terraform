# 🚀 LAMP Stack + WordPress on AWS EC2 with Terraform

This project sets up a **LAMP stack (Linux, Apache, MySQL, PHP)** and deploys **WordPress** on an Amazon EC2 instance using **Terraform**.

---

## 📦 What’s Included

- Amazon EC2 instance (Amazon Linux 2)
- Apache Web Server
- MariaDB (MySQL)
- PHP
- WordPress (latest version)
- Security Group allowing SSH, HTTP, and HTTPS
- EC2 user data script for automatic provisioning

---

## 📁 Project Structure

lamp-wordpress-terraform/ 
├── main.tf # Terraform resources
├── var.tf # Input variables 
├── outputs.tf # Output public IP 
├── install_lamp.sh # EC2 bootstrap script (LAMP + WordPress setup) 
├── generate_key.tf # SSH Key generator
└── README.md # Project documentation

---

## 1. 🚀 Getting Started

- AWS account
- Terraform installed
- AWS CLI configured (`aws configure`)
- An EC2 Key Pair (for SSH access)

---

## 2. 🚀 Deploy the Infrastructure

```bash
terraform init
terraform plan
terraform apply 
```

---

## 3. 🌐 Access WordPress

- After Terraform completes, find the public IP output:

Apply complete! Resources: 11 added, 0 changed, 1 destroyed.

Outputs:

lamp_server_url = "http://your-public-ip:80"
ssh_lamp_server_command = "ssh -i lamp_key_pair"

---


---

## 👨‍💻 Author

Built with ❤️ using Terraform and AWS.

Author: Freddy Shema
📌 GitHub Profile: https://github.com/shefreddy
