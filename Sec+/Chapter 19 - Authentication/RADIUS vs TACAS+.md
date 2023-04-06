---
tags: [CompTia,SecPlus,CyberSec,Certs]
#aliases:
#cssclass:
#publish:
---

# About
---
- Remote Authentication Dial-In User Service (RADIUS)
	- Provides centralized administration of dial-up, [[Virtual Private Network (VPN)|VPN]], and wireless [[Authentication]] services for [[802.1x]] and [[802.1x#Extensible Authentication Protocol (EAP)|EAP]] ^fcaf9c
	- A client server protocol running on the [[The OSI Model#Application|Application]] layer
	- Usually on a separate server but can also be on a #Windows server in a domain environment
	- Used to authenticate users, authorize their access, and account for their usage
		- Fulfills [[SecBasics#^45fffd|AAA Model]]
	- Uses UDP
	- Ports
		- Authentication - 1812
		- Accounting - 1813
		- Some Proprietary Authentication - 1645
		- Some Proprietary Accounting - 1646
	- Cross Platform compatible
	- Doesn't support
		- Remote Access Protocol, NetBIOS x.25 and some others
- Terminal access controller access control system + (TACAS+)
	- Proprietary #Cisco form of [[802.1x]] [[Authentication]] ^efe982
	- Uses TCP
	- Port - 49
	- Some additional security
	- Supports more network protocols

| Term   | Connections | Protocols | Ports     | Proprietary |
| ------ | ----------- | --------- | --------- | ----------- |
| RADIUS | UDP         | Limited   | 1812/1813 |             |
| TACAS+ | TCP         | Much more | 49        | X            |

# Objectives
---
- [[Objectives#3.4 - Given a scenario, install and configure wireless security settings|3.4 - Given a scenario, install and configure wireless security settings]]
- [[Objectives#3.8 - Given a scenario, implement authentication and authorization solutions|3.8 - Given a scenario, implement authentication and authorization solutions]]