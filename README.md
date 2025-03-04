<p align="center">
<img src="https://i.imgur.com/pU5A58S.png" alt="Microsoft Active Directory Logo"/>
</p>

<h1>On-premises Active Directory Deployed in the Cloud (Azure)</h1>
These are the steps I did that outline the implementation of on-premises Active Directory within Azure Virtual Machines.<br />




<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Active Directory Domain Services
- PowerShell

<h2>Operating Systems Used </h2>

- Windows Server 2022
- Windows 10 (21H2)

<h2>High-Level Deployment and Configuration Steps</h2>

 Step 1: Install Windows Server & Add Roles
Install Windows Server on the machine.
Open Server Manager and add the Active Directory Domain Services (AD DS) role.

Step 2: Promote to Domain Controller
Run the Active Directory Configuration Wizard to promote the server to a Domain Controller (DC).
Choose "Add a new forest" (if setting up a new domain) and set a domain name (e.g., example.com).

Step 3: Configure DNS & Users
Ensure the DNS role is installed (AD requires it).
Create Organizational Units (OUs), User Accounts, and Groups for management.

Step 4: Join Client Computers & Apply Policies
Connect client computers to the domain by adding them through System Properties.
Use Group Policy (GPO) to apply security settings and user policies.


