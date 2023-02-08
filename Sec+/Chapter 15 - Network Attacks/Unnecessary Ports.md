---
tags: [CompTia,SecPlus,CyberSec,Certs]
#aliases:
#cssclass:
#publish:
---

# About
---
- Any port that is associated with a service or function that is non essential to the operation of your computer or network ^dc0629
- You don't need [[Memorization of Ports|all ports]] available or open
- Example
	- A mail server only needs 25(SMTP),465/587(SMTP with SSL/TLS) to be listening
- Every open ports presents additional vulnerabilities

# Closing Ports
---
- Stop the relevant service on the machine
- Stop traffic with a [[Software Firewalls]] or [[Firewalls#Hardware Firewalls|Hardware Firewalls]]
	- Example
		- If you are no longer using a web server on port 80 be sure to disable or block it in the firewall when it is no longer needed
		- You likely needed to open the port in the first place so traffic can get through
- See also 
	- [[Network Address Translation]]
	- [[Network Address Translation#Port Address Translation (PAT)]]
	- [[Routers#Access Control List (ACL)]]
	- [[Firewalls#Access Control List (ACL) Config & Rules]]

```ad-example
title: Stopping Windows Services
collapse:close

![[Win_Service1.png]]
![[Win_Service2.png]]
![[Win_Service3.png]]
```

```ad-example
title: Stopping Linux Services 
collapse:close

![[Linux_Service1.png]]
![[Linux_Service2.png]]
```

```ad-example
title: Stopping OSX Services
collapse:close
![[OSX_Service1.png]]
![[OSX_Service2.png]]
![[OSX_Service3.png]]
![[OSX_Service4.png]]
![[OSX_Service5.png]]
![[OSX_Service6.png]]
```

# Objectives
---
- [[Objectives#1.6 - Explain the security concerns associated with various types of vulnerabilities|1.6 - Explain the security concerns associated with various types of vulnerabilities]]
- [[Objectives#3.2 - Given a scenario, implement host or application security solutions|3.2 - Given a scenario, implement host or application security solutions]]
- [[Objectives#3.3 - Given a scenario, implement secure network designs|3.3 - Given a scenario, implement secure network designs]]

# TODO (Delete when done)
---
- [x] Added vocab
- [x] Added and linked objectives in document
- [x] Linked objectives back to document
- [ ] Linked any relevant backlinks to and from document