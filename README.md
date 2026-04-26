# Github-CICD

**Flask CI/CD Pipeline using GitHub Actions**

**Project Overview**

This project demonstrates the implementation of a CI/CD (Continuous Integration and Continuous Deployment) pipeline for a Python Flask application using GitHub Actions.

The pipeline automates:

Dependency installation
Running tests
Building the application
Deployment to staging and production environments

**Technologies Used**

Python 3.10
Flask
Pytest
GitHub Actions

**Project Structure**
<img width="1146" height="409" alt="image" src="https://github.com/user-attachments/assets/0fa7e43b-6326-4e7c-873b-32b25203406c" />

**CI/CD Workflow Explanation**
The pipeline is defined in:

**Workflow Triggers**

<img width="870" height="278" alt="image" src="https://github.com/user-attachments/assets/3f03c1cf-8e3f-4b68-9993-86bf3411656f" />

**CI/CD Workflow Explanation**
<img width="1186" height="362" alt="image" src="https://github.com/user-attachments/assets/a34b439f-1b4a-4638-995f-6e96abc8ba03" />

**Workflow Stages**
**Install Dependencies**
Installs required Python packages using pip
**Run Tests**
Executes test cases using pytest
Ensures code quality before deployment
**Build**
Prepares the application after successful tests
**Deploy to Staging**
Triggered when code is pushed to staging branch
Simulates deployment to staging server
**Deploy to Production**
Triggered when a release tag (e.g., v1.0) is created
Simulates production deployment

**Environment Secrets**
The following secrets are configured in repository settings:

Secret Name	Description
<img width="1176" height="318" alt="image" src="https://github.com/user-attachments/assets/86b8534c-64a6-4df8-ba4b-f229a29c1fd8" />
.
**How to Run the Pipeline**
**Trigger CI (Main Branch)**
1.Make a change in main
2.Commit changes
3.Go to Actions tab to view pipeline execution
**Trigger Staging Deployment**
1.Switch to staging branch
2.Make a small code change
3.Commit changes
4.Pipeline will deploy to staging
**Trigger Production Deployment**
1.Go to Releases
2.Click Create new release
3.Add tag (e.g., v1.0)
4.Publish release
5.Production deployment will run automatically

**Successful CI Pipeline**
<img width="1202" height="330" alt="image" src="https://github.com/user-attachments/assets/7add8d1e-1bf1-472a-b4e3-4c622362a79d" />

**Staging Deployment**

<img width="1192" height="263" alt="image" src="https://github.com/user-attachments/assets/801355d8-26ca-47c7-9cf8-e43818424573" />
<img width="1194" height="272" alt="image" src="https://github.com/user-attachments/assets/24f83da2-1bec-4453-9def-691c4562d4d6" />

<img width="1222" height="560" alt="image" src="https://github.com/user-attachments/assets/89f14653-b3ce-4530-9b83-c54de72c911c" />

<img width="719" height="871" alt="image" src="https://github.com/user-attachments/assets/c9ddc5cb-8117-4a3c-858f-1259ba243c55" />
<img width="743" height="560" alt="image" src="https://github.com/user-attachments/assets/522b5091-a7b7-4865-addb-215652f31816" />




**Production Deployment**
<img width="863" height="321" alt="image" src="https://github.com/user-attachments/assets/29d756f1-c2ef-43e5-9e30-dfc396346e2b" />
<img width="848" height="301" alt="image" src="https://github.com/user-attachments/assets/05e02831-b752-4eb8-866b-72e2c795b296" />
<img width="856" height="303" alt="image" src="https://github.com/user-attachments/assets/f37d4581-7f69-4218-a752-062767da8894" />



**Key Learning Outcomes**
Understanding CI/CD concepts
Automating workflows using GitHub Actions
Writing and running tests using pytest
Managing branches (main and staging)
Using GitHub Secrets for secure deployments

