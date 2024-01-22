# AzureDevops: How to Connect Azure DevOps with GitHub

Connecting Azure DevOps with GitHub involves setting up a connection that allows you to integrate your GitHub repository with Azure DevOps services, such as Azure Pipelines for CI/CD.

Here’s a step-by-step guide on how to connect Azure DevOps with GitHub:

## 1. Create a New Project in Azure DevOps

We sign in to your Azure DevOps account

We navigate to the Azure DevOps portal and we create a new project if you haven’t done so already

We provide a name and description for your project

## 2. Generate GitHub Personal Access Token (PAT)

We go to GitHub and **sign in**

We click on your **profile icon** in the top right corner

![image](https://github.com/luiscoco/AzureDevops_Sample3_Connecting-Azure-DevOps-with-GitHub/assets/32194879/09b58098-7a7c-4c43-860b-5f676f4a0363)

We select the **Settings** option

![image](https://github.com/luiscoco/AzureDevops_Sample3_Connecting-Azure-DevOps-with-GitHub/assets/32194879/c6352d7a-7bd7-4d2f-904e-362e036f51f6)

From the sidebar, we select Developer settings > Personal access tokens.



Click on Generate new token.

Give your token a descriptive name, select the scopes or permissions you want to grant this token (for Azure DevOps, select repo, admin:repo_hook), and then click Generate token.

Copy the generated token and save it somewhere secure; you won’t be able to see it again.



