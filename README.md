<h1>Active Directory Home Lab</h1>

 ### [YouTube Demonstration](https://youtu.be/7eJexJVCqJo)

<h2>Description</h2>
Using VirtualBox, I created this basic Lab environment that will have active directory and just a few networking services.
I am mainly using this lab for my own practice as I want to completely grasp the understanding of configuring and running a virtual lab, to manage Active directory and practice windows Networking in general.
<br />


<h2>What is needed for this Lab:</h2>

- <b>VirtualBox</b> 
- <b>Windows Server 2019 ISO</b>
- <b>Windows 10 ISO</b> 


<h2>Environment</h2>


<h2>Walk-through:</h2>

<p align="center">
Network Diagram: <br/>
<img src= "https://i.imgur.com/0QRNlHo.jpg" height="80%" width="80%" alt="Network Diagram"/>
<br />

<h2>Environment: VirtualBox</h2>
<p align="center">



<br />
I started by opening Virtual box and select new to create my 1st virtual machine.  <br/>
<img src="https://imgur.com/DlHnG5N.png" height="80%" width="80%" alt="VM Machines"/>
<br />
<p align="center">
<br />
These are the specs for the Domain Controller. <br/>
<img src="https://imgur.com/8EgDQWE.png" height="80%" width="80%" alt="Specs"/>
<br />
<br />
DC 1st Network adapter will be using NAT.  <br/>
<img src="https://imgur.com/gyboULH.png" height="80%" width="80%" alt="1st network adapter"/>
<br />
<p align="center">
<br />
DC 2nd Network adapter will be Internal.  <br/>
<img src="https://imgur.com/S91X7QH.png" height="80%" width="80%" alt="2nd network adapter"/>
<br />

<h2>Environment: Windows Server 2019</h2>
<p align="center">



<br />
Windows 2019 installation. <br/>
<img src="https://imgur.com/1KBFJdM.png" height="80%" width="80%" alt="W2019 install"/>
<br />
<p align="center">
<br />
Logged as Administrator.  <br/>
<img src="https://imgur.com/ipYRgJo.png" height="80%" width="80%" alt="Logged as Administrator."/>
<p align="center">
After log in I went to Network Connections to Identify my 2 adapters.<br/>
As you can observe this is my 1st adapter that is using NAT.<br/>
<img src="https://imgur.com/h15dUMJ.png" height="80%" width="80%" alt="1st adapter"/>
<p align="center">
This is my internal adapter.
I changed it's settings as you can observe in the picture.<br/>
<img src="https://imgur.com/9hsyuPO.png" height="80%" width="80%" alt="2nd adapter"/>
<p align="center">
Named them for better reference.  <br/>
<img src="https://imgur.com/fR5j1W0.png" height="80%" width="80%" alt="Naming adapters"/>
<p align="center">
Observe the wiped disk:  <br/>
<img src="https://i.imgur.com/AeZkvFQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<p align="center">
Observe the wiped disk:  <br/>
<img src="https://i.imgur.com/AeZkvFQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<p align="center">
Observe the wiped disk:  <br/>
<img src="https://i.imgur.com/AeZkvFQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<p align="center">
Observe the wiped disk:  <br/>
<img src="https://i.imgur.com/AeZkvFQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
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
