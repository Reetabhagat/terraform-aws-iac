# Terraform AWS IaC Project 🚀

## 📌 Project Overview
This project demonstrates **Infrastructure as Code (IaC)** using **Terraform** to provision and manage AWS infrastructure in an automated, repeatable, and scalable way.

The infrastructure is created using Terraform instead of manual AWS Console steps.

---

## 🏗️ Infrastructure Components Created

Using Terraform, the following AWS resources are provisioned:

- ✅ **VPC**
- ✅ **Public Subnet**
- ✅ **Private Subnet**
- ✅ **Internet Gateway (IGW)**
- ✅ **Route Table & Route Table Association**
- ✅ **Security Group**
- ✅ **EC2 Instance**

---

## 🧱 Architecture Flow

VPC (10.0.0.0/16)
│
├── Public Subnet
│ ├── Internet Gateway
│ ├── Route Table (0.0.0.0/0 → IGW)
│ └── EC2 Instance
│
└── Private Subnet

---

## 📂 Project Structure

terraform-aws-iac/
├── main.tf # Main infrastructure resources
├── provider.tf # AWS provider configuration
├── variables.tf # Input variable declarations
├── terraform.tfvars # Variable values (ignored in git)
├── outputs.tf # Output values
├── .gitignore # Terraform ignored files
└── README.md # Project documentation


---

## ⚙️ Tools & Technologies Used

- **Terraform**
- **AWS (VPC, EC2, IAM, Subnets)**
- **Git & GitHub**
- **AWS CLI**

---

## 🔐 AWS Authentication

Terraform authenticates with AWS using **IAM User credentials** configured via AWS CLI:

```bash
aws configure

🚀 How to Run This Project
1️⃣ Initialize Terraform
terraform init

2️⃣ Validate Configuration
terraform validate

3️⃣ Preview Changes
terraform plan

4️⃣ Apply Infrastructure
terraform apply


Type yes when prompted.

📤 Terraform Outputs

After successful apply, Terraform outputs:

VPC ID
Public Subnet ID
Private Subnet ID
Internet Gateway ID

🧠 Key Learnings

Infrastructure provisioning using Terraform
Variable & output management
AWS networking fundamentals
Infrastructure automation best practices
Avoiding manual AWS Console dependency

🛑 Cleanup (Important)

To destroy all created resources:

terraform destroy

👩‍💻 Author

Reeta Bhaghat
DevOps / AWS Engineer
