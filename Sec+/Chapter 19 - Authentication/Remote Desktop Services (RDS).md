---
tags: [CompTia,SecPlus,CyberSec,Certs]
#aliases:
#cssclass:
#publish:
---

# About
---
- Provides ability to remotely provide ability network and its resources ^b19041
- Accomplished with
	- [[#Remote Desktop Protocol (RDP)]]
	- [[#Virtual Network Computing (VNC)]]
- Should only use for internal network
	- Use [[Virtual Private Network (VPN)|VPN]] or SSH first to connect in securely and then use a form of RDS
- See also
	- [[Remote Access Services (RAS)]]
  
# Remote Desktop Protocol (RDP)
---
- #Microsoft proprietary protocol that allows administrators and users to remotely connect to another computer via a GUI ^eed942
- As if you are sitting right in front of computer
- RPD has [[Disk Encryption#^501400|Encryption]]  but not [[Authentication]]
	- Enable SSL or TLS for service authentication
- Port 3389

# Virtual Network Computing (VNC)
---
- Cross-platform version of the [[#Remote Desktop Protocol (RDP)]] for remote users to have GUI access ^f2a0f0
- NOT proprietary
- Need 
	- To create a VNC server on the machine you want to access
	- To setup the VNC client on the machine trying to connect
	- To setup the protocol and frame buffer to allow the server and client to communicate
- Port 5900

# Objectives
---
- [[Objectives#3.1 - Given a scenario, implement secure protocols|3.1 - Given a scenario, implement secure protocols]]