<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket.<br />


<h2>Video Demonstration</h2>

- ### [YouTube: How To Configure osTicket, post-installation](https://www.youtube.com/watch?v=19WpzGui8vw)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Post-Install Configuration Objectives</h2>

- Configure Roles (for grouping permissions)
- Configure Departments (Ticket Visiblity)
- Configure Teams
- Allow everyone to create tickets without having an account
- Configure Agents (workers)
- Configure Users (customers)
- Configure SLA
- Configure Help Topics (For when users create a ticket)

<h2>Configuration Steps</h2>

<p>
<img width="1440" alt="Screenshot 2025-05-12 at 2 29 18 PM" src="https://github.com/user-attachments/assets/c9ed9006-4b87-43e9-92fa-f30cbb69b3e7" />
</p>
<p>
On the admin panel of the osTicket site, at the top next to "Emails" click "Agents". Next to "Teams" click "Roles". You will see different levels of access. If you click on each one and go to "Permissions", certain boxes will/will not be checked off. Here you can assign roles and permissions to departments and indivisuals. You can also create/define your own role. Above where it says "Last Updated" click on "Add New Roles". Type the name of the role you want to create, for example: "Supreme Admin", then go to "Permissions" and check the boxes of the permissions you want this role to have for "Tickets", "Tasks" and "Knowledgebase". When finished, click "Add Role". 
</p>
<br />

<p>
<img width="1141" alt="Screenshot 2025-05-12 at 2 35 13 PM" src="https://github.com/user-attachments/assets/818f4436-d543-477c-89f3-47f9a6dd0b6c" />
</p>
<p>
On the admin panel, next to "Emails" click "Agents" then go to "Departments". Fill out the info of the new department you would like to create. Under "Access" this is where you can add agents who would be members of this department. When finished, click "Create Dept". 
</p>
<br />

<p>
<img width="1106" alt="Screenshot 2025-05-12 at 2 37 17 PM" src="https://github.com/user-attachments/assets/3413e05c-7bc4-4dd8-be58-e4c054816f7e" />
</p>
<p>
On the admin panel, next to "Emails" click "Agents" and then "Teams". On the right, choose "Add New Team". Fill out the info of the team you would like to create, for example: "Online Banking", and under "Members" add who would be apart of this team. When finished, click "Create Team". 
</p>
<br />

<p>
<img width="1133" alt="Screenshot 2025-05-12 at 2 41 03 PM" src="https://github.com/user-attachments/assets/923df048-6edf-48aa-872b-ede76bfd9ebd" />
</p>
<p>
On the admin panel, next to "Dashboard" click "Settings". Next to "Agents" click "Users". Under "Authentication Settings" make sure "Registration Required" is unchecked. 
</p>
<br />

<p>
<img width="1440" alt="Screenshot 2025-05-12 at 2 43 28 PM" src="https://github.com/user-attachments/assets/1e8c2294-133f-4f1f-8a17-ceffee1c0db2" />
</p>
<p>
On the admin panel, next to "Emails" click on "Agents". On the right, click "Add New Agent". Fill out the info of the agent you would like to add (their name, email, phone number and a username they will use to log into their osTicket account. To set their password, click "Set Password" and uncheck the box. Type the password you would like to use. Uncheck the box at the bottom and then click "Update"). Under "Access" select the department they will be in and the role they will have. Under "Permissions" check the boxes of the permissions you want the agent to have. Under 'Teams" select the team that they will be apart of. Once finished filling all of this out, click "Create". Do this for all the agents you would like to add. 
</p>
<br />

<p>
<img width="1110" alt="Screenshot 2025-05-12 at 2 45 52 PM" src="https://github.com/user-attachments/assets/1e337d72-4235-4d65-bb85-acdebf3fa820" />
</p>
<p>
On the admin panel, at the top right click "Agent Panel". Now, on the agent panel, next to "Dashboard" click "Users". On the right, click "Add User". Fill out the info of the user that would create a ticket. When finished, click "Add User". 
</p>
<br />

<p>
<img width="1171" alt="Screenshot 2025-05-12 at 2 49 01 PM" src="https://github.com/user-attachments/assets/53454f79-3970-4c38-927b-063e82ce2581" />
</p>
<p>
At the top right, click "Admin Panel". On the admin panel, next to "Settings" click "Manage". Next to "Filters" click on "SLA". On the right, click "Add New SLA Plan". Create three of these named: "Sev-A", "Sev-B" and "Sev-C". For "Sev_A", the "Grace Period" would be "1" hour and the "Schedule" would be "24/7". For "Sev-B", the "Grace Period" would be "4" hours and the "Schedule" would be "24/7". For "Sev-C", the "Grace Period" would be "8" hours and the "Schedule" would be "Monday-Friday 8am-tpm with U.S Holidays". 
</p>
<br />

<p>
<img width="1171" alt="Screenshot 2025-05-12 at 2 51 29 PM" src="https://github.com/user-attachments/assets/3c6e305f-56b1-4391-bab2-ece3f31293f5" />
</p>
<p>
On the admin panel, go to "Manage" and then "Help Topics". On the right, click "Add New Help Topic". When you or a user are creating a ticket, this will be the category of the issue. You can create the categrories you would like for example: "Personal Computer Issues, Password Reset, etc...". Fill out the info apparent to you. "Topic" is what you would like to name the category and "Parent Topic" is what you specifically need for the issue. When finished, click "Add Topic". 
