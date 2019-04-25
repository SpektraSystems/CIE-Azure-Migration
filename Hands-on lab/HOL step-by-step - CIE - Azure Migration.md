**Contents** 

<!-- TOC -->

- [CIE - Azure Migration hands-on lab step-by-step](#cie-azure-migration-hands-on-lab-step-by-step)
  - [Abstract and learning objectives](#abstract-and-learning-objectives)
  - [Overview](#overview)
  - [Solution architecture](#solution-architecture)
  - [Requirements](#requirements)
  - [Exercise 1: Sign Up for pre configured environment and verify subscription access](#exercise-1-sign-up-for-pre-configured-environment-and-verify-subscription-access)
    - [Task 1: Sign Up for pre configured environment](#task-1-sign-up-for-pre-configured-environment)
    - [Task 2: Login to your Azure Portal and Verify access to the Subscription](#task-2-login-to-azure-portal-and-verify-access-to-the-subscription)
  - [Exercise 2: Migrate SQL server to azure SQL db offline](#exercise-2-migrate-sql-server-to-azure-db-offline)
    - [Help references](#help-references)
    - [Task 1: Validate and Migrate the AdventureWorks2008R2 Schema](#task-1-validate-and-migrate-the-adventureWorks2008R2-Schema)
    - [Task 2: ](#task-2-)
    - [Task 3: ](#task-3-)
    - [Task 4: ](#task-4-)
    - [Task 5: ](#task-5-)
    - [Task 6: ](#task-6-)
    - [Task 7: ](#task-7-)
  

<!-- /TOC -->

## Exercise 1: Sign Up for pre configured environment and verify subscription access
**Duration:** 5 Minutes
In this exercise, you will create a source environment and verify the access on azure subscription.

### Task 1: Sign Up for pre configured environment

Here, you will sign up for the lab.

1.	**Navigate** to bitly link which was provided by instructor and register by providing all required information with activation code and **clicking** on **SUBMIT button**.<br/>
  ![](Images/1_signup.jpg)

2. Once registration is accepted, you will be automatically redirected to the lab details page. Now, it is advised to save a copy of the URL of lab details page in browser. **Click** on the **Launch Lab** button to start the lab.<br/>
  ![](Images/2_launchlab.jpg)

3. You will see the environment details soon below.<br/>
  ![](Images/3_labdetails.jpg)

  Please ensure to take the values assigned to your deployment.
  
### Task 2: Login to your Azure Portal and Verify access to the Subscription

In this task, you will log into the **Azure Portal** using your Azure credentials and you will verify the type of role you are assigned in this Subscription.
1. **Navigate** to https://portal.azure.com and login (from the previous step).
1. **Enter** the **Username** which was displayed in the previous window and **click** on **Next**.<br/>
    ![](Images/4_username.jpg)
1. **Enter** the **Password** and click on **Sign in**. In the Stay signed in? pop-up window click on **Yes**.
    ![](Images/5_password.jpg)
1. Click on Resource Groups in left panel. You will see one Resource Group on which you have access. 
1. Click on **azure-migration-62244** Resource Group which contains the pre-deployed on-premises infrastructure.Here, 62244 is unique ID and it could be different.
   ![](Images/6_azuremigrationrg.jpg)
   
## Exercise 2: Migrate SQL Server to Azure SQL DB Offline

In this exercise, you will deploy **SQL Database** and **Azure Database Migration Service**. After that you will validate and Migrate the **schema** of on-prem(SQL Server 2008 R2) AdventureWorks2008R2 database to Azure SQL Database using Database Migration Assistant. Then you will migrate **on-prem** offline **AdventureWorks2008R2** database to **Azure SQL Database** using Azure Migration Service of azure.

### Task 1: Validate and Migrate the AdventureWorks2008R2 Schema

1. Go to https://portal.azure.com and login the you azure username and password as shown in previous steps.
1. Click on the **azure-migration-62244** Resource Group and click on the sqlvm and login to the sqlvm with Public IP or SQL VM DNS name using RDP . You can also find sqlvm admin username, password and sqlvm dns name on lab details page.
  * Username: **demouser**
  * Password: **demo@pass123**
1. After login to sql vm. Click on the **SQL Server Management Studio(SSMS)** icon on taskbar.
   ![](Images/7_ssms.jpg)
1. When SSMS popup for connect to database, then click on **Connect** button by keeping default values. Please note the default sql server name(SQL2008R2-VM) to use it later. </br>
   ![](Images/8_connect.jpg)
1. Now check and verify **AdventureWorks2008R2** database is preloaded in Object Explorer window.
   ![](Images/9_verifydb.jpg)
1. Now, click on the **Data Migration Assistant(DMA)** icon on taskbar.
   ![](Images/10_datamigrationassitant.jpg)
1. In this step, we will create New Assessment project.
    * Select **Assessment** in project type. Feel the values and click on **Create** button.
      * Project Name: **AzureDMSMigration**
      * Source server type: **SQL Server**
      * Target server type: Azure **SQL Database** </br>
        ![](Images/11_new.jpg)
    
   
  
