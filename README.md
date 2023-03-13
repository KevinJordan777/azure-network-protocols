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

Open Power Shell in VM1 the PING the private IP address for VM2 10.0.0.5

Access Network Security Gropus in Azure and block ICMP traffic in VM2 by adjusting the firewall and notice how the PING echo request is timed out.




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
<img src="https://i.imgur.com/o2dmlsu.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
</p>
<br />

<p>
<img src="https://i.imgur.com/DE4eNER.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

   
</p>
<br />

<p>
<img src="https://i.imgur.com/JKPWX93.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

  
 Download and install Wireshark to VM1. Then open wireshark and examine traffic coming from the ethernet connection.
   
</p>
<br />


<p>
<img src="https://i.imgur.com/4cHl1YK.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

   
</p>
<br />

<p>
<img src="https://i.imgur.com/9LByHfl.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

  
 Open Power Shell in VM1 then PING run a continous Ping to the private IP address for VM2 10.0.0.5 
   
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
