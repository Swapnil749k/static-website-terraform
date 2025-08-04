🌐 Deploy a Static Website Using Terraform on AWS
This project provisions a complete infrastructure to host a static website using Terraform on AWS. It includes:

S3 Bucket for hosting static content (HTML, CSS, JS)

Route53 (Optional) for custom domain and DNS management

IAM Policy for secure access

🚀 Features
Fully automated infrastructure deployment with Terraform

S3 bucket configured for static website hosting

Optional SSL using ACM and CloudFront

Versioning and public-read access configuration

Easy integration with GitHub Actions for CI/CD

🧱 Services Used
Amazon S3 – stores static website files

Amazon CloudFront – delivers content via CDN

Amazon Route53 – DNS management (optional)

AWS Certificate Manager (ACM) – for HTTPS (optional)

IAM – for permissions

📁 Project Structure
bash
Copy
Edit
terraform/
│
├── main.tf             # AWS resources (S3, CloudFront, etc.)
├── variables.tf        # Input variables
├── outputs.tf          # Outputs (bucket URL, etc.)
├── backend.tf          # Remote state configuration (optional)
└── terraform.tfvars    # Variable values
⚙️ How to Use

# 1. Clone the repo
git clone https://github.com/yourusername/static-website-terraform.git
cd static-website-terraform

# 2. Initialize Terraform
terraform init

# 3. Review and apply the plan
terraform plan
terraform apply
📸 Output Example
Static Website URL: http://your-bucket-name.s3-website-ap-south-1.amazonaws.com
