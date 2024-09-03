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
We install Green bone using the command "sudo apt install gvm -y":  <br/>
<img src="https://i.imgur.com/iTO6aBz.png" height="80%" width="80%" alt="Homelab setup & penetrating metasploitable Steps"/>
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
