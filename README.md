## 🚀 AWS Infrastructure Setup using Terraform

**(VPC + 2 EC2 + Apache + Load Balancer + S3)**

---

## 📌 Project Overview

This project demonstrates how to deploy a basic production-style AWS infrastructure using **Terraform**.
The setup includes a custom VPC, two EC2 instances running Apache with different web pages, and an Application Load Balancer that distributes traffic between them.

Everything is created using **Infrastructure as Code (IaC)** so the entire environment can be recreated anytime.

---

## 🏗️ Architecture

* Custom VPC
* Public subnets
* Internet Gateway
* Route tables
* 2 EC2 instances
* Apache web server on both instances
* Different web page on each instance
* Application Load Balancer
* Target group with health checks
* S3 bucket (for storage/state or assets)

Traffic flow:

```
User → Load Balancer → EC2 Instance 1 or EC2 Instance 2 → Apache Web Page
```

---

## 🛠️ Tech Stack

* AWS (VPC, EC2, ALB, S3)
* Terraform
* Linux
* Apache Web Server

---

## 📂 Project Structure

```
terraform-aws-project/
│
├── main.tf
├── variables.tf
├── provider.tf
├── userdata.sh
└── README.md
```

---

## ⚙️ Prerequisites

Before running this project, make sure you have:

* AWS account
* IAM user with admin or required permissions
* Terraform installed
* AWS CLI installed
* AWS CLI configured

```bash
aws configure
terraform -v
```

---

## 🚀 How to Run

### 1️⃣ Initialize Terraform

```bash
terraform init
```

### 2️⃣ Check Plan

```bash
terraform plan
```

### 3️⃣ Apply Infrastructure

```bash
terraform apply
```

Type `yes` when prompted.

Terraform will create:

* VPC
* Subnets
* EC2 instances
* Load balancer
* Security groups

---

## 🌐 Access Application

After deployment, Terraform will output:

```
LoadBalancer DNS: http://xxxx.elb.amazonaws.com
```

Open it in browser.
Refresh multiple times → you will see **different Apache pages** from both servers.

---

## 🧠 Key Learnings

* Terraform state management
* Infrastructure as Code basics
* AWS networking (VPC, subnet, routing)
* Load balancer configuration
* EC2 provisioning with user data
* Debugging Terraform issues
* Security group configuration

---

## ⚠️ Challenges Faced

* Terraform showing “No changes” due to state
* Load balancer health check failures
* Security group port issues
* Apache not accessible initially
* Understanding resource dependencies
* Recreating resources using Terraform

---

## 🧹 Destroy Infrastructure

To avoid AWS charges:

```bash
terraform destroy
```

---

## 📸 Output Example

* Two EC2 instances running Apache
* Load balancer distributing traffic
* Different web page on each refresh

---

## 👨‍💻 Author

**Nadeem Sufiyan**
Aspiring DevOps Engineer
AWS | Terraform | Kubernetes

---


If you’re learning DevOps or Terraform, this is a great beginner-to-intermediate hands-on project.
