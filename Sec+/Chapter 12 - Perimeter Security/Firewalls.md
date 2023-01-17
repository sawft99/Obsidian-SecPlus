---
tags: [CompTia,SecPlus,CyberSec,Certs]
#aliases:
#cssclass:
#publish:
---

# About
---
- Screens traffic and protects one network from another ^3a1f24

# Types

## Hardware Firewalls
---
- Standalone physical device or appliance

## Software Firewalls
---
- Software running on a server or computer
- See also [[Software Firewalls]]

## Embedded Firewalls
---
- A single function on a multifunctional device
- Such as [[Routers]] and [[Unified Threat Management]] systems also including a firewall
- Common in SOHO networks 

# Packet Filtering

## About
---
- Firewall inspects each packet passing through the firewall and accepts or rejects it based on the rules
- Such as [[Routers#Access Control List (ACL)|Access Control List (ACL)]]
- Runs either as [[#Stateful]] or [[#Stateless]]

## Stateless
---
- Only analyzes traffic based on IP or ports and makes an 'accept' or 'deny' decision
- Uses [[Routers#Access Control List (ACL)|Access Control List (ACL)]]

## Stateful
---
- Tracks request that <u>LEAVE</u> through the firewall
- Temporarily open a high number port
- Can almost eliminate IP spoofing because each header received is being inspected
- Compares against what it was expecting based on the request that went out
- It then makes an 'accept' or 'deny' decision based on its [[Routers#Access Control List (ACL)|Access Control List (ACL)]]rules
- This makes it more in depth compared to [[#Stateless]]

# [[Network Address Translation]] (NAT) Filtering
---
- Filter traffic based on the ports being used and type of connection such as [[The OSI Model#Transport|UDP]] or [[The OSI Model#Transport|TCP]]
- Check endpoint connection by matching incoming traffic to requesting IP and port

# Application Layer Gateway
---
- 

# Objectives
---
- [[Objectives#3.3 - Given a scenario, implement secure network designs|3.3 - Given a scenario, implement secure network designs]]
- [[Objectives#4.4 - Given an incident, apply mitigation techniques or controls to secure an environment|4.4 - Given an incident, apply mitigation techniques or controls to secure an environment]]

# TODO (Delete when done)
---
- [ ] Added vocab
- [ ] Added and linked objectives in document
- [ ] Linked objectives back to document
- [ ] Linked any relevant backlinks to and from document