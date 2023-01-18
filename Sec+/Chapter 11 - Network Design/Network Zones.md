---
tags: [CompTia,SecPlus,CyberSec,Certs]
#aliases:
#cssclass:
#publish:
---

# About
---
- Consider breaking network into multiple zones
- Can be further sub zoned with [[Routers#Access Control List (ACL)|Access Control List (ACL)]], subnets, [[Firewalls]], and other isolation methods
- Usually segmented into [[#LAN]], [[#WAN]], and [[#DMZ]] zones

```ad-example
title: Network Zones
collapse:close
![[NetworkZones1.png]]
```

# LAN
---
- Local Area Network
- Use Private IP
- Antimalware
- Behind [[Routers]] with [[Routers#Access Control List (ACL)|ACL]]

# WAN
---
- Wide Area Network
- Internet connection
- Monitor and firewall
- Use VPN to keep [[SecBasics#^51b6d8|Confidentiality]] of data going across WAN/Internet
	- HTTPS with TLS is a form of a VPN

# DMZ
---
- De-Militarized Zone
- A segmented zone isolated from the rest of a private network by one or more [[Firewalls]] that accepts connections from the internet over designated ports ^741e54
- Focused on providing controlled access to publicly available servers that are hosted within your organizations network
- Self hosted email, webservers, [[Proxy Servers]], RDP
- Created with multiple interfaces on [[Firewalls]]
- Each server has its own IP
- Traffic between [[#LAN]] and [[#DMZ]] passes through [[Firewalls]] and potentially an [[IDS]]

# Extranet
---
- A form of a [[#DMZ]] that is created for partner organizations to access over a [[#WAN]] ^eebd81
- Not publicly accessible
- Monitored heavily

# Intranet
---
- Expanded internal network across multiple areas such as with a VPN ^1b848e

# Objectives
---
- [[Objectives#3.3 - Given a scenario, implement secure network designs|3.3 - Given a scenario, implement secure network designs]]