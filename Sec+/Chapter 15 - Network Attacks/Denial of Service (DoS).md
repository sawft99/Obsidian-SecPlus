---
tags: [CompTia,SecPlus,CyberSec,Certs]
#aliases:
#cssclass:
#publish:
---

# About
---
- Describes any type of attack which attempts to make a computer, server resource, or other network equipment unavailable
- Types/Methods
	- [[#Flood Attacks]]
	- [[#Ping of Death]]
	- [[#Teardrop Attack]]
	- [[#Permanent DoS]]
	- [[#Fork Bomb]]

# Flood Attacks

## About
---
- A type of DOS which attempts to send more packets to a single server or resource than they can handle
- Hundreds or thousands of packets

## Ping Flood
---
- An attacker attempts to flood the server by sending too many ICMP echo request packets
- Common for organizations today to drop the packets so the attacker gets a timeout rather a rejection 

## Smurf Attack
---
- Attacker send a ping to a broadcast address with a forged source address matching the targeted server forcing other machines to reply to the broadcast and use up server resources
- Attack can be amplified because of this
- The larger the subnet the more intense

```ad-example
title: Smurf Attack
collapse:close
![[SmurfAttack1.png]]
```

# Ping of Death
---
-

# Teardrop Attack
---
-

# Permanent DoS
---
-

# Fork Bomb
---
-
# Objectives
---
- [[Objectives#1.3 - Given a scenario, analyze potential indicators associated with application attacks|1.3 - Given a scenario, analyze potential indicators associated with application attacks]]

# TODO (Delete when done)
---
- [ ] Added vocab
- [ ] Added and linked objectives in document
- [ ] Linked objectives back to document
- [ ] Linked any relevant backlinks to and from document