---
tags: [CompTia,SecPlus,CyberSec,Certs]
#aliases:
#cssclass:
#publish:
---

# About
---
- Stopping users from downloading, installing, and running software
- Able to centrally manage both [[#Whitelisting]] and [[#Blacklisting]]
	- Microsoft #ActiveDirectory and #GroupPolicy

# Whitelisting
---
- Only applications that are on the list are allowed to be run by the operating system while all other applications are blocked ^80ea87
	- "ACL rule w/ explicit allow"
- More secure
- Everything denied by default with specified apps being the only ones allowed to run
- More difficult to setup and manage
- Every time an update to an app is made you need to adjust your list

# Blacklisting
---
- Any application placed on the list will be prevented from running while all others will be allowed to run ^74bc0c
- Less secure
- Every new version of a program or [[Malware]] evolution would need to be explicitly denied

# [[Objectives]]
---
- [[Objectives#3.2 - Given a scenario, implement host or application security solutions|3.2 - Given a scenario, implement host or application security solutions]]
- [[Objectives#4.4 - Given an incident, apply mitigation techniques or controls to secure an environment|4.4 - Given an incident, apply mitigation techniques or controls to secure an environment]]

# TODO (Delete when done)
---
- [ ] Added vocab
- [ ] Added and linked objectives in document
- [ ] Linked objectives back to document
- [ ] Linked any relevant backlinks to and from document