<p align="center">
<img src="https://i.imgur.com/Ua7udoS.png" alt="Traffic Examination"/>
</p>

<h1>Inspecting Traffic Between Azure Virtual Machines and Network Security Groups (NSGs)</h1>
In this tutorial, we observe various network traffic to and from Azure Virtual Machines with Wireshark as well as experiment with Network Security Groups. <br />


<h2>Video Demonstration</h2>

- ### [YouTube: Azure Virtual Machines, Wireshark, and Network Security Groups](https://www.youtube.com)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Various Command-Line Tools
- Various Network Protocols (RDP, ICMP, SSH, DHCP, DNS)
- Wireshark (Protocol Analyzer)

<h2>Operating Systems Used </h2>

- Windows 10 (21H2)
- Ubuntu Server 20.04

<h2>High-Level Steps</h2>

- Create a resource group and Windows 10 and Ubuntu (Linux) Virtual Machines
- Remotely Login to Windows 10 Virtual Machine
- Download and Install Wireshark
- Observe RDP, ICMP, SSH, DHCP, and DNS Traffic

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
<h2>Download and Install Wireshark</h2>
<p>
Open web browser and search "download wireshark"
</p>
<p>
<img src="https://i.imgur.com/IaUWgMM.png"/>
</p>
<h2>Observe RDP, ICMP, SSH, DHCP, and DNS Traffic<h2>

<h2>RDP (Remote Desktop Protocol)<h2>
<p>
<img src="https://i.imgur.com/HuwguyK.png"/>
</p>
<h2>ICMP (Internet Control Message Protocol)<h2>
<p>
1. Use perpetual ping command to ping VM2 and observe VM2's replies
<p>
<img src="https://i.imgur.com/TCoLjJN.png"/>
</p>
<p>
2. Block ICMP traffic to VM2 by setting an inbound firewall rule in Azure Network Security Groups and observe results
<p>
<img src="https://i.imgur.com/HdQomj0.png"/>
</p>
<p>
<img src="https://i.imgur.com/MWo2nc7.png"/>
</p>
<h2>SSH (Secure Shell)<h2>
<p>
The username and password created for VM2 will be used in this exercise
<p>
<img src="https://i.imgur.com/m9gorqJ.png"/>
</p>
<h2>DHCP (Dynamic Host Configuration Protocol)<h2>
<p>
<img src="https://i.imgur.com/iVjJEFt.png"/>
</p>
<h2>DNS (Domain Name System)<h2>
<p>
<img src="https://i.imgur.com/ZpRW8AI.png"/>
</p>
