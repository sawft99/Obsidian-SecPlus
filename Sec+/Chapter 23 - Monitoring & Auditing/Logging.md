---
tags: [CompTia,SecPlus,CyberSec,Certs]
#aliases:
#cssclass:
#publish:
---

# About
---
- Data files that contain the accounting and [[Auditing]] trail for actions performed by a user on the computer or network
- #Linux log location
	- /var/log
- #Windows  [[#Log Types]]
	- [[#Security]]
	- [[#System]]
	- [[#Application]]

# Log Types

## Security
---
- Logs the events such as successful and unsuccessful logons to the system

## System
---
- Logs that have events such as a system shutdown or driver failure

## Application
---
- Log the events for the operating system and third party applications

# Windows Log Tools
---
- #Windows Event Viewer
	- On both workstation and server
	- Specialized events like DHCP, file replication, and other server roles will only be available on #Windows Server

# Syslog Server
---
- A server that uses standardized format for computer message logging that allows for the separation of the <u>software</u> that generates messages, the <u>system</u> that generates messages, and the software that <u>reports and analyzes</u> the messages ^25aaaa
- Allows you to consolidate all the logs into a single repository
- Use a [[Syslog]] client
- UDP port 514
- See also
	- [[Syslog]]

# Objectives
---
- [[Objectives#1.7 - Summarize the techniques used in security assessments|1.7 - Summarize the techniques used in security assessments]]
- [[Objectives#4.3 - Given an incident, utilize appropriate data sources to support an investigation|4.3 - Given an incident, utilize appropriate data sources to support an investigation]]
- [[Objectives#4.5 - Explain the key aspects of digital forensics|4.5 - Explain the key aspects of digital forensics]]