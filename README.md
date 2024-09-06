# Optimizing Web App Deployment on Azure with CI/CD Automation


# Overview
This project addresses the challenges of manual and error-prone deployment processes for web applications on Azure. It implements an automated CI/CD pipeline that streamlines deployment, ensuring reliability and efficiency.

## Key Components:
### Azure Container Registry (ACR):
- A place to store Docker containers (packages with your web app code and its environment). These containers are created when your app code is built and are saved in ACR for future use.

### GitHub Repository:
- The project’s code is saved on GitHub, which acts as a version control system. Developers can collaborate, and the latest code can be accessed by Azure for deployment.

### Azure DevOps:
- A tool that automates the process of building and deploying your app. When code is changed in GitHub, Azure DevOps automatically starts building the app and prepares it for deployment.

### Build Pipeline:
- The build pipeline fetches your project code from GitHub, creates a Docker container, and stores it in ACR. It automates the process of compiling your code and packaging it for deployment.

### Azure App Service:
- A platform that hosts your web application. It uses the Docker container stored in ACR to run your app, providing a cost-effective and scalable solution.

### Deployment Center:
- A section in the Azure portal where you can manually deploy your app’s Docker container from ACR to Azure App Service. It’s a useful tool if you prefer hands-on control over deployment.

### Release Pipeline:
- The release pipeline automatically deploys the app. Every time you commit changes to the main branch on GitHub, Azure DevOps handles the build and deployment steps automatically, ensuring that the latest version of your app is always live.

### Summary:
- By automating everything from building the app to deploying it, the project saves time, reduces mistakes, and allows you to easily make updates. This is a perfect way for beginners to deploy web applications without dealing with complicated manual steps.


## Problem Statement

Manual deployments are error-prone and time-consuming, leading to delays in feature releases. This project automates the CI/CD process, reducing errors and accelerating deployment.

## Project Description

This project automates the deployment pipeline for web applications on Azure using Docker containers. Code is pushed to a GitHub repository, triggering Azure DevOps to build and deploy the application using ACR and Azure App Service. This automated process enhances deployment speed and consistency.

## Complete Step By Step Process :
1. Create Container Repository:
![alt text](image.png)
2. Use Azure Devops Portal For Creating Service Connections From Devops To Github and ACR.
![alt text](image-1.png)
3. Create required Service Connection for the project
![alt text](image-3.png)
![alt text](image-2.png)
![alt text](image-4.png)
4. Push The Code To Github Repo Which Should Contain the Required Docker File.
![alt text](image-5.png)
5. Create Build Pipeline To Create And Store The Docker Container In ACR.
![alt text](image-6.png)
![alt text](image-7.png)
![alt text](image-8.png)
![alt text](image-9.png)
![alt text](image-13.png)
![alt text](image-12.png)
![alt text](image-10.png)
![alt text](image-11.png)
![alt text](image-14.png)
![alt text](image-15.png)
6. Docker Container Stored In The Repository.
![alt text](image-16.png)
7. Allow Access.
![alt text](image-17.png)
8. Create Web App.
![alt text](image-18.png)
9. Establish The Required Environment And Deploy if any eg. MongoDB
![alt text](image-19.png)
10. Create Release Pipeline.
![alt text](image-20.png)
![alt text](image-21.png)
![alt text](image-22.png)
![alt text](image-23.png)
![alt text](image-25.png)
![alt text](image-24.png)
![alt text](image-26.png)
![alt text](image-27.png)
![alt text](image-28.png)
![alt text](image-29.png)