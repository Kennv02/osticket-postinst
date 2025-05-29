<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket.<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Post-Install Configuration Objectives</h2>

- Configure Roles
- Configure Departments
- Configure Teams
- Configure Agent
- Configure Users 
- Configure SLA
- Configure Help Topics 

<h2>Configuration Steps</h2>

<p>
<img src="https://github.com/user-attachments/assets/90e765ac-1f5d-4f15-8ef0-4210bad566b7"
</p>
<p>
<img src="https://github.com/user-attachments/assets/0041a682-43eb-4a12-90ba-d329b4e977d1"

</p>
<p>
Configuring roles is an essential part of the osticket system as it enables permissions for asssigning tickets,closing, editing, deleting, etc. 
You would want to open osticket and add a new role to which you can grant access to all functions as an admin. Go to:
  
- Admin Panel -> Agents -> Roles.
- Feel free to title your new role suited to personal preference and give admin role access to all of the functions as previuously mentioned. 

Following these steps would be useful for the tickets and tickets lifecycle overview.
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/148d3272-15c1-422c-ae94-113011cfad47"
</p>
<p>
For this next portion of the post installation process, we will create a new department through:
  
- Admin Panel -> Agents -> Departments
  
Name the Department as SysAdmin or however you prefer. The new department that is created will be used to direct new tickets to it. 

- Please note, we will add agents through the "access" section at a later step.
</p>
<br />

<p>
<imng src="https://github.com/user-attachments/assets/6d77488d-229d-4542-aac5-9e4da3049a8d"
</p>
<p>
<img src="https://github.com/user-attachments/assets/b0c39d82-4958-4766-bcfc-95aacb1d328b"
</p>
<p>
We will be creating a team in this next section. A team is essentially where we can pull agents from different departments to focus on a specific ticket issue. 
In this case, I created "Online Banking" as a team that will focus on online banking issues.

- I also ensured to allow anyone to create tickets without an account. Unregistered users can be given access by admins
- Admins can go to:
- Admin Panel -> Settings -> User Settings (**uncheck** unregistered users can create tickets)
</p>
<br />

<p> 
<img src="https://github.com/user-attachments/assets/82093dd7-8450-461c-a3b7-5f7867c528f5"
</p>
<p>
<img src="https://github.com/user-attachments/assets/cad903ac-74ab-45e7-b808-1bda44a23cf3"
</p>
<p>
To create an agent, go to:

- Admin Panel -> Agents -> Add New
- Names are subject to vary, I used Jane and Jon Doe for this example.
- Email address can be a superficial one. Make one up.
- In order to set an agent passworsd please **uncheck** send the agent password a reset email and you add a new password **uncheck** require password change at next login and click update. 
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/a1f0cd57-207a-4f71-b4d0-c801aac22a28"
</p>
<p>
<img src="https://github.com/user-attachments/assets/79e42be2-a6b5-4d0b-a04d-2bc71f04ce4e"
</p>
<p>
  
- I ensured to assign Jane or Joe in different teams as seen above which grants them access to certain tickets regardless of the deparment they were assigned to.
- They were also given acccess to selected departments. In this case, I assigned Jane to SysAdmin deparment and Jon is placed in Support department(not shown above).
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/b1f1efb7-b956-4faf-b494-09d1cb8f6a0c"
</p>
<p>

Creating users is essential to be able to create/submit tickets through osticket system and build an intuition of how the system operates from a user perspective.

- To create a user, go to:
- Agent Panel -> Users -> Add a user
- Add a superficial email address and a name. In this example, I went with Ken and ken@usmail.com
- Once the missing information is filled, click Add User.
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/56ea6185-ba8e-4aff-865f-557e5b38ea15" />

Configuring SLAs (Service Level Agreements) is an essential portion of the osticket support system as they allow the agent/admin to assess the severity of the ticket and how quickly they should be addressed 
- I configured three different SLA Plans.
- Sev-A (Grace Period: 1 hour, Schedule 24/7)
- Sev-B (Grace Period: 4 hours, Schedule 24/7)
- Sev-C (Grace Period: 8 hours, Schedule Business Hours 8am-5pm)
  
One example above as reference. To create new SLA Plan, go to:

- Admin Panel -> Manage -> SLA
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/c892727e-f49e-4280-b46d-8456782686cf" />

Configuring Help Topics will be the last portion of the post-installation configuration process. In short, Help Topics are categories that a user can choose from when creating as ticket.

I added the following Help Topics:

- Business Critical Outage
- Personal Computer Issues
- Equipment Request
- Password Reset
- Other

To Configure Help Topics, got to:

- Admin Panel -> Manage -> Help Topics 
</p>
  



</p>

