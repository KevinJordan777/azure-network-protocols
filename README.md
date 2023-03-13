<p align="center">
<img src="https://i.imgur.com/Ua7udoS.png" alt="Traffic Examination"/>
</p>

<h1>Network Security Groups (NSGs) and Inspecting Traffic Between Azure Virtual Machines</h1>
In this tutorial, we observe various network traffic to and from Azure Virtual Machines with Wireshark as well as experiment with Network Security Groups. <br />




<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Various Command-Line Tools
- Various Network Protocols (SSH, RDH, DNS, HTTP/S, ICMP)
- Wireshark (Protocol Analyzer)

<h2>Operating Systems Used </h2>

- Windows 10 (21H2)
- Ubuntu Server 20.04

<h2>High-Level Steps</h2> 

Create 2 Virtual Machines inside of Azure. VM1 running Windows 10 (21H2) and VM2 runnig Ubuntu(Linux) Server 20.04 

Login to VM1 with Remote Desktop(RDP)

Download and install Wireshark to VM1. Then open wireshark and examine traffic coming from the ethernet connection.




<h2>Actions and Observations</h2>

<p>
<img src="https://i.imgur.com/vvKdlIw.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Create 2 Virtual Machines inside of Azure. VM1 running Windows 10 (21H2) and VM2 runnig Ubuntu(Linux) Server 20.04
</p>
<br />

<p>
<img src="https://i.imgur.com/nhET0WJ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Login to VM1 with Remote Desktop(RDP)
</p>
<br />

<p>
<img src="https://i.imgur.com/KqbRUVr.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Set the following permissions (share the folder) for the “Domain Users” group: Folder:
  
 Folder: “write-access”,  Group: “Domain Users”, Permissions: “Read/Write” 
  
  Normal domain users are granted permission to  read and write in the "write-acces" group.
</p>
<br />

<p>
<img src="https://i.imgur.com/vamyV36.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Set the following permissions (share the folder) for the “Domain Users” group:
  
 Folder: “no-access”, Group: “Domain Admins”, “Permissions: “Read/Write 
  
  Normal domain users are not granted permission to access the "no-access" group at all.
  
  Only Domain Admin are allowed permission to access the "no access" group.
   
</p>
<br />
