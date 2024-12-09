<p align="center">
<img src="https://i.imgur.com/fME09po.png" alt="osTicket logo"/>
</p>

<h1>Joining a computer to a domain.</h1>
This tutorial demonstrates how to join a computer to a domain.<br />




<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
  

<h2>Operating Systems Used </h2>

- Windows 10 Pro</b> (21H2)

<h2>List of Prerequisites</h2>

- Windows Server 2022
- Installed Active Directory
  

<h2>Installation Steps</h2>

<p>
<img src="https://i.imgur.com/T1jb1Qa.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Within Azure portal,create a VM Windows 10 Pro with atleast 2 virtual CPUs,use the same Username and password you used when creating a Windows Server 2022 VM on the previous task.
</p>
<br />

<p>
<img src="https://i.imgur.com/INOdyPI.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
On your Windows server 2022 VM [DC-1], go to Networking and edit IP configuration,change Windows Server private IP address from DYNAMIC to STATIC.
</p>
<br />

<p>
<img src="https://i.imgur.com/XW4UloV.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
On your Windows 10 Pro VM,go to networking and DNS SERVER tab,change  DNS SERVER from "inherit from virtual network" to "custom" and use Windows Server 2022 private IP address,this IP address will now be a Windows 10 machine's DNS IP address.The VM will restart,log back in and go to CMD and type "ipconfig /all" and notice that the DNS IP address has changed.
</p>
<br />


<p>
<img src="https://i.imgur.com/iY7cUKY.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
On Windows 10 Pro VM,go to, "SYSTEM" then "RENAME THIS PC" tab and click change, enter your domain name then OK,enter username and password then OK, the VM will restart and you will log back in as "mydomain.com\username" 
</p>
<br />


<p>
<img src="https://i.imgur.com/bQVNyYc.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
On Windows Server machine,type "ACTIVE DIRECTORY USERS AND COMPUTERS", go to "COMPUTERS" and check if Windows 10 Pro machine is added successfully to a domain. 
</p>
<br />


<p>
<img src="https://i.imgur.com/sXPEmjw.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
On Windows 10 Pro VM, go to "SYSTEM", then "REMOTE DESKTOP" then "SELECT USERS THAT CAN REMOTELY ACCESS THIS PC" tab, click "ADD" type "DOMAIN USERS" then OK.This will now allow all domain users to access your Windows 10 Pro VM.  
</p>
<br />



