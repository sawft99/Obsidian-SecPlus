---
tags: [CompTia,SecPlus,CyberSec,Certs]
#aliases:
#cssclass:
#publish:
---

# About
---
- Most PCs can use removeable media
	- [[Data Loss Prevention (DLP)#Data theft evolution|Data theft evolution]]
- Want to ensure [[SecBasics#CyberSecurity Models|Confidentiality]]
	- Apply [[Disk Encryption#^501400]]

# Encryption
---
- #Windows has #Bitlocker to go
	- Software encryption
- Hardware Encryption is also an option
	- Ironkey USB

# Removeable Media Controls
---
- Technical limitations placed on a system in regards to the utilization of USB storage devices and other removeable media can be accessed ^285fde
- Examples
	- Group policy disallowing read and/or write access to USB/CD drives
- Need to consider admin controls as well
	- Policy that guides technical specifications

# Network Attached Storage (NAS)
---
- Appliance full of hard drives that connects directly into the network
- Often uses a RAID
- High availability and #Uptime is important here
- Combine multiple NAS units to form a [[#Storage Area Network (SAN)]]

# Storage Area Network (SAN)
---
- Network designed specifically to perform block storage functions that may consist of multiple [[#Network Attached Storage (NAS)]] devices ^ed6df7

# Tips
---
- Use full [[Disk Encryption]]k]
-  [[SecBasics#^45fffd|AAA Model]]
	- Have proper authentication
		- Username and passwords
			- Unique to each person
	- Log access to devices
		- "Who accessed, downloaded, etc"

# Objectives
---
- [[Objectives#2.1 - Explain the importance of security concepts in an enterprise environment|2.1 - Explain the importance of security concepts in an enterprise environment]]
- [[Objectives#2.5 - Given a scenario, implement cybersecurity resilience|2.5 - Given a scenario, implement cybersecurity resilience]]
- [[Objectives#3.3 - Given a scenario, implement secure network designs|3.3 - Given a scenario, implement secure network designs]]