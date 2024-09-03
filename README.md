# Basic-Homelab
Homelab setup ,Exploiting and penetrating of Metasploitable 2

<h2>Description</h2>
Project consists of creating a Homelab , Adding greenbone a vulnerability scanner and exploiting and penetrating of metasploitable 2
<br />


<h2>Environments Used </h2>

- <b>Kali linux </b>
- <b>Metasploitable 2 </b> 

<h2>Program walk-through:</h2>

<p align="center">
Launch the metasploitable: <br/>
<img src="https://i.imgur.com/CpMtJaf.png" height="80%" width="80%" alt="Homelab setup & penetrating metasploitable Steps"/>
<br />
  <br />
Find ip Address using "ifconfig on our metasploitable " Command:  <br/>
<img src="https://i.imgur.com/As6Lquh.png" height="80%" width="80%" alt="Homelab setup & penetrating metasploitable Steps"/>
<br />
<br />
Launch Kali linux and check ip address to confirm its on same network as metasploitable2:  <br/>
<img src="https://i.imgur.com/DB72fsK.png" height="80%" width="80%" alt="Homelab setup & penetrating metasploitable Steps"/>
<br />
<br />
Scan our network to detect the metasploitable using the "nmap" command: <br/>
<img src="https://i.imgur.com/KSwn8Bc.png" height="80%" width="80%" alt="Homelab setup & penetrating metasploitable Steps"/>
<br />
<br /> We do a ping scan to determine which hosts are listening in the network using the "nmap -n" command
 <br/>
<img src="https://i.imgur.com/Ia71wsw.png" height="80%" width="80%" alt="Homelab setup & penetrating metasploitable Steps"/>
<br />
<br />
Do a "sudo apt update" to update all kali dependecies & Wait for process to complete (may take some time):  <br/>
<img src="https://i.imgur.com/1G4WJyf.png" height="80%" width="80%" alt="Homelab setup & penetrating metasploitable Steps"/>
<br />
<br />
We install Green bone using the command "sudo apt install gvm -y":  <br/>
<img src="https://i.imgur.com/iTO6aBz.png" height="80%" width="80%" alt="Homelab setup & penetrating metasploitable Steps"/>
<br />
  <br />
we install all the databases,create permissions, and install services for greenbone to work using the command "sudo gvm-setup":  <br/>
<img src="https://i.imgur.com/H5P6c5i.png" height="80%" width="80%" alt="Homelab setup & penetrating metasploitable Steps"/>
<br />
  <br />
We open up our web browser and go to the web address "http://127.0.0.1:9392" , accept risks . <br/>
<img src="https://i.imgur.com/XcHQoSl.png" height="80%" width="80%" alt="Homelab setup & penetrating metasploitable Steps"/>
  <img src="https://i.imgur.com/tDCBCWN.png" height="80%" width="80%" alt="Homelab setup & penetrating metasploitable Steps"/>
<br />
  <br />
We login using the default username "admin" and password.  <br/>
<img src="https://i.imgur.com/6ncxP9I.png" height="80%" width="80%" alt="Homelab setup & penetrating metasploitable Steps"/>
<br />
  <br />
To reset your password if you don't remember it use the command "sudo  runuser -u_gvm -- gvmd --user=admin --new-password="input new password here"  <br/>
<img src="https://i.imgur.com/a9ZiDbo.png" height="80%" width="80%" alt="Homelab setup & penetrating metasploitable Steps"/>
<br />
   <br />To start up OPENVAS by Greenbone use the command "sudo gvm-start"   <br/>
<img src="https://i.imgur.com/UmHRDbv.png" height="80%" width="80%" alt="Homelab setup & penetrating metasploitable Steps"/>
<br />
<br />
Observe the wiped disk:  <br/>
<img src="https://i.imgur.com/AeZkvFQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
