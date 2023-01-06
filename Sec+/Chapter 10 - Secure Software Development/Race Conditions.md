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
- Exploits against file systems and databases usually comes in the form of a "Time of Check to Time of Use" (TOCTTOU)
	- The potential vulnerability that occurs when there is a change between when an app checked a resource and when the app used the resource
	- Invalidate check already made

## Example
---
- Shopping app
- Leave items in cart
- Come back to later and check out
- If the shopping app doesn't check again to see the current prices or if the items are in stock this would be a TOCTTOU issue

## Prevention
---
1. Develop applications to not process things sequentially if possible
	1. Doing things in parallel vs step 1, then 2, then 3, etc
	2. Decreases the number of sequences and therefore less race condition possibilities
2. Impellent a locking mechanism to provide app with exclusive access
	1. A shopping app where the item is in your cart and it is locked in your cart for 5 minutes so other people can not order something out of stock
	2. A similar concept can be employed with a database or file share where you check the file out, change it, and then check back in thus preventing multiple people from editing at the same time and causing conflicts

# Objectives
---
- Obj

# TODO (Delete when done)
---
- [ ] Added vocab
- [ ] Added and linked objectives in document
- [ ] Linked objectives back to document
- [ ] Linked any relevant backlinks to and from document