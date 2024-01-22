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

From the sidebar, we select **Developer settings** -> **Personal access tokens**

![image](https://github.com/luiscoco/AzureDevops_Sample3_Connecting-Azure-DevOps-with-GitHub/assets/32194879/ca8feb1d-792b-41b3-8dfa-f07cb5d597c3)

We click on Generate new token.

![image](https://github.com/luiscoco/AzureDevops_Sample3_Connecting-Azure-DevOps-with-GitHub/assets/32194879/808f097d-3b11-4c3b-9ba5-fa1638165c0b)

We give your token a descriptive name, select the scopes or permissions you want to grant this token (for Azure DevOps, select repo, admin:repo_hook), and then click Generate token

![image](https://github.com/luiscoco/AzureDevops_Sample3_Connecting-Azure-DevOps-with-GitHub/assets/32194879/8931666f-f893-40a1-8bba-bc0c8fa35107)

![image](https://github.com/luiscoco/AzureDevops_Sample3_Connecting-Azure-DevOps-with-GitHub/assets/32194879/a67a5c8d-36db-4cf8-b332-4a5925fef552)

We copy the generated token and we save it somewhere secure; you won’t be able to see it again

![image](https://github.com/luiscoco/AzureDevops_Sample3_Connecting-Azure-DevOps-with-GitHub/assets/32194879/83dbac73-b7b8-420d-85f7-933d08f31a70)
