---
tags: [CompTia,SecPlus,CyberSec,Certs]
#aliases:
#cssclass:
#publish:
---

# About
---
- A software vulnerability that occurs when resulting outcome from an execution process is directly dependent on the order and timing of certain events, and those events fail to execute in the order and timing intended by the developer ^d9302d
- If you and an attacker are trying to do something at the same time and the attacker can get in before you. That is considered a race condition
- Found where multiple threads are attempting to write a variable or object at the same memory location at the same time

# Dereferencing/Null Pointer Dereferencing

## About
---
- A software vulnerability when code attempts to remove relationship between the pointer and the thing the pointer is pointing to in memory
- Hard for [[Endpoint Analysis#AntiVirus (AV)|AntiVirus (AV)]] to detect and mitigate
	- If you get in before the [[Endpoint Analysis#AntiVirus (AV)|AntiVirus (AV)]] can take hold it may not detect it

## Example
---
- Dirty Cow
	- "Copy on Write"
	- Affected Linux and Android OS
	- Targeted against the programing for the copy on write function used in the kernel memory management system
	- Turn read only mapping into writing mapping
		- Form of [[Active Intercept & Privilege Escalation|Privilege Escalation]]
	- Didn't leave any traces in logs

# Databases and File Systems

## About
---
- Usually comes in the form of a "Time of Check to Time of Use (TOCTTOU)
	-



# Objectives
---
- Obj

# TODO (Delete when done)
---
- [ ] Added vocab
- [ ] Added and linked objectives in document
- [ ] Linked objectives back to document
- [ ] Linked any relevant backlinks to and from document