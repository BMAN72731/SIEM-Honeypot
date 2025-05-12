# SIEM-Honeypot

## Objective

This Honeypot SIEM project was designed to grow my understanding of attackers patterns and locations around the world. By simulating these attacks on a cloud virtual machine, I was able to analyze logs from real world scenarios in a controlled manner to better understand SIEM's (Microsoft Sentinel) and how to track real adversaries.

### Skills Learned
[Bullet Points - Remove this afterwards]

- Constructing a SIEM
- Interpreting network and windows event viewer logs
- Interpreting attack patterns and location of adversaries
- Broadened knowledge of protocols, ports, and security vulnerabilities
- Basic understanding of KQL

### Tools Used
[Bullet Points - Remove this afterwards]

- Microsoft Sentinel
- KQL
- Azure virtual machine

## Steps

I began this project by setting up a basic resource group in azure to host all the tools necessary to deploy this SIEM. Once the foundation was setup, I deployed a low resource virtual machine in the resource group and began running it after receiving a set IP address from the virtual network. This VM will act as the honeypot to attract attackers all around the world. 

<img src="images/RG-SOC-Lab1.PNG" alt="Resource Group Overview">
(Finished azure foundation hosted in the resource group)
<p style="margin-top: 30px;"></p>


Now that the basics are setup, it is necessary to begin opening up defenses to allow attackers to start attempting to breach the defenses of this machine. To accomplish this, I set the security group connected to the virtual machine to allow all inbound connections on all ports. The next step is to log back onto the virtual machine and disable all firewalls locally. Both of these actions will make the machine extremely attractive to adversaries.

<img src="images/Sec rules.PNG" alt="Resource Group Overview">
