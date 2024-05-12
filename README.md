# GCP Terraform Jenkins Project

This project sets up a Continuous Integration/Continuous Deployment (CI/CD) pipeline using Jenkins and Terraform to manage resources on Google Cloud Platform (GCP).

## Jenkins Pipeline Configuration

The `Jenkinsfile` in this repository defines the CI/CD pipeline with the following stages:

1. **Git Checkout:** Retrieves the latest code from the GitHub repository.
2. **Terraform Init:** Initializes Terraform in the Jenkins environment.
3. **Terraform Plan:** Generates an execution plan for Terraform.
4. **Manual Approval:** Waits for manual approval before proceeding.
5. **Terraform Apply:** Applies the Terraform execution plan to provision resources on GCP.

## Terraform Configuration

The `main.tf` file contains the Terraform configuration to create a Google Cloud Storage (GCS) bucket.

## Additional Notes

- A Git token and GCP service account key (`gcp-key`) are required for authentication.
- Ensure proper access control and permissions are configured for Jenkins and GCP resources.

## Prerequisites:

A cloud provider account (e.g., Google Cloud Platform) with a deployable Jenkins instance
Access to a GitHub repository
