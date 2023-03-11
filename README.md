<p align="center">
<img src="https://i.imgur.com/Ua7udoS.png" alt="Traffic Examination"/>
</p>

<h1>Network Security Groups (NSGs) and Inspecting Traffic Between Azure Virtual Machines</h1>
In this tutorial, we observe various network traffic to and from Azure Virtual Machines with Wireshark as well as experiment with Network Security Groups. <br />


<h2>Video Demonstration</h2>

- ### [YouTube: Azure Virtual Machines, Wireshark, and Network Security Groups](https://www.youtube.com)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Various Command-Line Tools
- Various Network Protocols (SSH, RDP, DNS, HTTP/S, ICMP)
- Wireshark (Protocol Analyzer)

<h2>Operating Systems Used </h2>

- Windows 10 (21H2)
- Ubuntu Server 20.04

<h2>High-Level Steps</h2>

- Create a resource group and Windows 10 and Ubuntu (Linux) Virtual Machines
- Remotely Login to Windows 10 Virtual Machine
- Download and Install Wireshark and Open Command Prompt
- Observe traffic on ICMP, SSH, DHCP, DNS, RDP

<h2>Actions and Observations</h2>
<h2>Create a resource group and Windows 10 and Ubuntu (Linux) Virtual Machines</h2>
<p>
1. Create a resource group in Microsoft Azure
</p>
<p>
<img src="https://i.imgur.com/Iq1UNZP.png"/>
</p>
<p>
2. Create two virtual machines under the resource group
</p>
<p>
 -Give virtual machine 1 (VM1) a Windows 10 (21H2) OS and virtual machine 2 (VM2) an Ubuntu Server 20.04 OS 
</p>
<p>
 -Make the region of both virtual machines the same as our resource group's
</p>
<p>
 -Size of both virtual machines will be Standard_E2s_v3-2vcpus, 16 GiB memory
</p>
<p>
 -Create a username and password for each virtual machine (We will use these to login to our virual machines.)
<p>
<img src="https://i.imgur.com/mLztC45.png"/>
</p>
<p>
<img src="https://i.imgur.com/gylLFsp.png"/>
</p>
<h2>Remotely Login to Windows 10 Virtual Machine</h2>
<p>
1. Connect to VM1 by using Remote Desktop Connection and VM1's public IP address
<p>
<img src="https://i.imgur.com/3u3xSsb.png"/>
</p>
</p>
2. Login to VM1 with username and password 
</p>
<p>
<img src="https://i.imgur.com/Z1UyG6g.png"/>
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

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />
