---
tags: [CompTia,SecPlus,CyberSec,Certs]
#aliases:
#cssclass:
#publish:
---

# About
---
- A protocol enabling different appliances and software applications to transmit logs or event records to a [[Logging#Syslog Server|Syslog Server]] ^037c11
- Standard for [[Logging]] across various systems and software
- Most major operating systems and network appliances support and use it
- Can be used to refer to the [[Ports and Protocols#^fc134a|Protocols]] , the [[Logging#Syslog Server|Syslog Server]], the log entries themselves, or a combination

```ad-example
title: PFSense Console for Syslog
collapse:close
![[PFSenseSyslogEx1.png]]
```

# Contents

## PRI Code
---
- Calculated based on facility and severity
- "Priority Code"

## Header
---
- Contains the timestamp and the hostname from where the event originated
- Ideally in UTC since it is standardized
- [[SIEM]] appliance may do it for you

## Message Portion
---
- The source process of the event and related content
- What actually happened

# Drawbacks
---
- Relying on UDP causes delivery issues in congested or unstable networks
- Very few security controls such as [[Disk Encryption#^501400|Encryption]] or [[Authentication]]

# Newer Syslog
---
- Uses port 1468 over <u>TCP</u>
- Uses <u>TLS</u> for enc sent to servers
- Use <u>MD5 or SHA1</u> #Hashing  for [[Authentication]] and [[SecBasics#^48ae1d|Integrity]] checks
- Some newer ones can also use message filtering, automated log analysis, event response scripting, and alternative message formats
- Newer versions called
	- syslog-ng (Next Generation)
	- rsyslog
		- Adds buffered operation and Reliable Event Logging Protocol (RELP) support

# Objectives
---
- [[Objectives#1.7 - Summarize the techniques used in security assessments|1.7 - Summarize the techniques used in security assessments]]
- [[Objectives#4.3 - Given an incident, utilize appropriate data sources to support an investigation|4.3 - Given an incident, utilize appropriate data sources to support an investigation]]