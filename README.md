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
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />


<p>
<img src="https://i.imgur.com/bQVNyYc.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />


<p>
<img src="https://i.imgur.com/sXPEmjw.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />


<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />
