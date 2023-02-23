---
tags: [CompTia,SecPlus,CyberSec,Certs]
#aliases:
#cssclass:
#publish:
---

# About
---
- Much less secure than wired networking since network traffic is broadcasted
- Don't need physical access
- See also
	- [[Securing Wireless Devices]]

# Common Vulnerabilities
---
- Weak admin credentials or defaults
- Remote administration
	- Allows you to access device over the internet to manage it
	- Should only manage locally
- Service Set Identifier (SSID)
	- Uniquely Identifies the network and is the name of the WAP used by the clients ^de74b1
	- <u>The exam encourages you to disable the SSID</u> but in reality it is not difficult for hackers to obtain since every packet sent wirelessly will have the network information

# Rouge Access Point

## About
---
- An unauthorized WAP or wireless router that allows access to the secure network ^58e171
- Someone could plug in a WAP or wireless router of their own into the wired network
- This would extend your wired network into the open since your internal network is no accessible over wireless
- This could also introduce additional issues like someone running their own DHCP service and causing conflicts

## Prevention
---
- [[Firewalls#MAC Filtering|MAC Filtering]]
- [[Network Access Control]]
- [[NIDS & NIPS]]

# Evil Twin

## About
---
- A rouge, counterfeit, and unauthorized WAP with the same SSID as your legitimate on ^e1ae28
- Devices look for SSID to connect and can't tell the difference between a real one and a fake one
- Can perform [[Hijacking#Man-in-the-Middle (MITM)|Man-in-the-Middle (MITM)]]

## Prevention
---
- Can't stop at the source unless you can find it and unplug it
- Have clients configured to use a VPN whenever on wifi even if on your wifi
- Avoid wifi all together if possible

# Objectives
---
- [[Objectives#1.4 - Given a scenario, analyze potential indicators associated with network attacks|1.4 - Given a scenario, analyze potential indicators associated with network attacks]]
- [[Objectives#3.4 - Given a scenario, install and configure wireless security settings|3.4 - Given a scenario, install and configure wireless security settings]]