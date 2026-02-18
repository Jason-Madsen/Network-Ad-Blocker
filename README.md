<h1>Network Level Ad Blocker</h1>

<h2>Description</h2>
Successfully transformed an HP Envy dv7 laptop into a dedicated Pi-hole DNS server running on Zorin OS. By configuring a static IP and integrating the server with an Arris G18 Gateway, I implemented a network-wide "sinkhole" that filters advertising and tracking telemetry for all connected devices, significantly improving network privacy and speed.
<br />


<h2>Languages and Utilities Used</h2>

- <b>Static IP Reservation</b> 
- <b>WAN DNS Configuration</b>
- <b>Bash Terminal</b>

<h2>Environments Used </h2>

- <b>Linux Zorin OS Lite</b>

<h2>Program walk-through:</h2>

<p align="center">
Pi-Hole Install / Status / IP Verification : <br/>
<img src="images/BashTerminal.png" height="80%" width="80%" alt="Bash terminal showing Pi-Hole install and configuration commands."/>
<br />
<br />
Static IP Configuration :  <br/>
<img src="images/Static IP Configuration.png" height="80%" width="80%" alt="Router Web Interface Static IP Configuration Page"/>
<br />
<br />
WAN DNS Configuration : <br/>
<img src="images/DNS Server Configuration.png" height="80%" width="80%" alt="Router Web Interface WAN Settings DNS Static Configuration"/>
<br />
<br />
Pi-Hole Ad-Blocker Dashboard :  <br/>
<img src="images/Pi-Hole Dashboard.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />

<h2>Challenges</h2>
While configuring the HP Envy dv7 challenges arose as I incorrectly saved teh dns server to the wrong address (182.168.0.122) This led to the entire network shutting down and I was unable to reconnect to my router from the app on my phone nor the ethernet cable into the wall. I had to plug the ethernet cable directly into the router so that I could access the Web Interface and reset the DNS configuration automatic. The difficulties here were that every time I needed to reset it, it needed to reboot. Unfortunately each time I rebooted, the connection timed out because it couldn't reconnect to the internet due to the misconfigured WAN DNS. Finally, I was able to reset the router by cutting the power to it and letting it reboot itself for a few minutes. I was then able to reset the WAN DNS configuration to automatic and I decided to test the DNS server through the HP Envy on my phone only. After successfully connecting I felt confident to reconfigure the WAN DNS to the HP Envy and was able to successfully connect on all devices.
<br />
<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
