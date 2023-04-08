<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post Installation and configuration</h1>

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Post Installation Configuration Objectives</h2>

- Configure Roles, departments and teams in Admin Panel
- Allow anyone to create tickets in osTicket
- Configure agents and users
- configure SLA
- Configure help topics


<h2>Configuration Steps</h2>
<p>
<img src=https://i.imgur.com/A866phg.png/>

  
Roles are the permissions granted to Agents per Department that they have access to. Each Role has a set of permissions that can be assigned to agents given that Role in association with a Department they have access to. In this lab, I logged into the admin panel of os Ticket to configure roles. As per the picture, I added an "administration" role. I also, added permissions to this role. The picture below shows some of the permissions which were added.
  
  
  



<img src=https://i.imgur.com/EnMya60.png/>

<p>
<img src=https://i.imgur.com/AD17fNe.png/>
</p>
<p>
A new department called "System Administrator" were added to os Ticket. As per the picture, this is the top level department of the organization, it has its personalized email address.
</p>
<br />

<p>
<img src=https://i.imgur.com/87VHYvg.png/>
</p>
<p>
"Level II support" team was added. The settings were then configured.Teams allow you to pull Agents from different Departments and organize them to handle a specific issue or user via a Help Topic or Ticket Filter. This for the ticket to be resolve in a timely manner and with the best means possible.
</p>
<br />

<img src=https://i.imgur.com/M9rEHHZ.png/>

The picture above shows that "Registration Required: Require registration and login to create tickets" were unchecked. This enables any user to creat tickets in osTicket.

<img src=https://i.imgur.com/GTr1jnk.png/> 
<img src=https://i.imgur.com/w9r8OCi.png/>
<img src=https://i.imgur.com/Xsa1RsA.png/>

The picture above shows a new agent; Michael Peters with his credentials added. He has access to the system administrator department and he also a member of level II support team.Agents are given access to the help desk with the intent to respond and resolve the tickets.


<img src=https://i.imgur.com/X3J4bph.png/>

A new user called Aiden Mark was created. Users can create an account and log-in to create a ticket or check a ticket’s status.They are ticket owners of the tickets in the help desk.


<img src=https://i.imgur.com/Nqv3Spp.png/>

SLA Plans or Service Level Agreements, are unlimited in osTicket. The purpose of the SLA Plan is to provide a length of time in which the help desk Administrator expects tickets to be closed. Three SLA plans were created; SEV A (critical tickets that needs to be resolve as soon as possible), SEV B ( tickets with high priority that has a longer grace period that SEV A), SEV C (issues that could wait longer to be solved).



<img src=https://i.imgur.com/v6L0D2Z.png/>
Help topics allows for proper ticket assignment and prompted a response to solving those tickets. Three help topics were created in addition to the generated ones. They were also assigned a department. The image below shows an email created for the system administrator department  with a high priority and help topic assigned. Tickets can be automatically by emailing this address.

<img src=https://i.imgur.com/mCyNuY6.png/>
