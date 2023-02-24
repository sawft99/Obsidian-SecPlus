---
tags: [CompTia,SecPlus,CyberSec,Certs]
#aliases:
#cssclass:
#publish:
---

# About
---
- Placement and config matter
- Small office or homes rely on a single AP while larger organizations may rely on multiple in a single location
- See also
	- [[Securing Wireless Devices]]

# Heatmaps
---
- Visual way to demonstrate wireless signal strength in different areas ^7a863b
- Will show you the different frequencies, their strength, and its affects in di
- Accomplish by walking around an area with a specialized tool and software
- Also called a Wireless Site Survey
- Multi points use Extended Service Set (ESS) configuration
	- Provides a single wireless network that all access points are part of and broadcast

```ad-example
title: Single AP & Multi AP Heatmap
collapse:close
![[HeatMapEx1.png]]
![[HeatMapEx2.png]]
```

# Directional Antennas
---
- An AP that broadcasts in <u>all directions and dimensions is Omnidirectional</u>
	- Can be considered more dangerous since it is more accessible by all including attackers
- Alternatives include
	- Bidirectional
		- Radio goes in two directions
	- Unidirectional
		- Radio is focused in a single direction
- An attacker could positions themselves in something like a parking lot and attempt to break into the WIFI

# Frequency

## About
---
- 2.4 and 5 ghz frequency
- 2.4 can travel farther since it has a longer wavelength
- So 2.4 ghz is more likely to penetrate more material and reach farther

## Jamming
---
- <u>Intentional</u> [[Securing Network Media#Radio Frequency Interference (RFI)]|Radio Frequency Interference (RFI)]] targeting your wireless network to cause a [[Denial of Service (DoS)]] condition ^31a301

# AP Isolation
---
- Creates a network segment, like a [[VLAN]], for each client when it connects to prevent them from communicating with each other clients on the network ^5b10f8
- Can only talk to gateway or internet depending on [[Firewalls#Access Control List (ACL) Config & Rules|Access Control List (ACL) Config & Rules]]

## Additional Prevention
---
- Have focused WIFI
- Turn down power
- Many APs have built in security that can be configured
- Avoid WIFI all together if possible
- See also
	- [[Securing Wireless Devices]]
	- [[Securing WIFI Devices]]

# Objectives
---
- [[Objectives#1.4 - Given a scenario, analyze potential indicators associated with network attacks|1.4 - Given a scenario, analyze potential indicators associated with network attacks]]
- [[Objectives#3.4 - Given a scenario, install and configure wireless security settings|3.4 - Given a scenario, install and configure wireless security settings]]