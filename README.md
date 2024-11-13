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

