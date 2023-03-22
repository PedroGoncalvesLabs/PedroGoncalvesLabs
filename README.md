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

<h2>Walk-through:</h2>

<p align="center">
Network Diagram: <br/>
<img src= "https://i.imgur.com/0QRNlHo.jpg" height="80%" width="80%" alt="Network Diagram"/>

<h2>Environment: VirtualBox</h2>

<p align="center">
I started by opening Virtual box and select new to create my 1st virtual machine.  <br/>
<img src="https://imgur.com/DlHnG5N.png" height="80%" width="80%" alt="VM Machines"/>
<br/>
 
<p align="center">
These are the specs for the Domain Controller. <br/>
<img src="https://imgur.com/8EgDQWE.png" height="80%" width="80%" alt="Specs"/>
<br/>
 
<p align="center">
DC 1st Network adapter will be using NAT.  <br/>
<img src="https://imgur.com/gyboULH.png" height="80%" width="80%" alt="1st network adapter"/>
<br/>
 
<p align="center">
DC 2nd Network adapter will be Internal.  <br/>
<img src="https://imgur.com/S91X7QH.png" height="80%" width="80%" alt="2nd network adapter"/>
<br/>

<h2>Environment: Windows Server 2019</h2>

<p align="center">
Windows 2019 installation. <br/>
<img src="https://imgur.com/1KBFJdM.png" height="80%" width="80%" alt="W2019 install"/>
<br/>

<p align="center">
Logged as Administrator.  <br/>
<img src="https://imgur.com/ipYRgJo.png" height="80%" width="80%" alt="Logged as Administrator."/>
<br/>
 
<p align="center">
After logging in, I accessed Network Connections to identify my two adapters.<br/>
As you can observe, this is the 1st adapter that will be doing Network Address Translation (NAT).<br/>
<img src="https://imgur.com/h15dUMJ.png" height="80%" width="80%" alt="1st adapter"/>
<br/>
 
<p align="center">
This one is my Internal adapter.
I changed it's settings as you can observe in the picture.<br/>
<img src="https://imgur.com/9hsyuPO.png" height="80%" width="80%" alt="2nd adapter"/>
<br/>
 
<p align="center"> 
Naming them for better reference.  <br/>
<img src="https://imgur.com/fR5j1W0.png" height="80%" width="80%" alt="Naming adapters"/>
<br/>
 
<p align="center">
Changing the PC name.  <br/>
<img src="https://imgur.com/eUPgavL.png" height="80%" width="80%" alt="Changed the pc name."/>
<br/>
 
<p align="center"> 
Installing Active Directory Domain Services.  <br/>
<img src="https://imgur.com/185bgaO.png" height="80%" width="80%" alt="Installed Active Directory Domain Services."/>
<br/>
 
<p align="center"> 
Initiated Post Deployment Configuration.  <br/>
<img src="https://imgur.com/T33CtKZ.png" height="80%" width="80%" alt="Post Deployment Configuration"/>
<br/>
 
<p align="center"> 
Selecting forest and naming the Domain Root. <br/>
<img src="https://imgur.com/FEny2cU.png" height="80%" width="80%" alt="Added my forest"/>
<br/>
 
<p align="center"> 
Observe here that NetBIOS assigned me a domain name based on my root domain name.   <br/>
<img src="https://imgur.com/ma1vWGk.png" height="80%" width="80%" alt="NetBIOS assigned my domain name"/>
<br/>
 
<p align="center">
After completing the installation, I can now log in to MYDOMAIN.  <br/>
<img src="https://imgur.com/IYH6fb2.png" height="80%" width="80%" alt="log in MYDOMAIN"/>
<br/>
 
<p align="center">
I created a new Organizational Unit for the Admins.  <br/>
<img src="https://imgur.com/JAAMgI2.png" height="80%" width="80%" alt="new Organizational Unit for the Admins"/>
<br/>
 
<p align="center">
In the same Organizational Unit, I created an account for an Admin.  <br/>
<img src="https://imgur.com/q655vsx.png" height="80%" width="80%" alt="own account to be used as an Admin"/>
<br/>
 
<p align="center"> 
Setting up this account as a "Domain Admins" member.  <br/>
<img src="https://imgur.com/agW9IEd.png" height="80%" width="80%" alt="User account as a Domain Admins member"/>
<br/>
 
<p align="center"> 
Switching to the new Account.  <br/>
<img src="https://imgur.com/tGtEGVQ.png" height="80%" width="80%" alt="new Account"/>
<br/>
 
<p align="center"> 
Initiated, Remote Access installation.  <br/>
<img src="https://imgur.com/pRvZ3Dc.png" height="80%" width="80%" alt="Remote Access installation"/>
<br/>
 
<p align="center">
Added Service Features.  <br/>
<img src="https://imgur.com/NdmCSyu.png" height="80%" width="80%" alt="Service Features"/>
<br/>
 
<p align="center">
Routing and Remote Access configuration.  <br/>
Network Address Translation (NAT) <br/>
<img src="https://imgur.com/lKik9ZQ.png" height="80%" width="80%" alt="Routing and Remote Access configuration"/>
<br/>
 
<p align="center"> 
Selecting my public interface.  <br/>
<img src="https://imgur.com/ul9NLu0.png" height="80%" width="80%" alt="public interface"/>
<br/>
 
