<p align="center">
  <img src="https://github.com/user-attachments/assets/ffd50746-4f18-4308-8160-81f15c4dd28b" width="150" height="auto">
  <h1 align="center">Entra ID Management on Azure</h1>
</p>

#### *In this tutorial, we will:*
*•	Secure and manage identities with Microsoft Entra ID.*

*•	Create and oversee users and groups.*

#### Tasks:
 1. Create a Microsoft Entra ID tenant.
 2. Create and configure internal and external user accounts.
 3. Establish groups and assign members.

## Task 1: Create a Microsoft Entra ID tenant.

Create a new Microsoft Entra ID tenant (a dedicated instance of Entra ID for your organization) to manage identities.

1.	In the Azure portal, search for and select "Microsoft Entra ID".
2.	On the "Microsoft Entra ID" blade, click "Manage tenants".
3.	On the "Manage tenants" blade, click "+ Create".
4.	Select the default tenant type (e.g., "Microsoft Entra ID"), then click "Next: Configuration".

<p align="center">
<img src="https://github.com/user-attachments/assets/7bdcfa2d-bef5-4cc6-a45e-61dbd6cc9708">
</p>

5.	On the "Configuration" tab, enter the following values:
    -  Organization name: Enter your organization’s name (e.g., "Contoso Lab").
    -  Initial domain name: Enter a unique domain name (e.g., "contosolab"). This forms the initial domain (e.g., "contosolab.onmicrosoft.com").
    -  Country/Region: Select your country or region (e.g., "United States").

<p align="center">
<img src="https://github.com/user-attachments/assets/bf73498d-43fd-4664-a6dd-b001cfc3364d">
</p>

6.	Click "Review + Create", then click "Create".

<p align="center">
<img src="https://github.com/user-attachments/assets/ce49a2dd-5e8e-4d1b-856c-3ae83f6d1dd1">
</p>

7.	After the tenant is created, on the confirmation blade, click the "Click here to navigate to your new tenant" link. (A new browser tab opens with your new tenant’s Microsoft Entra ID dashboard.)

<p align="center">
<img src="https://github.com/user-attachments/assets/47e7b2e7-7f3b-4d13-8333-421e14bd79a3">
</p>

## Task 2: Create and configure internal and external user accounts.

Create and configure user accounts in Microsoft Entra ID to store information such as name, department, and contact details. This task covers both internal and external users.

1.	From the "Microsoft Entra ID" blade, click "Manage tenants".
2.	Select your newly created tenant (e.g., "Contoso Lab") from the list.

<p align="center">
<img src="https://github.com/user-attachments/assets/b158e9fd-32af-4079-976a-9a6d224c7e1b">
</p>

3.	Navigate to the Microsoft Entra ID dashboard at entra.microsoft.com.
4.	Expand "Identity" in the left menu, then select "Users" > "All users".
5.	In the "New user" drop-down, select "Create new user" to add an internal user.

<p align="center">
<img src="https://github.com/user-attachments/assets/acae9b7b-1d37-4365-8dcb-53faf01a06d9">
</p>

6.	On the "Basics" tab, configure:
    -  User principal: Enter a username (e.g., "john.doe@contosolab.onmicrosoft.com").
    -  Display name: Enter a full name (e.g., "John Doe").
    -  Auto-generate password: Check this box to create a temporary password.
    -  Account enabled: Check this box to activate the account.

<p align="center">
<img src="https://github.com/user-attachments/assets/351837d8-c85d-4391-92ff-d50d345e8b93">
</p>

7.	On the "Properties" tab, configure:
    -  Job title: Enter a title (e.g., "Developer").
    -  Department: Enter a department (e.g., "Engineering").
    -  Usage location: Select a location (e.g., "United States").

<p align="center">
<img src="https://github.com/user-attachments/assets/48ac8af9-bc33-4958-a392-b0df60ac6270">
</p>

8.	Click "Review + create", then click "Create".
9.	To invite an external user, return to the "New user" drop-down and select "Invite an external user".
10.	Configure the external user:
    -  Email: Enter the external user’s email (e.g., "jane.smith@example.com").
    -  Display name: Enter a full name (e.g., "Jane Smith").
    -  Send invite message: Check this box.
    -  Message: Enter a custom invitation message (e.g., "Welcome to Contoso Lab!").
11.	On the "Properties" tab, configure:
    -  Job title: Enter a title (e.g., "Consultant").
    -  Department: Enter a department (e.g., "External").
    -  Usage location: Select a location (e.g., "United States").
12.	Click "Review + create", then click "Create". (An invitation email is sent to the external user.)

<p align="center">
<img src="https://github.com/user-attachments/assets/5912274f-1aef-4d02-8c4b-b620f0d536e6">
</p>

<p align="center">
<img src="https://github.com/user-attachments/assets/7ffccca2-85ac-4a58-9905-b2f13daa75fa">
</p>

13.	Refresh the "All users" page and confirm both the internal and external users appear.

<p align="center">
<img src="https://github.com/user-attachments/assets/9bd0dadf-c9ac-4813-8b9f-7fc6a85b7336">
</p>

## Task 3: Establish groups and assign members.

Create a group in Microsoft Entra ID to manage users and devices collectively. Groups can be static (manually managed) or dynamic (automatically updated based on attributes like job title), with dynamic groups requiring an Entra ID Premium P1 or P2 license.

1.	In the Azure portal, search for and select "Groups".
2.	On the "All groups" blade, click "+ New group".
3.	Configure the new group:
    -  Group type: Select "Security" (for access control) or "Microsoft 365" (for collaboration).
    -  Group name: Enter a name (e.g., "Engineering Team").
    -  Group description: Enter a description (e.g., "Group for engineering staff").
    -  Membership type: Choose "Assigned" (static) or "Dynamic User/Device" (if you have a Premium license).

<p align="center">
<img src="https://github.com/user-attachments/assets/d2f82f4b-fe36-43ea-a430-3b49a0c52c8f">
</p>

4.	Click "No owners selected", then on the "Add owners" page search for and select yourself as the owner, then click "Select".
5.	Click "No members selected", then on the "Add members" pane search for and select the internal and external users created in Task 2 (e.g., "John Doe" and "Jane Smith"), then click "Select".

<p align="center">
<img src="https://github.com/user-attachments/assets/9705ad90-906a-45ad-8875-0ecd44053afa">
</p>

6.	Click "Create" to deploy the group.
7.	Refresh the "All groups" page and confirm your group (e.g., "Engineering Team") appears.

<p align="center">
<img src="https://github.com/user-attachments/assets/7b941dd9-a6c9-4bf8-bd74-585b2e64e897">
</p>
