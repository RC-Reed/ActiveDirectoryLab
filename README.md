<h1>Active Directory Home Lab</h1>

<hr />

<h2>Description</h2>
<p>This project showcases my implementation of a fully functional Active Directory (AD) lab environment on my personal computer using VirtualBox. By following a structured process, I created a mini-enterprise network, including domain controllers, client machines, and essential network services.</p>

<hr />

<h2>Languages and Utilities Used</h2>
<ul>
  <li><b>PowerShell</b></li>
  <li><b>Oracle VirtualBox</b></li>
</ul>

<h2>Environments Used</h2>
<ul>
  <li><b>Windows 10 ISO</b></li>
  <li><b>Server 2019 ISO</b></li>
</ul>

<hr />

<h2>Key Components</h2>
<ul>
  <li><b>Configured a domain controller (DC)</b> running Active Directory Domain Services.</li>
  <li><b>Set up DHCP and DNS services</b> to manage network communication and automatic IP address assignment.</li>
  <li><b>Enabled NAT and routing</b> to allow internal network machines to access the internet.</li>
  <li><b>Automated the creation of 1,000 user accounts</b> in Active Directory using a custom PowerShell script.</li>
  <li><b>Deployed and joined a Windows 10 client machine</b> to the AD domain for testing and user authentication.</li>
</ul>

<hr />

<h2>Key Learnings</h2>
<ul>
  <li><b>Active Directory Fundamentals:</b> Setting up a domain, managing user accounts, and understanding organizational units (OUs).</li>
  <li><b>Networking Basics:</b> Configuring IP addressing, NAT, DHCP, and DNS. Designing and managing a private network.</li>
  <li><b>Automation with PowerShell:</b> Writing and debugging PowerShell scripts for bulk user account creation and directory management.</li>
  <li><b>Virtualization:</b> Using VirtualBox to create isolated virtual environments for lab simulations.</li>
</ul>

<hr />

<h2>Challenges Overcome</h2>
<ul>
  <li><b>Debugging DHCP configuration issues:</b> Ensured proper IP address assignment and default gateway settings.</li>
  <li><b>Troubleshooting NAT and routing:</b> Provided internet access to internal network clients.</li>
  <li><b>Optimizing virtual machine performance:</b> Allocated resources (CPU, RAM, network) efficiently to enhance performance.</li>
  <li><b>AD Web services was set to disabled by default which was breaking the user creation script but simply setting it to automatic and enabling it fixed the issue</li>
</ul>


<h2>Walk-Through:</h2>


<p align="center">
Environment architecture based on this Diagram Provided by Josh Madakor: <br/>
<img src="https://imgur.com/NXOYXXy.png" height="80%" width="80%" alt="Creating Domain COntroller"/>
<br />
<p align="center">
Creating Domain Controller: <br/>
<img src="https://imgur.com/szSIiwS.png" height="80%" width="80%" alt="Creating Domain COntroller"/>
<br />
<br />
Formatting Hard drive for the Domain Controller:  <br/>
<img src="https://imgur.com/JGI7WIN.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Giving Internal NIC an IP address: <br/>
<img src="https://imgur.com/ovcNAiL.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
Installing Active Directory Domain Services on VM: <br/>
<img src="https://imgur.com/MGWU8mK.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
AD Post-Deployment Config: <br/>
<img src="https://imgur.com/uSijODU.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
Creating Admin OU: <br/>
<img src="https://imgur.com/HVDjw5N.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
Creating Personal Admin Account: <br/>
<img src="https://imgur.com/d2h7zv5.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
Signing in with admin account: <br/>
<img src="https://imgur.com/sOE94Qf.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
Installing Remote Access on Domain Controller: <br/>
<img src="https://imgur.com/i6KRX6k.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
Installing NAT: <br/>
<img src="https://imgur.com/VqnbgHU.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
Installing DHCP Server: <br/>
<img src="https://imgur.com/cZ2N6U9.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
Configuring The DHCP Scope: <br/>
<img src="https://imgur.com/8Dzrd5f.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
Script to Generate 1000 Users in AD: <br/>
<img src="https://imgur.com/y5DJQmA.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
Script Working (Creating Users): <br/>
<img src="https://imgur.com/tz215hC.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
Users provisioned in Users Folder in AD: <br/>
<img src="https://imgur.com/Ebxw1Mv.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
Creating Client VM: <br/>
<img src="https://imgur.com/Cl4lCQm.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
DNS Server working (Pinging the Internet on Client VM): <br/>
<img src="https://imgur.com/uPf9Wba.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
Renaming Client VM and connecting it to the Domain Controler: <br/>
<img src="https://imgur.com/pjoDp9c.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />


