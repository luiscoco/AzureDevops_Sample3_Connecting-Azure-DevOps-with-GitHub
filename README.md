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

We are redirected to continue configuring the Pipeline.

We select the **Starter Pipeline** option to input the **yaml** file code

![image](https://github.com/luiscoco/AzureDevops_Sample3_Connecting-Azure-DevOps-with-GitHub/assets/32194879/a1e95c0c-44f2-48db-a495-846c361f72cb)



## 3. Connect Azure DevOps to GitHub

### 3.1. Using Azure Pipelines

In Azure DevOps, we go to your project and we select **Pipelines** from the left navigation panel

We click on **Create Pipeline**

![image](https://github.com/luiscoco/AzureDevops_Sample3_Connecting-Azure-DevOps-with-GitHub/assets/32194879/07db76ca-4edf-4abd-af2a-8215a750e789)

We choose **GitHub** as the **code source**

![image](https://github.com/luiscoco/AzureDevops_Sample3_Connecting-Azure-DevOps-with-GitHub/assets/32194879/471da684-e2f1-47f1-b096-8d3a94458485)

You may be prompted to sign into GitHub and authorize Azure Pipelines if you haven't already connected your GitHub account to Azure DevOps.

After authorization, select the repository you want to connect to Azure DevOps.

We select the Github repo to connect to

![image](https://github.com/luiscoco/AzureDevops_Sample3_Connecting-Azure-DevOps-with-GitHub/assets/32194879/7211f0ef-0d6c-49a9-9bf6-b9deaf884fba)

We automatically navigate to the following page

![image](https://github.com/luiscoco/AzureDevops_Sample3_Connecting-Azure-DevOps-with-GitHub/assets/32194879/1e900144-ccb1-4ab2-8992-197c65e63d9f)

We scroll down and select the repo and press the button **Approve and Install**

![image](https://github.com/luiscoco/AzureDevops_Sample3_Connecting-Azure-DevOps-with-GitHub/assets/32194879/bda79cdb-3ae8-4d2c-adad-a70f479836e2)

We are redirected to the Azure DevOps to continue with the PipeLine configuration

We select the **Starter pipeline** option to input the **yaml** file source code

![image](https://github.com/luiscoco/AzureDevops_Sample3_Connecting-Azure-DevOps-with-GitHub/assets/32194879/8a889afc-aaed-48a0-ae05-1249605df404)

### 3.2. Service Connection Method

We go to **Project settings** in the bottom left corner of your Azure DevOps project

Under **Pipelines**, we select **Service connections**

We click on **New service connection** and choose **GitHub**

![image](https://github.com/luiscoco/AzureDevops_Sample3_Connecting-Azure-DevOps-with-GitHub/assets/32194879/9bb7c3c6-70f5-4d79-af22-aeac9aebc2f2)

We choose **GitHub** via **Personal Access Token (PAT)**, we enter the PAT you generated earlier, and we give your connection a name

![image](https://github.com/luiscoco/AzureDevops_Sample3_Connecting-Azure-DevOps-with-GitHub/assets/32194879/87752df0-195d-4923-8753-ab8885efa282)

![image](https://github.com/luiscoco/AzureDevops_Sample3_Connecting-Azure-DevOps-with-GitHub/assets/32194879/22d234ee-bf9c-4391-ae83-1edbd6bf982e)

![image](https://github.com/luiscoco/AzureDevops_Sample3_Connecting-Azure-DevOps-with-GitHub/assets/32194879/e8809aac-874d-4740-bfa0-104a2d21fcef)

After we setting up the connection, we can use it in your pipelines to access our GitHub repositories

