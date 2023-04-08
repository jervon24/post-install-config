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
</p>
<p>
I logged into the admin panel of os Ticket to configure roles. As per the picture, I added an "administration" role. I also, added permissions to this role. The picture below shows some of the permissions which were added.
  
  <img src=https://i.imgur.com/EnMya60.png/>
</p>
<br />

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
"Level II support" team was added. The settings were then configured.
</p>
<br />

<img src=https://i.imgur.com/M9rEHHZ.png/>

The picture above shows that "Registration Required: Require registration and login to create tickets" were unchecked. This enables any user to creat tickets in osTicket.

<img src=https://i.imgur.com/GTr1jnk.png/> 
<img src=https://i.imgur.com/w9r8OCi.png/>
<img src=https://i.imgur.com/Xsa1RsA.png/>

The picture above shows a new agent; Michael Peters with his credentials added. He has access to the system administrator department and he also a member of level II support team.
