---
tags: [CompTia,SecPlus,CyberSec,Certs]
#aliases:
#cssclass:
#publish:
---

# About
---
- [[#Network Intrusion Detection System (NIDS)]] used to detect only ^763e90
- [[#Network Intrusion Prevention System (NIPS)]] used to prevent
	- In addition to functions on [[#Network Intrusion Detection System (NIDS)]]
- See also [[IDS]] and [[IDS#HIDS|HIDS]], and [[Endpoint Analysis#HIDS/HIPS|HIDS/HIPS]]

```ad-info
title: IDS/IPS Inline
collapse:close
![[IDS-Inline1.png]]
```

# Network Intrusion Detection System (NIDS)
---
- Attempts to detect, log, and alert of malicious network activities ^675d49
- Such as port scans or #DDoS 
	- Behind [[Firewalls]] gives it less incoming traffic to analyze
- Runs in promiscuous mode
	- Sees all traffic crossing the network versus only the traffic meant for the device MAC address
	- Only if on mirrored ports in [[Switches]]
- <u>Can only detect, monitor, or alert</u> with heuristics or [[IDS#^646241|Signatures]]
- <u>Passive</u>

# Network Intrusion Prevention System (NIPS)

## About
---
- Attempts to remove, detain, or redirect malicious traffic ^7ad297
- In addition to functions of NIDS
- Install "in-line" in network
- Tune correctly to avoid false positives and #DDoS
- <u>Active</u>

## Fail Open Or Shut?
---
- If a [[#Network Intrusion Prevention System (NIPS)]] device fails should it let all the traffic through or block all traffic?
- Shutting can lead to a #DDoS problem
- Most organizations choose to fail open and let other defensive measures take over

## Protocol Analyzer
---
- Allows an admin to analyze traffic and better troubleshoot or secure a network
	- Similar to programs such as Wireshark or network monitor
- In addition to [[#Network Intrusion Prevention System (NIPS)]] normal function it can act as a protocol analyzer
	- It has this in order to detect [[The OSI Model#Application|Application]] level traffic like http, ftp and telnet
- [[#Network Intrusion Prevention System (NIPS)]] will then pass this to the signature engine either on itself or a [[#Network Intrusion Detection System (NIDS)]] system
- Allows device to establish a baseline and then identify what abnormal is for its [[Endpoint Analysis#User and Entity Behavioral Analytics (UEBA)|behavioral]] or [[IDS#^ed7614|anomalous]] traffic functions
- Takes more processing power

# Objectives
---
- [[Objectives#3.3 - Given a scenario, implement secure network designs|3.3 - Given a scenario, implement secure network designs]]