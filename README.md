# terraform-portfolio-site
# Terraform AWS S3 Static Website Hosting

This Terraform project provisions an **AWS S3 bucket** configured to host a static website. It includes the necessary resources for bucket ownership controls, public access settings, bucket policy, and uploads of `index.html` and `error.html` files.

---

## Project Structure

- `main.tf` — Main Terraform configuration creating the S3 bucket, policies, and website hosting setup.
- `variable.tf` — Declares variables, such as the S3 bucket name.
- `provider.tf` — AWS provider configuration (region and credentials).
- `index.html` — The static website’s homepage.
- `error.html` — The custom error page for the static website.

---

## Usage

1. **Set your AWS credentials** in `provider.tf` or configure them using environment variables or AWS CLI.

2. **Set your bucket name** in `variable.tf`.

3. Initialize Terraform and apply the configuration:

   ```bash
   terraform init
   terraform apply
   terraform destroy
