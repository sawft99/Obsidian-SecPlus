---
tags: [CompTia,SecPlus,CyberSec,Certs]
#aliases:
#cssclass:
#publish:
---

# About
---
- As an analyst this is a main part of the job
- Can be done manually or through automation
- Automated types include
	- [[#Signature Based]]
	- [[#Anomaly Based]]
	- [[#Behavioral Based]]
- See also
	- [[IDS]]
	- [[NIDS & NIPS]]

# Signature Based
---
- Network traffic is analyzed for predetermined attack patterns
- Least [[IDS#^70e651|False Positives]]
- See also
	- [[IDS#Methods]]

# Anomaly Based
---
![[IDS#^ed7614]]
- Some [[IDS#^70e651|False Positives]]
- See also
	- [[IDS#Methods]]

# Behavioral Based
---
- Activity is evaluated based on the previous behavior of applications, executables, and the operating system in comparison to the current activity of the system
- Can result in a number of [[IDS#^70e651|False Positives]] because there are a large number of applications and various ways they talk to each other
- See also
	- [[Endpoint Analysis#User and Entity Behavioral Analytics (UEBA)]]

# Hybrid
---
- Often in an [[IDS]] ,[[NIDS & NIPS]], or [[IDS#HIDS|HIDS]]

# Objectives
---
- [[Objectives#3.3 - Given a scenario, implement secure network designs|3.3 - Given a scenario, implement secure network designs]]