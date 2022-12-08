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
3. Each system reacts or works on different [[IDS#Methods|Methods]]

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
- Both will use <u>signature based detection</u> with logging and monitoring
- Often use "File system Integrity Monitoring"
	- Checks that OS, driver, and application files have not been changed
- Is usually able to address the problem better than a network based [[IDS]]/[[IPS]] since it is directly on the machine
- See also [[IDS#HIDS|IDS]]

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
- A software agent that <u>collects system data and logs for analysis</u> by a monitoring system to provide early detection of threats
- More focus on <u>behavior and anomalies</u> than signatures
- Logs endpoints observables and indicators which then combines with an analysis
- "Early detection" of threats
- Not designed to stop execution but to provide currently running and historical visibility in a compromise
- Allows you to gather more information as a threat responder and enhance remediation

# UEBA
---
- A system that can provide <u>automated identification</u> of suspicious activity by user accounts and endpoints
- Focus is not on collecting data but on <u>the analysis of it</u>
- Establishing baseline knowledge and then monitoring for anything outside of the baseline
- With analytics as the primary function and large amount of data provided, they rely heavily on advanced computing techniques like #MachineLearning or #AI
- Flow
	1. Typical flow would be taking an unknown threat and placing it into a #Sandbox environment for analysis
	2. Heuristic model is generated base don what the system saw
	3. Passes it into its #MachineLearning  and #AI
	4. Based on their decision it will be determined as either a threat or safe

```ad-info
title: Microsoft Advanced Threat Analytics Example
collapse:close
![[MS-ATT.png]]
```

# Advanced Threat Protection (ATP)
---
- More crossover and <u>hybrid companies/products</u> emerging
	- EPP, EDR, UEBA all in one
- Other names
	- Advanced Endpoint Protection (AEP)
	- NextGen AV (NGAV)

# [[Objectives]]
---
- [[Objectives#3.1 - Given a scenario, implement secure protocols|3.1 - Given a scenario, implement secure protocols]]
- [[Objectives#3.3 - Given a scenario, implement secure network designs|3.3 - Given a scenario, implement secure network designs]]