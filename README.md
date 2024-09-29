# <p align="center">
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

- Configure Roles (for grouping permissions)
- Configure Departments (Ticket Visibility, Help Desk vs SysAdmins, vs Networking)
- Configure Teams
- Configure Agents (workers)
- Configure Users (customers)
- Configure SLA
- Configure Help Topics (For when users create a ticket)


<h2>Configuration Steps</h2>
<p>
<img src="https://i.imgur.com/ChwWes6.png"
"/>
</p>
<p>
Logged into our Azure VM using Remote Desktop and logged into admin and local host users using different URLs (Step-1)
</p>
<br />

<p>
<img src="https://i.imgur.com/Ga7cxLc.png"

</p>
<p>
In the osTicket admin panel we opened up the Roles folder and clicked on view only (Step-2)
</p>
<br />

<p>
<img src="https://i.imgur.com/vaSMzqa.png" 
</p>
<p>
Clicked on Permissions and observed there was nothing checked under view only (Step-3)
</p>
<br />

<p>
<img src="https://i.imgur.com/kTuK2sw.png" 
</p>
<p>
Went to Expanded Access Roles and observed what was enabled and how it was different from view only (Step-4)
</p>
<br />

<p>
<img src="https://i.imgur.com/BbqrGGV.png"
</p>
<p>
Created a new role and named it Supreme Admin and enabled Permissions to do everything (Step-5)
</p>
<br />

<p>
<img src="https://i.imgur.com/Qw4tStK.png"
</p>
<p>
Under Agents-Departments we created a new top-level Department and named it SYsAdmins (Step-6)
</p>
<br />

<p>
<img src="https://i.imgur.com/HoZDbth.png"
</p>
<p>
Within Agents-Teams we created a new team and named it Online Banking (Step-7)
</p>
<br />

<p>
<img src="https://i.imgur.com/gpwqosH.png"
</p>
<p>
Under Agents-Agents we created a new (fake) user and set an email and password (Step-8)
</p>
<br />

<p>
<img src="https://i.imgur.com/QP21PaY.png"
</p>
<p>
Gave Jane SupremeAdmin access (able to access everything) (Step-9)
</p>
<br />

<p>
<img src="https://i.imgur.com/cCfac89.png"
</p>
<p>
Added Jane to the Online Banking Team and then created the Agent (Step-10)
</p>
<br />

<p>
<img src="https://i.imgur.com/cCfac89.png"
</p>
<p>
Created an account for a John Doe and put him in the Support Department and gave him View Only Access(Step-11)
</p>
<br />

<p>
<img src="https://i.imgur.com/eR0TAXP.png"
</p>
<p>
Switched to the Agent Panel and added a new user and named it Karen (Step-12)
</p>
<br />

<p>
<img src="https://i.imgur.com/0Mmr1Gs.png"
</p>
<p>
Created another User (still in the Agent Panel) and named it Ken (Step-13)
</p>
<br />

<p>
<img src="https://i.imgur.com/eWpgJ5W.png"
</p>
<p>
Back in Admin Panel-Manage-SLA created a new plan named it Sev-A set grace period to 1 hour (Step-14)
</p>
<br />

<p>
<img src="https://i.imgur.com/k4GCqAD.png"
</p>
<p>
Added another plan named it Sev-B and set grace period to 4 hours 24-7 (Step-15)
</p>
<br />

<p>
<img src="https://i.imgur.com/cSM8HqH.png"
</p>
<p>
Created another plan named it Sev-C and set the grace period to 8 hours 24-5 (Buisness Hours) (Step-16)
</p>
<br />

<p>
<img src="https://i.imgur.com/ry33MMU.png"
</p>
<p>
Next we created a new help topic under manage-help topics and named it Buisness Critical Outage (Step-17)
</p>
<br />

<p>
<img src="https://i.imgur.com/X6yfKsf.png"
</p>
<p>
Lastly we configured 4 more help topics still while in the Admin Panel (Step-18)
</p>
