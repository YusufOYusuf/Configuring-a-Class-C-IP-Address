<h1>Configuring a Class C IP Address</h1>



<h2>Description</h2>
In this lab, I learned to configure a Class C IP address. In a Class C network, the first two bits are set to 1, and the third bit is set to 0. That makes the first 24 bits of the address the network address and the remainder as the host address. There are over 2 million possible Class C networks. Example for a Classic C IP address is 192.168,178.1.
<br />



<h2>Environments Used </h2>

- <b>Windows Server 2016 Standard</b> 


<h2>Languages and Utilities</h2>

- <b>Windows Powershell<b>

<h2>Program walk-through:</h2>

<p align="center">
Right click the start Menu and open Network Connections: <br/>
<img src="https://i.postimg.cc/bvsn0jpk/Screen-Shot-2022-06-23-at-3-15-34-PM.png" height="80%" width="80%" alt="Creating a Subinterface on a Router and Assigning an IP Address Steps"/>
<br />
  
  
<br>
In the Network Connections window, double click the Ethernet 3 network adapter:<br>
<img src="https://i.postimg.cc/W4bBXXHM/Screen-Shot-2022-06-23-at-3-18-21-PM.png" height="80%" width="80%" alt="Creating a Subinterface on a Router and Assigning an IP Address Steps"/>
<br />
  
  
  
<br />
In the Ethernet 3 status dialog box, click Properties:</br>
<img src="https://i.postimg.cc/P5ZJdrX6/Screen-Shot-2022-06-23-at-3-19-53-PM.png" height="80%" width="80%" alt="Creating a Subinterface on a Router and Assigning an IP Address Steps"/>
<br />
  
  
  
<br />
In the Ethernet 3 Properties dialog box, under This connection uses the following items double click Internet Protocol Version 4(TCP/IPv4:  <br/>
<img src="https://i.postimg.cc/C5P7MsNV/Screen-Shot-2022-06-23-at-3-23-49-PM.png" height="80%" width="80%" alt="Creating a Subinterface on a Router and Assigning an IP Address Steps"/>
<br />


<br />
IN the Internet Protocol Cersion 4 (TCP/IPv4) Properties dialog box, select Use the following IP address and type in IP address,subnet mask,default gateway,preferred DNS server and alternate DNS Server:  <br/>
<img src="https://i.postimg.cc/RZrf7YqD/Screen-Shot-2022-06-23-at-3-26-28-PM.png" height="80%" width="80%" alt="Creating a Subinterface on a Router and Assigning an IP Address Steps"/>
<br />



<br />
Click start menu and open Windows powershell:  <br/>
<img src="https://i.postimg.cc/x1J5YZ4f/Screen-Shot-2022-06-23-at-3-31-44-PM.png" height="80%" width="80%" alt="Creating a Subinterface on a Router and Assigning an IP Address Steps"/>
<br />




<br />
In Windows Powershell window execute the following command to get the IP address of the Ethernet 3 network adapter: (Get-NetAdapter -Name "Ethernet 3" | Get-NetIPAddress).IPAddress:  <br/>
<img src="https://i.postimg.cc/gj3D8L3x/Screen-Shot-2022-06-23-at-3-37-07-PM.png" height="80%" width="80%" alt="Creating a Subinterface on a Router and Assigning an IP Address Steps"/>
<br />





<br />
You will observe the IP address 192.168.137.24:  <br/>
<img src="https://i.postimg.cc/BnCM6FCb/Screen-Shot-2022-06-23-at-3-39-39-PM.png" height="80%" width="80%" alt="Creating a Subinterface on a Router and Assigning an IP Address Steps"/>
<br />







</p>

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
