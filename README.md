<h1>Setting up a SIEM in Azure</h1>

<h2>Description</h2>
In this project I designed, implemented, and managed a comprehensive Security Information and Event Management (SIEM) system from the ground up. I mainly used Microsoft Azure to do this. I created a Virtual Machine in the cloud which acted as my honeypot and made it super suseptible to the internet. After setting up Azure Sentinel, I began to log and monitor a number of attacks from different IP addresses from all over the world, these logs gave me attackers information which included not only their username and sourcehost, but also there longitude, latitude, and country. I then took that data and displayed it on a world map so I could see where all the attacks were coming from in real time.
<br />

<h2>Exposure:</h2>

- <b>Azure Portal</b>
- <b>Azure Sentinal</b>
- <b>Kusto Query Language</b>
- <b>Network Security Groups</b>

<h2>Program walk-through:</h2>

<p align="center">
Diagram overview of project: <br/>
<img src="https://i.imgur.com/8oAz7BK.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<p align="center">
Create Virtual Machine in Azure: <br/>
<img src="https://i.imgur.com/sMtxGQ5.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<p align="center">
Open up Firewall to make VM vulnerable to attacks: <br/>
<img src="https://i.imgur.com/W52DIi4.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<p align="center">
Create Log Analytics Workspace: <br/>
<img src="https://i.imgur.com/AwZPd0g.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<p align="center">
Enable gathering of VM logs in Security Centre: <br/>
<img src="https://i.imgur.com/Ttc1Hth.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<p align="center">
Connect Log Analytics Workspace to VM: <br/>
<img src="https://i.imgur.com/qb10UTv.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<p align="center">
Set up Azure Sentinel: <br/>
<img src="https://i.imgur.com/Psy9ZKF.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<p align="center">
Log in to VM with Remote Desktop: <br/>
<img src="https://i.imgur.com/aB3GUcm.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<p align="center">
Observe Event Viewer Logs in VM: <br/>
<img src="https://i.imgur.com/ZCrPNdD.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<p align="center">
Turn off Windows Firewall on VM: <br/>
<img src="https://i.imgur.com/wo4iMHy.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<p align="center">
Get Geolocation API Key: <br/>
<img src="https://i.imgur.com/coXuJVc.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<p align="center">
Run Script in Powershell ISE to get Geo Data from attackers: <br/>
<img src="https://i.imgur.com/EXhhsj3.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<p align="center">
Create Custom Log in Log Analytics Workspace to bring in our custom logs: <br/>
<img src="https://i.imgur.com/Afu2l77.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<p align="center">
Setup map in Azure Sentinel with Latitude and Longitude: <br/>
<img src="https://i.imgur.com/RGjM8K0.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<p align="center">
Configure World Map: <br/>
<img src="https://i.imgur.com/WAeBfIt.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<p align="center">
India and Italy join the attack: <br/>
<img src="https://i.imgur.com/iqaCckN.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<p align="center">


<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
