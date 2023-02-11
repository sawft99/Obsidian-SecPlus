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
		- [[#Ping Flood]]
		- [[#Smurf Attack]]
		- [[#Fraggle Attack]]
		- [[#UDP Flood]]
		- [[#SYN Flood]]
		- [[#XMAS Attack]]
	- [[#Ping of Death]]
	- [[#Teardrop Attack]]
	- [[#Permanent DoS]]
	- [[#Fork Bomb]]

# Flood Attacks

## About
---
- A type of DOS which attempts to send more packets to a single server or resource than they can handle
- Thousands of packets or more at once

## Ping Flood
---
- An attacker attempts to flood the server by sending too many ICMP echo request packets
- Common for organizations today to drop the packets so the attacker gets a timeout rather a rejection 

## Smurf Attack
---
- Attacker send a ping (ICMP) to a broadcast address with a forged source address matching the targeted server forcing other machines to reply to the broadcast and use up server resources
- The larger the subnet the more intense
- Attack can be amplified because of this and a server can receive up to 3x as much traffic than the attacker sent out
- Older attack generally not an issue with modern equipment

```ad-example
title: Smurf Attack
collapse:close
![[SmurfAttack1.png]]
```

## Fraggle Attack
---
- Attacker sends a UDP echo packet to a broadcast IP on port 7 (ECHO) and port 19 (CHARGEN) to flood a server with UDP packets
- Like [[#Smurf Attack]] but instead of an ICMP echo reply it uses a UDP echo
- Don't confuse with ICMP echo, this is the echo <u>protocol</u>
- Older attack generally not an issue with modern equipment
	- Ports often closed

```ad-example
title: Fraggle Attack
collapse:close

![[FraggleAttack1.png]]
```

## UDP Flood
---
- A variant of a [[#Fraggle Attack]] that uses different UDP ports
- Can be just about any other UDP port especially if it is one that a server is hosting something on

## SYN Flood
---
- A DOS attack where an attacker initiates multiple TCP sessions by forging the source IP but the 3 way TCP handshake never completes
- Can be prevented with
	- "Flood Guards"
		- Can be a feature built into [[Routers]] or a dedicated device
	- Configuring a server to timeout
		- 10, 15, 30 seconds
	- [[NIDS & NIPS]] and [[Endpoint Analysis#HIDS/HIPS|HIDS/HIPS]]

```ad-example
title: Normal TCP
collapse:close

![[NormalTCPEx1.png]]
```

```ad-example
title: SYN Flood
collapse:close

![[SYNFloodEx1.png]]
```

## XMAS Attack
---
- "Christmas" Attack
- A specialized network scan that sets the FIN, PSH, and URG flags in a TCP pack to 'on' and can cause a device to crash or reboot
- A non standard formatted packet
- Named this because in a protocol analyzer you can see all of these flags turned on making the analyzer "Light up like a Christmas tree"
- Most device today will discard because they don't know how to handle

```ad-example
title: Wireshark XMAS Attack
collapse:close
![[XMASEx1.png]]
![[XMASEx2.png]]
```

# Ping of Death
---
- An attack that sends an oversized and malformed packet to another computer or server causing it to crash
	- It would write to areas of memory like a [[Buffer Overflow]]
- Packet should not be bigger than 65,535 bytes (64k)
- Most devices today will discard
- One of the first types of DOS attacks

```ad-example
title: Ping of Death
collapse:close
![[PingOfDeathEx1.png]]
```

# Teardrop Attack
---
- Attack that breaks packets into IP fragments, modifies them with overlapping and oversized payloads, and sends them to a victim machine
- "Teardrops can eventually form a large puddle"
- Many small packets that can't be put back together properly because a system does not know how to handle it

```ad-example
title: Teardrop Attack
collapse:close

![[TearDropEx1.png]]
![[TearDropEx3.png]]
![[TearDropEx2.png]]
```

# Permanent DoS
---
- Attack which exploits a security flaw to germanely break a networking device by reflashing its firmware

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