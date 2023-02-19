---
tags: [CompTia,SecPlus,CyberSec,Certs]
#aliases:
#cssclass:
#publish:
---

# About
---
- Address Resolution Protocol (ARP)
	- [[Ports and Protocols|Protocol]] for mapping an IP address to a MAC address that is recognized in the local network ^a4d399
- ARP Poisoning
	- An attack that exploits the Ip to MAC address resolution in a network to steal, modify, or redirect frames within the local area network
- Attacker associates their MAC with another IP so that when the router goes to send to an IP it will instead send to the attacker rather than the legitimate client
- Allows an attacker to take over any session that would involve communications at the [[The OSI Model#Data Link|Data Link]] layer 
	- An attacker could set up a MITM by taking over a MAC and then passing data between data and rest of the network 
- See also
	- [[Switches#MAC Spoofing]]

# Prevention
---
- Proper [[VLAN]] segmentation
- DHCP Snooping 

# Objectives
---
- [[Objectives#1.4 - Given a scenario, analyze potential indicators associated with network attacks|1.4 - Given a scenario, analyze potential indicators associated with network attacks]]

# TODO (Delete when done)
---
- [ ] Added vocab
- [ ] Added and linked objectives in document
- [ ] Linked objectives back to document
- [ ] Linked any relevant backlinks to and from document