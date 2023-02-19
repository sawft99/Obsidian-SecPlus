---
tags: [CompTia,SecPlus,CyberSec,Certs]
#aliases:
#cssclass:
#publish:
---

# About
---
- Hubs
	- Originally traffic would go into one port and out all other ports in what was called a "broadcast" ^a8e9c4
	- As networks got larger this caused many collisions
- Bridges
	- Evolution after hubs
	- Separate physical LAN to WAN into 2 logical networks or connect 2 logical networks ^841797
- Switches
	- The evolution of both Hubs and Bridges combined
	- Works at the [[The OSI Model#Data Link|Data Link]] layer
	- Every port is like a bridge and hub combined by connecting logical networks and being able to send traffic out of individual ports ^b00706
	- Intelligence use of MAC and only sending out traffic to the MAC in question
	- Improves overall security and reduces traffic

# Vulnerabilities

## MAC Flooding
---
- An attempt to <u>overwhelm the limited switch memory</u> set aside to store the MAC address for each port ^334c18
	- Content Addressable Memory (CAM Table)
- A flooded switch can begin to act like a hub and start broadcasting traffic on all ports

## MAC Spoofing

### About
---
- Occurs when an attacker masks their own MAC address to <u>pretend they have the MAC address of another</u> device ^0b472f
- Example
	- WIFI may use MAC filtering to prevent unknown device from connecting
	- Switch your MAC address to an allowed address and you could bypass an [[Routers#Access Control List (ACL)|Access Control List (ACL)]] like this
- Often combined with Address Resolution Protocol (ARP) Spoofing or [[ARP Poisoning]]
	- Relies on MAC addresses as a way to associate IP's to MAC and vice versa
- Appear as the destination the traffic is attempting to go to in order to trick other network devices
- See also
	- [[Spoofing]]
	- [[ARP Poisoning]]

### Prevention
---
- Limit number of static MAC address accepted
- Limit duration of time for ARP entry on hosts
- conduct ARP inspection
	- Keep track of which MAC is used with which IPs

## Physical Tampering

### About
---
- Occurs when an attacker attempts to gain physical access to a device ^56ec11
- <u>Often if you can physically access something you can control it</u>
- Switches may have a configured management port which would allow someone to plug in and begin configuring the switch
- Attackers could unplug Ethernet or power cables causing a [[Denial of Service (DoS)]]

### Prevention
---
- Locked in network rack, closet, or door

# Objectives
---
- [[Objectives#1.4 - Given a scenario, analyze potential indicators associated with network attacks|1.4 - Given a scenario, analyze potential indicators associated with network attacks]]
- [[Objectives#2.7 - Explain the importance of physical security controls|2.7 - Explain the importance of physical security controls]]
- [[Objectives#3.1 - Given a scenario, implement secure protocols|3.1 - Given a scenario, implement secure protocols]]