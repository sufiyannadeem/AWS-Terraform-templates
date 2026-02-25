# 🚀 AWS Infrastructure Provisioning using Terraform

This project demonstrates how to provision a complete AWS infrastructure using **Terraform (Infrastructure as Code)**.
The setup includes a custom VPC, subnets, EC2 instances, networking components, and S3 integration — all automated using Terraform.

---

## 📌 Architecture Overview

* Custom **VPC**
* Public subnets in multiple AZs
* Internet Gateway
* Route tables
* EC2 instances
* Amazon S3 bucket
* Security groups
* Fully automated using Terraform

This project follows best practices for **Infrastructure as Code (IaC)** and reproducible cloud environments.

---

## 🛠️ Tech Stack

* Terraform
* AWS (VPC, EC2, S3, Networking)
* AWS CLI
* Linux

---

## 📂 Project Structure

```
.
├── main.tf
├── variables.tf
├── provider.tf
├── terraform.tfvars
└── README.md
```

---

## ⚙️ Prerequisites

Make sure you have installed:

* Terraform
* AWS CLI
* AWS account
* Configured credentials

```bash
aws configure
```

---

## 🚀 Deployment Steps

### 1️⃣ Initialize Terraform

```bash
terraform init
```

### 2️⃣ Validate configuration

```bash
terraform validate
```

### 3️⃣ Plan infrastructure

```bash
terraform plan
```

### 4️⃣ Apply configuration

```bash
terraform apply
```

Type `yes` when prompted.

---

## 🧹 Destroy Infrastructure

To remove all resources:

```bash
terraform destroy
```

---

## 📚 Key Learnings

* Infrastructure as Code using Terraform
* AWS VPC and networking setup
* Terraform state management
* Resource dependencies
* Idempotent deployments
* Debugging Terraform issues
* Remote vs local state
* AWS IAM permissions

---

## ⚠️ Challenges Faced

* Terraform state conflicts
* Resource recreation issues
* IAM permission errors
* Networking misconfigurations
* Understanding Terraform lifecycle
* Debugging “No changes” message
* Managing backend state

---

## 💡 Future Improvements

* Add remote backend (S3 + DynamoDB)
* Use Terraform modules
* Add Auto Scaling
* Add Load Balancer
* CI/CD with GitHub Actions
* EKS deployment

---

## 👨‍💻 Author

**Nadeem Sufiyan**
Aspiring DevOps Engineer

* LinkedIn: 

---

## ⭐ If you found this useful

Give this repo a star ⭐ and connect with me on LinkedIn.
