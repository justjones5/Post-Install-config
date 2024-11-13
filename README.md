<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket.<br />


<h2>Video Demonstration</h2>

- ### [YouTube: How To Configure osTicket, post-installation](https://www.youtube.com)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Post-Install Configuration Objectives</h2>

- Adding Roles
- Permissions
- Configure Departments
- Teams
- creating tickets/ users
- Agents
- Configuring SLA
- Help Topics

<h2>Configuration Steps</h2>

Step 1: Open osTicket and log in using the credentials created during the installation process.

![image](https://github.com/user-attachments/assets/35384838-f306-4f91-bc3d-9b42fe317a1d)


Step 2: Configure Roles

-Ensure you’re in the Admin panel (check the top-right corner; it should display "Agent" if you’re in the Admin panel).
- Go to the Agent tab, then select Roles > Add New Role.
   - Enter the name Supreme Admin.
- Check all boxes under the Tickets, Tasks, and Knowledgebase sections in the Permissions tab.
Click Add Role.

![image](https://github.com/user-attachments/assets/41afd265-415a-40b4-80f7-9bfa2f4754df)
![image](https://github.com/user-attachments/assets/0227afc1-2088-4ec1-9866-cb4edfe8b72a)

Step 3: Configure Departments
- Confirm that you're still in the Admin panel.
- Go to the Agent tab, then select Departments > Add New Department.
    - Enter System Administrators as the department name.
- Click Create Department.

![image](https://github.com/user-attachments/assets/540f1e92-b91a-45ed-9e02-a064b69f301e)
![image](https://github.com/user-attachments/assets/07b0f651-e9f3-446f-a4ea-751c853a2f29)

Step 4: Configure Teams
- Navigate to the Agent tab and choose Teams > Add New Team.
   - Enter Level II Support as the team name.
- In the Members tab, select your name from the Select Agent dropdown menu.
- Click Create Team.

![image](https://github.com/user-attachments/assets/76bb3839-d383-42a3-9535-ba59014e9d7f)

![image](https://github.com/user-attachments/assets/b78f9535-4c22-43ff-8712-65b3a1758bec)

Step 5: Allow Anyone to Create Tickets
Go to Settings > User Settings.
 -  Ensure the Registration Required option 
-    (Require registration and login to create tickets) is unchecked.

![image](https://github.com/user-attachments/assets/6a3046f4-6e7b-4cb6-97d4-2786e6c24584)

Step 6: Configure Agents
- Go to the Agent tab and select Add New Agent.
Enter the following details:
 - Name: Jane Doe
 - Email: jane.doe(@)osticket.com
 - Username: jane.doe
 - Click Set Password, then uncheck Send the Agent a Password Reset Email.
   - Set a password of your choice.
      - Uncheck the required password change at the next login.
        - Click Set.

![image](https://github.com/user-attachments/assets/945932c7-1d8f-48ec-b74d-1d5c99a3c118)
![image](https://github.com/user-attachments/assets/a4d98e8b-ec47-4af3-97d6-56cf790199f8)

Go to the Access tab.
- Under Primary Department:
  - Choose System Administrators from the Department dropdown.
  - Choose Supreme Admin from the Role dropdown.
Under Extended Access:
 - Select Department > Support > Add > Supreme Admin.
Navigate to the Team tab.
 - From the Team dropdown, select Level II Support.
- Click Add.
Click Create.

![image](https://github.com/user-attachments/assets/4a0bf9b2-3467-4da3-9a99-6388f4b6a146)
![image](https://github.com/user-attachments/assets/71eae0df-771f-4f59-ae2d-43537245001f)

- Create a new agent, replacing "Jane" with "John."
   - Follow the previous steps for creating an agent, but make these adjustments for the primary department:
   - In the Department dropdown, select Support.
   - In the Role dropdown, choose View Only.
- For Extended Access:
      -Select Department > Support > Save Changes.
![image](https://github.com/user-attachments/assets/123f8a2f-8971-4cab-8530-0e4ec880f428)
![image](https://github.com/user-attachments/assets/920926d6-466e-4a0d-b5b6-e37e0f213093)

Step 7: Configure Users

![image](https://github.com/user-attachments/assets/224b148a-7561-4d6c-b161-631a3b8d2f21)

- Go to the Users tab to create a new user.
  - Enter the following details:
    - Email Address: Karen(@)osticket.com
    - Full Name: Karen Karen
    -Click Add User.

    ![image](https://github.com/user-attachments/assets/49b3c9d9-677f-4309-ac15-0cb9ea079342)
    
 Go to the User tab again to create a new user.
  - Enter the following details:
  - Email Address: Ken(@)osticket.com
- Full Name: Ken Ken
- Click Add User.
 
![image](https://github.com/user-attachments/assets/5d08457d-8a8e-4934-afe9-446789c5da56)

Step 8: Configure Service Level Agreements (SLA)
- We'll create three SLA plans.
- Go to the Manage tab, then select SLA > Add New SLA Plan.
- Name: SEV-A
- Grace Period: 1
- Schedule: 24/7 (from the dropdown menu)
- Click Add Plan.

     ![image](https://github.com/user-attachments/assets/74b22906-b775-4a27-8960-7e687d4e29e3)
 
![image](https://github.com/user-attachments/assets/b0379e28-22c9-49bd-ae10-9b605852800e)

- Name: SEV-B
- Grace Period: 4
- Schedule dropdown menu: 24/7
- Select Add Plan

  ![image](https://github.com/user-attachments/assets/dc8d0e5b-092b-4ec8-971d-b0df6ba987e1)

- Name: SEV-C 
- Grace Period: 8
- Schedule dropdown menu: Monday - Friday 8AM - 5PM with U.S. Holidays
- Select Add Plan

  ![image](https://github.com/user-attachments/assets/4cedb250-4f4e-4953-8ba8-2f3a62639803)

Step 9: Configure Help Topics
We will create four Help Topics:
 Go to the Manage tab, then select Help Topics > Add New Help Topic.
 - Business Critical Outage
  - Personal Computer Issues
  - Equipment Request
  - Password Reset.
For each topic, click Add Topic.
![image](https://github.com/user-attachments/assets/e1fdc087-982d-4d21-81ee-037619f33d98)
