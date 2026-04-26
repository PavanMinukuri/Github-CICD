# Github-CICD

GitHub-CICD
Flask CI/CD Pipeline using GitHub Actions
Project Overview
This project demonstrates the implementation of a CI/CD (Continuous Integration and Continuous Deployment) pipeline for a Python Flask application using GitHub Actions.

The pipeline automates:

Dependency installation
Running tests
Building the application
Deployment to staging and production environments
Technologies Used
Python 3.10
Flask
Pytest
GitHub Actions
Project Structure
image
CI/CD Workflow Explanation
The pipeline is defined in:

Workflow Triggers
Event	Action
Push to main	Runs CI pipeline
Push to staging	Runs CI + deploy to staging
Release creation	Deploy to production
CI/CD Workflow Explanation
image
Workflow Stages
Install Dependencies
Installs required Python packages using pip
Run Tests
Executes test cases using pytest
Ensures code quality before deployment
Build
Prepares the application after successful tests
Deploy to Staging
Triggered when code is pushed to staging branch
Simulates deployment to staging server
Deploy to Production
Triggered when a release tag (e.g., v1.0) is created
Simulates production deployment
Environment Secrets
The following secrets are configured in repository settings:

Secret Name	Description
STAGING_KEY	Used for staging deployment
PROD_KEY	Used for production deployment
Note: These are stored securely using GitHub Secrets.

How to Run the Pipeline
Trigger CI (Main Branch)
Make a change in main
Commit changes
Go to Actions tab to view pipeline execution
Trigger Staging Deployment
Switch to staging branch
Make a small code change
Commit changes
Pipeline will deploy to staging
Trigger Production Deployment
Go to Releases
Click Create new release
Add tag (e.g., v1.0)
Publish release
Production deployment will run automatically
Successful CI Pipeline
image
Staging Deployment
imageimageimageimageimage
Production Deployment
imageimageimage
Key Learning Outcomes
Understanding CI/CD concepts
Automating workflows using GitHub Actions
Writing and running tests using pytest
Managing branches (main and staging)
Using GitHub Secrets for secure deployments
Author
Your Name : Pavan Kumar Minukuri
