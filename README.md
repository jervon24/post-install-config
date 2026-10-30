<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket: Post-Installation Configuration</h1>

This project covers configuring osTicket after installation: setting up roles, departments, teams, agents, users, SLA plans, and help topics so the help desk is ready to receive and route tickets.

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)
- osTicket

<h2>Operating System Used</h2>

- Windows 10 (21H2)

<h2>Configuration Objectives</h2>

1. Configure roles
2. Create departments
3. Create teams
4. Allow anyone to create tickets
5. Configure agents and users
6. Configure SLA plans
7. Configure help topics

<h3>1. Configure Roles</h3>

<img src="https://i.imgur.com/A866phg.png" alt="Creating the Administration role"/>
<img src="https://i.imgur.com/EnMya60.png" alt="Permissions assigned to the Administration role"/>

A role defines what an agent can do within the departments they can access. In the Admin Panel, I created an **Administration** role and assigned its permissions (shown above). In production, roles should follow the principle of least privilege, giving each agent only the permissions their job requires.

<h3>2. Create Departments</h3>

<img src="https://i.imgur.com/AD17fNe.png" alt="System Administrator department settings"/>

I created a **System Administrator** department as the top-level department, with its own dedicated email address.

<h3>3. Create Teams</h3>

<img src="https://i.imgur.com/87VHYvg.png" alt="Level II Support team settings"/>

I created a **Level II Support** team and configured its settings. Teams group agents from different departments so escalated or specialized issues reach the right people, regardless of which department they sit in.

<h3>4. Allow Anyone to Create Tickets</h3>

<img src="https://i.imgur.com/M9rEHHZ.png" alt="Registration Required setting unchecked"/>

I unchecked **Registration Required: Require registration and login to create tickets**, so anyone can submit a ticket. This lowers the barrier for users, but in a real environment it's a trade-off: open submission can invite spam or abuse, so it's often paired with CAPTCHA or limited to internal networks.

<h3>5. Configure Agents and Users</h3>

<img src="https://i.imgur.com/GTr1jnk.png" alt="New agent account details"/>
<img src="https://i.imgur.com/w9r8OCi.png" alt="Agent department access"/>
<img src="https://i.imgur.com/Xsa1RsA.png" alt="Agent team membership"/>

**Agents** are help desk staff who respond to and resolve tickets. I created agent **Michael Peters**, gave him access to the System Administrator department, and added him to the Level II Support team.

<img src="https://i.imgur.com/X3J4bph.png" alt="New user account"/>

**Users** are the people who submit tickets and own them. I created user **Aiden Mark**, who can log in to create tickets and check their status.

<h3>6. Configure SLA Plans</h3>

<img src="https://i.imgur.com/Nqv3Spp.png" alt="SLA plans"/>

SLA (Service Level Agreement) plans set how long a ticket can stay open before it's considered overdue. I created three:

| SLA Plan | Use | Grace Period |
|---|---|---|
| SEV-A | Critical issues needing immediate resolution | `<X> hours` |
| SEV-B | High-priority issues | `<X> hours` |
| SEV-C | Issues that can wait | `<X> hours` |

<h3>7. Configure Help Topics</h3>

<img src="https://i.imgur.com/v6L0D2Z.png" alt="Help topics list"/>

Help topics categorize incoming tickets so they're routed to the right department automatically. In addition to the defaults, I created three topics, `<Topic 1>`, `<Topic 2>`, and `<Topic 3>`, each assigned to a department.

<img src="https://i.imgur.com/mCyNuY6.png" alt="System Administrator email with priority and help topic"/>

I also set up an email address for the System Administrator department with high priority and a help topic assigned. Emails sent to this address automatically become tickets.
