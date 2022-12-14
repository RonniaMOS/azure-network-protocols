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

- Create Resources
- Observe ICMP Traffic
- Observe SSH Traffic)
- Observe DHCP Traffic
- Observe DNS Traffic
- Observe RDP Traffic

<h2>Actions and Observations</h2>

<p>
<img src="https://i.imgur.com/R21OQ1i.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
  1 A resource group and 2 virtual machines (Microsoft 10 and Linux) were created.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Within Windows 10 Virtual Machine, Wireshark was installed. In Wireshark ICMP traffic was flitered. The private IP address was retrieved of the Ubuntu VM and pinged from within the Windows 10 VM. Observed ping requests and replies within WireShark. From the Windows 10 VM,  PowerShell was opened and a public website (www.google.com) was pinged. A perpetual/non-stop ping was initiated from Windows 10 VM Ubuntu VM.
Network Security Group was opened on Ubuntu VM. Incoming (inbound) ICMP traffic was disabled. In Windows 10 VM, observe the ICMP traffic in WireShark and the command line Ping activity. ICMP traffic was re-enabled for the Network Security Group on the Ubuntu VM. In Windows 10 VM, the ICMP traffic was observed in WireShark and the command line ping activity.

</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />
