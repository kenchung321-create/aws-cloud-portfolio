# AWS Cloud Portfolio Architecture (IaC)

Automated infrastructure deployment for a high-availability, secure static portfolio website on AWS using Terraform.

## Architecture & Features
- **AWS S3**: Private bucket hosting web assets.
- **AWS CloudFront**: CDN for global edge caching and SSL/TLS encryption (HTTPS).
- **Origin Access Control (OAC)**: Restricts S3 access exclusively to CloudFront.
- **Terraform (IaC)**: Fully automated creation and teardown of cloud resources.

## How to Deploy
1. `terraform init`
2. `terraform apply`
3. `aws s3 cp index.html s3://<your-bucket-name>/index.html`
