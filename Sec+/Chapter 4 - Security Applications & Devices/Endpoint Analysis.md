---
tags: [CompTia,SecPlus,CyberSec,Certs]
#aliases:
#cssclass:
#publish:
---

# About
---
- Endpoints
	- Any device that is used and connects to your network
	- Desktop, Laptop, Phone
	- Move to [[Vocab]]
- Analysis is used when conducting monitoring, logging, and analysis of an endpoint(s)
- The job
	1. Analysts use tools to identify behavioral anomalies
	2. Then Identify techniques used by the [[Malware]] such as [[Active Intercept & Privilege Escalation|Privilege Escalation]] and persistence on the host

# Endpoint Security Capabilities
---
1. Antivirus (AV)
2. [[IDS#HIDS|HIDS]]/[[HIPS]]
3. Endpoint Protection (EPP) Platforms
4. Endpoint Detection Response (EDR) Platforms
5. User and Entity Behavioral Analytics (UEBA) Platforms

# AntiVirus (AV)
---
- Software capable of detecting and removing [[Viruses]] and in most cases other types of [[Malware]]
- Sometimes also called "Antimalware"

# HIDS/HIPS
---
- A type of [[IDS]] or [[IPS]] that monitors a computer system for unexpected behavior or drastic changes to the systems state on an endpoint
- Both will use signature based detection with logging and monitoring
- Often use "File system Integrity Monitoring"
	- Checks that OS, driver, and application files have not been changed
- Is usually able to address the problem better than a network based [[IDS]]/[[IPS]] since it is directly on the machine
- See also [[IDS#HIDS]]

# EPP
---
- A software agent and monitoring system the performs multiple security tasks such as [[#AntiVirus (AV)]], [[#HIDS/HIPS]], #Fireall, [[Data Loss Prevention (DLP)]], and [[Disk Encryption|Encryption]]
- Gartner magic quadrant that  shows industry leaders

```ad-info
title: Gartner Magic quadrant
collapse:close
![[GartnerMagicQ.png]]
```

# EDR
---
- A software agent that collects system data and logs for analysis by a monitoring system to provide early detection of threats

# UEBA
---
-

# Objectives
---
- [[Objectives#3.1 - Given a scenario, implement secure protocols|3.1 - Given a scenario, implement secure protocols]]
- [[Objectives#3.3 - Given a scenario, implement secure network designs|3.3 - Given a scenario, implement secure network designs]]