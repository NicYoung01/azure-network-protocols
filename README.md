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

- Created 2 Virtual Machines inside of Microsoft Azure
- Entered VM1 through Remote Desktop and downloaded / installed WireShark 
- Pinged VM2's private IP Address on VM1 to observe traffic
- Adjusted VM2's network security inside of Microsoft Azure to stop and allow pings coming through VM1

<h2>Actions and Observations</h2>

<p>
<img src="https://i.imgur.com/zS6VBSZ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Observing the traffic between virtual machines 1 and 2 by using Windows PowerShell or Command Prompt to ping virtual machine 2's private IP address.
</p>
<br />

<p>
<img src="https://i.imgur.com/9bY3qxT.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Inside Microsoft Azure, we changed the security rules to deny the pings coming through VM1.
</p>
<br />

<p>
<img src="https://i.imgur.com/FsjDCH8.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Back inside VM1, connection requests to VM2 started to time out until security allowed access again, resuming regular pings through IMCP protocol.
</p>
<br />