<p align="center"> 
DHCP Installation.  <br/>
<img src="https://imgur.com/9RC5SZr.png" height="80%" width="80%" alt="DHCP Installation"/>
<br/>
 
<p align="center">
DHCP Settings:  <br/>
Defining the Router. <br/>
<img src="https://imgur.com/SwoeRVR.png" height="80%" width="80%" alt="Defining the Router."/>
<br/>
 
<p align="center">
DHCP Settings:  <br/>
Defining Adress Scope. <br/>
<img src="https://imgur.com/hnfvgjW.png" height="80%" width="80%" alt="Defining Adress Scope"/>
<br/>
 
<p align="center">
Defining first, last Address and Subnet Mask.  <br/>
<img src="https://imgur.com/TxAlDD9.png" height="80%" width="80%" alt="1st and last Address and Subnet Mask"/>
<br/>
 
<p align="center">
<img src="https://imgur.com/DzUNgFd.png" height="80%" width="80%" alt="DHCP Option for this scope."/>
<br/>
 
<p align="center">
Defining Default Gateway.  <br/>
<img src="https://imgur.com/EEwwoUA.png" height="80%" width="80%" alt="Defining Default Gateway."/>
<br/>
 
<p align="center">
Information confirmation.  <br/>
<img src="https://imgur.com/g9ooTdI.png" height="80%" width="80%" alt="Confirming information"/>
<br/>
 
<p align="center">
Observe the active Address Pool.  <br/>
<img src="https://imgur.com/u11eApb.png" height="80%" width="80%" alt="active Address Pool"/>
<br/>
 
<p align="center">
New User creation. To be used on Client windows 10 Virtual Machine.  <br/>
<img src="https://imgur.com/0xlyNce.png" height="80%" width="80%" alt="New User creation"/>
<br/>
 
<p align="center">
<h2>Environment: VirtualBox</h2>
<br/>

<p align="center">
 Client1 creation (Windows 10 Virtual Machine).  <br/>
<img src="https://imgur.com/7ryIekl.png" height="80%" width="80%" alt="Client1 creation"/>
<br/>
 
<p align="center"> 
This machine will be in the Internal Network.  <br/>
<img src="https://imgur.com/haFIuB0.png" height="80%" width="80%" alt="Network Adapter (Internal)"/>
<br/>
 

<h2>Environment: Windows 10</h2>

<p align="center">
Windows 10 Installation.  <br/>
<img src="https://imgur.com/5SO4TxV.png" height="80%" width="80%" alt="Install"/>
<p align="center">
<img src="https://imgur.com/kVQ8jld.png" height="80%" width="80%" alt="OS Sellection"/>
<br/>
 
<p align="center">
 Naming User.  <br/>
<img src="https://imgur.com/KMP4rp7.png" height="80%" width="80%" alt="Naming User"/>
<br/>
 
<p align="center"> 
After logging in. I open Command Prompt to test a few things.  <br/>
You can observe here how I automatically was assigned an IP address by the server, but this computer is still not recognised as a member of the Domain. <br/>
<img src="https://imgur.com/ZxMKytT.png" height="80%" width="80%" alt="CMD/not recognizes as Domain Computer"/>
<br/>
 
<p align="center"> 
Changing Computers Name and Joining the Domain.  <br/>
<img src="https://imgur.com/uJIE9hM.png" height="80%" width="80%" alt="Changing Computers Name and Joining the Domain"/>
<br/>
 
<p align="center">
After rebooting the computer, I can log in with my User account on MYDOMAIN.<br/>
<img src="https://imgur.com/GFc1EXB.png" height="80%" width="80%" alt="Login MYDOMAIN"/>
<br/>
 
<p align="center">
Network Connection, details.  <br/>
<img src="https://imgur.com/GWQQmfW.png" height="80%" width="80%" alt="Network Connection Details."/>
<br/>
 
<p align="center"> 
Member of the Domain, confirmation. <br/>
<img src="https://imgur.com/EsrRcWB.png" height="80%" width="80%" alt="Member of the Domain Confirmation"/>
<p align="center">
<br/>
 
<p align="center">
IP Configuration.  <br/>
<img src="https://imgur.com/axht8re.png" height="80%" width="80%" alt="IP Configuration"/>
<br/>
 
<p align="center"> 
Use of Ping to reach the Domain and Google website.  <br/>
<img src="https://imgur.com/18zYKAl.png" height="80%" width="80%" alt="Ping"/>
<p align="center">
At this point is safe to say that there is connectivity all the way to the Default Gateway. The Domain controller is properly NATing, forwarding me to the Internet and the ping properly comes back as an Echo Reply. 
 <br/>
 
 <h2>Environment: Server 2019</h2>

<p align="center"> 
Observe the IP leased to my "Client1" (Windows 10 Virtual Machine). <br/>
<img src="https://imgur.com/3se6TMD.png" height="80%" width="80%" alt="IP leased"/>
<p align="center">
<br/>

<p align="center"> 
You can observe here the Computers connected to the Domain. <br/>
<img src="https://imgur.com/1rVMYRH.png" height="80%" width="80%" alt="Computers connected to the Domain"/>
<p align="center">
<br/>

 
 
 <!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
