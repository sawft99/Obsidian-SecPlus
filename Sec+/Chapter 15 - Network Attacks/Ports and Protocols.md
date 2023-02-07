---
tags: [CompTia,SecPlus,CyberSec,Certs]
#aliases:
#cssclass:
#publish:
---

# About
---
- A logical communication endpoint that exists on a computer or server ^c22133
- Many common network attack occur because of open or unsecured ports
- See also [[Memorization of Ports]]

```ad-example
title: Inbound & Outbound Ports Example
collapse:close

![[PortEx1.png]]
```

# Port Types
---
- Inbound Ports
	- A port that is <u>listening</u> for a connection form a client ^7edb83
	- Example
		- Hosting a webserver on port 80
- Outbound Ports
	- A port created on a client to <u>call</u> out to a server that has an inbound port ^d8a5f2
	- Example
		- Trying to access a website on port 80, your computer picks a random high number port like 58254 to send traffic from

# Port Ranges
---
- All ports
	- 0 - 65,635
- Well known
	- 0 -1,023
	- Designated by IANA
	- Assigned to common protocols and ports
	- HTTP(80), HTTPS(443), FTP(21)
- Registered Ports
	- 1024 - 49,151
	- Assigned to proprietary ports
	- Vendors register with IANA
	- Microsoft SQL(1433), RDP(3389)
- Dynamic/Private Ports
	- 49,152 - 65,535
	- Can be used by any application
	- Don't need to register with IANA
	- Typical for client when picking a port for outbound communication
	- Gaming or IM

# Objectives
---
- [[Objectives#3.1 - Given a scenario, implement secure protocols|3.1 - Given a scenario, implement secure protocols]]

# TODO (Delete when done)
---
- [x] Added vocab
- [x] Added and linked objectives in document
- [ ] Linked objectives back to document
- [ ] Linked any relevant backlinks to and from document