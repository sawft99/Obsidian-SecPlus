---
tags: [CompTia,SecPlus,CyberSec,Certs]
#aliases:
#cssclass:
#publish:
---

# About
---
- Allow you to reconstruct events after an incident ^a9b138
- See also
	- [[Logging#Syslog Server]]

# Log File Maintenance
---
- Actions taken to ensure the proper creation and storage of a log file, such as the proper configuration, [[#Saving logs|saving]], backing up, securing, and [[#Protecting Logs|encrypting]] of the log files ^8a2b47

# Choosing
---
- Have to choose <u>what</u> you want to log and what you don't
	- The <u>size/scope</u> of the log collection
- The <u>amount of time</u> you want to store logs
	1. Archive to another storage space
	2. [[#Overwrite Events]] after certain amount of time

# Saving logs
---
- Don't save logs on the device that is being logged
- Log to a separate partition, hard drive, or external server
- Logging too much data without archiving or [[#Overwrite Events]] can cause the logs to fill up and use up available storage
	- <u>Crashing</u> of system can occur

# Overwrite Events
---
- When a maximum log size is reached, the system can begin overwriting the <u>oldest</u> events in the log files to make room ^2681e6
- Lose overwritten older data unless archived some other way
- Some highly regulated industries require you to keep logs for years

```ad-example
title: Windows Log Overwrite Option
collapse:close
![[WindowsLogEx1.png]]
```

# Write Once Read Many (WORM)
---
- Technology like a DVD-R that allows data to be written only once but read an unlimited number of times ^0831a7
- Can't be modified by someone such as [[SecBasics#Hackers|Hackers]]

# Protecting Logs
---
- Encrypt!

# Objectives
---
- [[Objectives#4.3 - Given an incident, utilize appropriate data sources to support an investigation|4.3 - Given an incident, utilize appropriate data sources to support an investigation]]