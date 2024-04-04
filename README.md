 <h1>Installing Kali Linux to Windows Using Virtual Box</h1>


<h2>Description</h2>
In this example, we will installing The Kali Linux Distro onto our Windows computer using Oracle VM Virtual Box
These are three main steps to get up an running. 


We will be using Nessus Essentials to scan local VMs hosted on VMWare Workstation in order run credentialed scans to discover vulnerabilities, remediate some of the vulnerabilities, then perform a rescan to verify remediation.
<br />


<h2>Utilities Used</h2>

- <b>Oracle VM Virtual Box</b> 

<h2>Environments Used </h2>

- <b>Kali Linux</b> (2024.1-amd64)
- 

<h2>Install Oracle VM Virtual Box to your system:</h2>

<p>
Create virtual machine instance in VMWare:  <br/>
<img src="https://i.imgur.com/GMU6LES.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Ensure connectivity by pinging the virtual machine with your local machine:  <br/>
<img src="https://i.imgur.com/n633l78.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />


<h2>Install Kali Linux Distrobution to the Virtual Machine:</h2>

Next-up:
Setup the virtual machine to be able to accept authenticated scans. Provide credentials to Nessus then rescan the virtual machine to compare results with the new scans compared to the one shown on the first scan.
<br />
<br />
<p>
In the Virtual Machine, enable remote registry (this will allow the scanner to connect to this Virtual Machine's registry and look for unsecure configurations):  <br/>
<img src="https://i.imgur.com/4UA2A8t.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
For the Advance Sharing Settings in the VM, make sure that the file and printer share is on:  <br/>
<img src="https://i.imgur.com/j01cO02.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />


<h2>Configure the settings of your Kali Linux VIrtual Machine:</h2>

Setup the virtual machine to be able to accept authenticated scans. Provide credentials to Nessus then rescan the virtual machine to compare results with the new scans compared to the one shown on the first scan.
<br />
<br />
<p>
In the Virtual Machine, enable remote registry (this will allow the scanner to connect to this Virtual Machine's registry and look for unsecure configurations):  <br/>
<img src="https://i.imgur.com/4UA2A8t.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
For the Advance Sharing Settings in the VM, make sure that the file and printer share is on:  <br/>
<img src="https://i.imgur.com/j01cO02.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />


<h2>Lessons Learned</h2>

- <b>The loop process of scanning and remediating to manage vulnerabilities</b>
- <b>A credential scan is will give us more feedback and alerts for us to dig into and remediate</b> 
<br />

<h2>Brush Up</h2>

- <b>Vulnerability Management on a large scale </b>
- <b>Touch up on CVSS scoring. </b>
- <b>Third Party Patching, Windows OS Patching that are setup, tested and deployed regularly (prevents going through and dealing with individual vulnerbilities that could be easily fixed by automated patching</b>
<br />

<h2>Shortcuts Learned</h2>

- <b>appwiz.cpl - Programs and features</b> 


<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>

