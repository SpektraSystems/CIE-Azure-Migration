**Contents** 

<!-- TOC -->

- [CIE - Azure Migration hands-on lab step-by-step](#cie-azure-migration-hands-on-lab-step-by-step)
  - [Abstract and learning objectives](#abstract-and-learning-objectives)
  - [Overview](#overview)
  - [Solution architecture](#solution-architecture)
  - [Requirements](#requirements)
  - [Exercise 1: Sign Up for pre configured environment and verify subscription access](#exercise-1-sign-up-for-pre-configured-environment-and-verify-subscription-access)
    - [Help references](#help-references)
    - [Task 1: Sign Up for pre configured environment](#task-1-sign-up-for-pre-configured-environment)
    - [Task 2: Login to your Azure Portal and Verify access to the Subscription](#task-2-login-to-azure-portal-and-verify-access-to-the-subscription)
  

<!-- /TOC -->

## Exercise 1: Sign Up for pre configured environment and verify subscription access

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
