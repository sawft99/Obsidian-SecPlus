---
tags: [CompTia,SecPlus,CyberSec,Certs]
#aliases:
#cssclass:
#publish:
---

# About
---
- Analysis is used when conducting [[SecBasics#^45fffd|monitoring, logging]], and analysis of an endpoint(s)
- The job
	1. Analysts use tools to identify behavioral [[IDS#^ed7614|anomalies]]
	2. Then Identify techniques used by the [[Malware]] such as [[Active Intercept & Privilege Escalation|Privilege Escalation]] and persistence on the host
- Each system reacts or works on different [[IDS#Methods|Methods]]
- See also
	- [[Monitoring Types]]

# Endpoint
---
- Any device that is used and connects to your network ^69959c
- Desktop, Laptop, Phone

# Endpoint Security Capabilities
---
1. [[#AntiVirus (AV)]]
2. [[#HIDS/HIPS]]
3. [[#Endpoint Protection Platforms (EPP)]]
4. [[#Endpoint Detection Response (EDR)]]
5. [[#User and Entity Behavioral Analytics (UEBA)]]

# AntiVirus (AV)
---
- Software capable of detecting and removing [[Viruses]] and in most cases other types of [[Malware]] ^982ce4
- Sometimes also called "Antimalware"

# HIDS/HIPS
---
- Host Intrusion Detection System/Host Intrusion Prevention System ^84109b
- A type of [[IDS]] or [[IDS#^f81e57|IPS]] that [[SecBasics#^45fffd|monitors]] a computer system for unexpected behavior or drastic changes to the systems state on an endpoint
- Both will use <u>signature based detection</u> with [[SecBasics#^45fffd|Logging and Monitoring]]
- Often use <u>"File system Integrity Monitoring"</u>
	- Checks that OS, driver, and application files have not been changed
- Is usually able to address the problem better than a network based [[IDS]]/[[IDS#^f81e57|IPS]] since it is directly on the machine
- See also
	- [[IDS#HIDS]]

# Endpoint Protection Platforms (EPP)
---
- A software agent and [[SecBasics#^45fffd|Monitoring]] system the performs multiple security tasks such as [[#AntiVirus (AV)]], [[#HIDS/HIPS]], [[Software Firewalls]], [[Data Loss Prevention (DLP) - Appliance]], and [[Disk Encryption|Encryption]] ^fc7325
- Gartner magic quadrant that shows industry leaders

```ad-info
title: Gartner Magic quadrant
collapse:close
![[GartnerMagicQ.png]]
```

# Endpoint Detection Response (EDR)
---
- A software agent that <u>collects system data and logs for analysis</u> by a [[SecBasics#^45fffd|Monitoring]] system to provide early detection of threats ^46bc3d
- More focus on <u>behavior and anomalies</u> than signatures
	- [[IDS#^ed7614|Anomalies]]
- Logs endpoints observables and indicators which then combines with an analysis
- "Early detection" of threats
- Not designed to stop execution but to provide currently running and historical visibility in a compromise
- Allows you to gather more information as a threat responder and enhance remediation

# User and Entity Behavioral Analytics (UEBA)
---
- A system that can provide <u>automated identification</u> of suspicious activity by user accounts and endpoints ^2a3fce
- Focus is not on collecting data but on <u>the analysis of it</u>
- Establishing baseline knowledge and then [[SecBasics#^45fffd|Monitoring]] for anything outside of the baseline
- With analytics as the primary function and large amount of data provided, they rely heavily on advanced computing techniques like #MachineLearning or #AI
- Flow
	1. Typical flow would be taking an unknown threat and placing it into a #Sandbox environment for analysis
	2. Heuristic model is generated based on what the system saw
	3. Passes it into its #MachineLearning and #AI
	4. Based on their decision it will be determined as either a threat or safe
- See also
	- [[Monitoring Types#Behavioral Based]]

```ad-example
title: #Microsoft Advanced Threat Analytics Example
collapse:close
![[MS-ATT.png]]
```

# Advanced Threat Protection (ATP)
---
- More crossover and <u>hybrid companies/products</u> emerging ^befc27
	- [[#Endpoint Protection Platforms (EPP)]], [[#Endpoint Detection Response (EDR)]], [[#User and Entity Behavioral Analytics (UEBA)]] all in one
- Other names
	- Advanced Endpoint Protection (AEP)
	- NextGen AV (NGAV)

# Objectives
---
- [[Objectives#1.7 - Summarize the techniques used in security assessments|1.7 - Summarize the techniques used in security assessments]]
- [[Objectives#3.1 - Given a scenario, implement secure protocols|3.1 - Given a scenario, implement secure protocols]]
- [[Objectives#3.2 - Given a scenario, implement host or application security solutions|3.2 - Given a scenario, implement host or application security solutions]]
- [[Objectives#3.3 - Given a scenario, implement secure network designs|3.3 - Given a scenario, implement secure network designs]]