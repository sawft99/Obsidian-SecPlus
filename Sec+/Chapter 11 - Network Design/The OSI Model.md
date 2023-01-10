---
tags: [CompTia,SecPlus,CyberSec,Certs]
#aliases:
#cssclass:
#publish:
---

# About
---
- Open Systems Interconnection
- Used to explain network communications between a host and remote device over a LAN or WAN ^2ed6f4
- Categorizes different communication protocols
- Common Lexicon to describe network equipment

# Layers - Bottom to Top

## Physical
---
- Represents the actual cables and radio waves used to carry data over network
- Measure with "Bits"
	- Electrical signal or radio waves
- Examples
	- Cables Fiber, COAX
	- Radio waves
	- "Dumb devices" like repeaters

## Data Link
---
- Describes how a connection is established, maintained, and transferred over the physical layer and uses physical addressing (MAC Addresses0
- At this level Bits are grouped into Frames
- Examples
	- MAC Addresses
	- Switches
		- Use MAC Addresses to decide where to send a frame
	- Bridges/Hub
		- Earlier device before switches

## Network
---
- Uses logical address to route or switch information between hosts, the network, and the internetworks
- Routing and Switching
- Frames are grouped into packets
- Examples
	- IP Addresses
	- Layer 3 Switches which use MAC and IP to route
	- Routers

## Transport
---
- Manages and ensures transport of packets from host to destination with either TCP or UDP
- TCP
	- <u>Connection Oriented</u>
	- 3 way handshake
	- Packets grouped into <u>Segments</u>
- UDP
	- <u>Connectionless</u>
	- "Fire and Forget"
	- Packets grouped into <u>Datagrams</u>

## Session
---
- Manages the establishment, termination, and synchronization of a session over a network
- Creates a unique that allows data to find way from host to destination in a continual sequence

## Presentation
---
- Translates information into a format that the sender and receiver understand
- Example
	- Receiving a text you need to know if it is ASCII or UTF format
	- Picture files, encryption and more
- How will we understand and format the 1's and 0's in order to display it t the user

## Application
---
- Layer from which the message is created, formed, and originated
- High level protocols
- Examples
	- HTTP
	- SMTP
	- FTP
- Where user most interacts with a network

```ad-info
title: OSI Visual
collapse:close
![[OSIViz1.png]]
```

# Objectives
---
- [[Objectives#3.3 - Given a scenario, implement secure network designs|3.3 - Given a scenario, implement secure network designs]]
- [[Objectives#3.6 - Given a scenario, apply cybersecurity solutions to the cloud|3.6 - Given a scenario, apply cybersecurity solutions to the cloud]]