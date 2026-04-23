# post-install-config
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

- Windows 11</b> (21H2)

<h2>Post-Install Configuration Objectives</h2>

- Configure Roles 
- Configure Departments
- Configure Teams
- Configure Agents 
- Configure Users
- Configure SLA
- Configure Help Topics


<h2>Configuration Steps</h2>

<p>
<<img width="801" height="665" alt="image" src="https://github.com/user-attachments/assets/1591d6ae-297c-4de0-8159-69ada5121436" />

<p>
Configure Roles (for grouping permissions)
Admin Panel -> Agents -> Roles
Supreme Admin

Configure Departments (Ticket Visibility, Help Desk vs SysAdmins, vs Networking)
Admin Panel -> Agents -> Departments
SysAdmins

Configure Teams
Admin Panel -> Agents -> Teams (Pull Agents from different Departments)
Online Banking

</p>
<br />

<p>
<img width="797" height="637" alt="image" src="https://github.com/user-attachments/assets/c2205c3e-3844-48d5-9113-e40e8253c671" />

</p>
<p>
Allow anyone to create tickets
Admin Panel -> Settings -> User Settings (UNCHECK: unregistered users can create tickets)
Registration Required: Require registration and login to create tickets 

Configure Agents (workers)
Admin Panel -> Agents -> Add New
Jane (Dept: SysAdmins)
John (Dept: Support)

Configure Users (customers)
Agent Panel -> Users -> Add New
Karen
Ken

</p>
<br />

<p>
<<img width="798" height="620" alt="image" src="https://github.com/user-attachments/assets/ac1aa84d-d08d-4738-9278-2105528725c1" />

</p>
<p>
Configure SLA
Admin Panel -> Manage -> SLA
Sev-A (Grace Period: 1 hour, Schedule: 24/7)
Sev-B (Grace Period: 4 hours, Schedule: 24/7)
Sev-C (Grace Period: 8 hours, Business Hours)

Configure Help Topics (For when users create a ticket)
Admin Panel -> Manage -> Help Topics
Business Critical Outage
Personal Computer Issues
Equipment Request
Password Reset
Other


