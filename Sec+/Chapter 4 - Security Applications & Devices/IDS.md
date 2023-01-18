---
tags: [CompTia,SecPlus,CyberSec,Certs]
#aliases:
#cssclass:
#publish:
---

# About
---
- <u>Intrusion Detection System</u>
- <u>Device or software</u> on system or network that <u>analyzes data going through it</u> ^a1d565
- Identify incident or attacks
- Host based ([[#HIDS]]) or network based ([[#NIDS]])
- Intrusion Prevention System (IPS)
	- An [[IDS]] with capabilities to also prevent [[Malware]] ^f81e57
- See also [[NIDS & NIPS]]

# HIDS
---
- <u>Host</u> Intrusion Detection System
- <u>Software</u> on computer or server
- Logs everything that it "thinks" is suspicious

```ad-example
title: HIDS (Snort)
collapse: close
![[HIDS_Snort.png]]
```

# NIDS
---
- <u>Network</u> Intrusion Detection System
- Hardware on network
- Traffic that goes through a [[Switches|switch]] that is mirrored to a NIDS
- See also [[NIDS & NIPS]]

```ad-info
title: NIDS
collapse: close
![[NIDS_Diagram.png]]
```

# Methods
---
- Signature ^646241
	- Specific <u>string of bytes</u> to trigger an alert
	- Continually searches for a known specific key
	- Any time it sees a pattern it is flagged
- Policy
	- <u>Specific declaration</u>
		- Filtering Port, IP, etc.
		- "No Telnet inbound/outbound"
- Anomaly ^ed7614
	- Analyzes the current traffic <u>against the established baseline</u> and triggers an alert if <u>outside the statistical average</u>
	- Full name "Statistical anomaly detection"
		- Also "Anomaly based detection" or "Statistical based detection"
	- Example
		- 9 - 5 work hours
		- Large downloads after hours
		- Gets flagged

# Alerts
---
- True Positive
	- Something <u>bad happened and system flagged</u> and/or alerted
- True Negative
	- Good and <u>normal happened and system didn't flag</u>
- False Positive
	- A legit or <u>normal operation was flagged improperly</u>
		- Such as opening up MS Word and setting off an alert
- False Negative
	- Something <u>bad happens but is identified as a legit</u> process
		- Getting [[Viruses]] but IDS does not go off

# Operations
---
- <u>ONLY alert and log</u>
- [[IDS#^f81e57|IPS]] actually prevents issues
- Host based systems will usually log only locally
	- Set up a Syslog server
	- If logs are kept only on the host an attacker could damage or alter the logs
	- Uploading to a central server helps prevent such an issue
- [[#HIDS]] logs are <u>used to recreate the events</u> after an attack has occurred


# Objectives
---
- [[Objectives#3.2 - Given a scenario, implement host or application security solutions|3.2 - Given a scenario, implement host or application security solutions]]
- [[Objectives#3.3 - Given a scenario, implement secure network designs|3.3 - Given a scenario, implement secure network designs]]