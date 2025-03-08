<p align="center">
  <img src="https://github.com/user-attachments/assets/ffd50746-4f18-4308-8160-81f15c4dd28b" width="150" height="auto">
  <h1 align="center">Entra ID Management on Azure</h1>
</p>

#### *In this tutorial, we will:*
*- Secure and manage identities using Microsoft Entra ID.*

*- Implement and oversee users and groups.*

#### Tasks:
 1. Create a Microsoft Entra ID tenant.
 2. Create and configure internal and external user accounts.
 3. Establish groups and assign members.

## Task 1: Create a Microsoft Entra ID tenant.

In this task, you will create a new Azure AD tenant.

1.	In the Azure portal, search for and select Microsoft Entra ID and click "Manage tenants:"
2.	On the Manage tenants blade, click "+ Create" and select the following option.

<p align="center">
<img src="https://github.com/user-attachments/assets/7bdcfa2d-bef5-4cc6-a45e-61dbd6cc9708">
</p>

3.	Click "Next : Configuration". On the Configuration tab, enter the required values, Organization name, Initial domain name and Country/Region:

<p align="center">
<img src="https://github.com/user-attachments/assets/bf73498d-43fd-4664-a6dd-b001cfc3364d">
</p>

4.	Click "Review + Create" and then click Create.

<p align="center">
<img src="https://github.com/user-attachments/assets/ce49a2dd-5e8e-4d1b-856c-3ae83f6d1dd1">
</p>

5.  In the confirmation blade of the newly created tenant select Click here to navigate to your new tenant: Contoso Lab link. A new tab will open in your browser and you will be presented with your newly created Tenant.

<p align="center">
<img src="https://github.com/user-attachments/assets/47e7b2e7-7f3b-4d13-8333-421e14bd79a3">
</p>

## Task 2: Create and configure internal and external user accounts.

In this task, you will create and configure user accounts. User accounts will store user data such as name, department, location, and contact information.

1.	From the Overview blade select "Manage tenants". You will now see your tenant. A tenant is a specific instance of Microsoft Entra ID containing accounts and groups. Depending on your situation, you can create more tenants and Switch between them.

<p align="center">
<img src="https://github.com/user-attachments/assets/b158e9fd-32af-4079-976a-9a6d224c7e1b">
</p>

2.	Now we will create a new user, go to the Microsoft Entra ID dashboard entra.microsoft.com and expand Identity.
3.	Select "Users > All users" from the left hand side, then in the New user drop-down select "Create new user".

<p align="center">
<img src="https://github.com/user-attachments/assets/acae9b7b-1d37-4365-8dcb-53faf01a06d9">
</p>

4.	In the Basics tab enter values for User principal, Display name, Auto-generate password, Account enabled.

<p align="center">
<img src="https://github.com/user-attachments/assets/351837d8-c85d-4391-92ff-d50d345e8b93">
</p>

5. In the Properties tab, enter values for Job title, Department and Usage location.

<p align="center">
<img src="https://github.com/user-attachments/assets/48ac8af9-bc33-4958-a392-b0df60ac6270">
</p>

6.	Once you have finished reviewing, select "Review + create" and then "Create". We will proceed to invite an external user.
7.	In the New user drop-down select Invite an external user and enter values for Email, Display name, Send invite message and Message. In the Properties tab complete the basic information, Job title, Department and Usage location. This will send an invitation to the email.

<p align="center">
<img src="https://github.com/user-attachments/assets/5912274f-1aef-4d02-8c4b-b620f0d536e6">
</p>

<p align="center">
<img src="https://github.com/user-attachments/assets/7ffccca2-85ac-4a58-9905-b2f13daa75fa">
</p>

8.  Refresh the page and confirm the invited user was created.

<p align="center">
<img src="https://github.com/user-attachments/assets/9bd0dadf-c9ac-4813-8b9f-7fc6a85b7336">
</p>

## Task 3: Establish groups and assign members.

In this task, you will create a group account, which can include both user accounts and devices. Members can be assigned to groups in two primary ways: statically or dynamically. In static groups, administrators manually add and remove members. In contrast, dynamic groups update automatically based on user account or device attributes, such as job title.

1.	In the Azure portal, search for and select Groups.
2.	In the All groups blade, select "+ New group" and "create a new group". Enter the values for Group type, Group name, Group description and Membership type (an Entra ID Premium P1 or P2 license is required for dynamic membership).

<p align="center">
<img src="https://github.com/user-attachments/assets/d2f82f4b-fe36-43ea-a430-3b49a0c52c8f">
</p>

4.	Select "No owners selected" and in the Add owners page, search for and select yourself as the owner.
5.	Select "No members selected" and in the Add members pane, search for and select the previously created users, add both of them to the group.

<p align="center">
<img src="https://github.com/user-attachments/assets/9705ad90-906a-45ad-8875-0ecd44053afa">
</p>

6.  Select "Create" to deploy the group.
7.	Refresh the page and ensure your group was created.

<p align="center">
<img src="https://github.com/user-attachments/assets/7b941dd9-a6c9-4bf8-bd74-585b2e64e897">
</p>
