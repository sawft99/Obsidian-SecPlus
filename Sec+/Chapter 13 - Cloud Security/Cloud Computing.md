---
tags: [CompTia,SecPlus,CyberSec,Certs]
#aliases:
#cssclass:
#publish:
---

# About
---
- A way of offering on demand services that extend traditional capabilities of a computer or network ^3cf5c0
- Increases
	- [[SecBasics#^51b6d8|Availability]]
	- [[Virtualization#^a6ee8d|Elasticity]]
	- Resiliency
- Can bring additional security challenges

# Functioning
---
- Many cloud providers and services rely on [[Virtualization]] to gain efficiency and increase cost savings
- Reduce power, space, and cooling
- Achieves higher availability by firing up [[Virtualization#Virtual Machine Types|Virtual Machines]] when needed
	- Allows more dynamic use of server resources like CPU and RAM

# Hyperconvergence
---
- Fully integrates storage, network, and servers by having software and [[Virtualization]] manage these tasks ^eb058d
- Don't have to perform hardware changes
- Single interface and device to manage

# Virtual Desktop Infrastructure (VDI)
---
- A full desktop operating system for an end user to use from a centralized server ^a1b451
- Security benefits example
	- Can create a new [[Virtualization#Virtual Machine Types|Virtual Machine]] every time a user logs in
	- Even if exploited it is non persistent so every time a user logs off the [[Virtualization#Virtual Machine Types|Virtual Machine]] or at midnight, the [[Virtualization#Virtual Machine Types|Virtual Machine]] is destroyed

# Secure Enclaves
---
- Uses 2 different areas where data can be stored and accessed from ^82b260
- Each enclave can be accessed by the proper processor

# Secure Volumes
---
- Keep data at rest secure
- When data is needed, it is decrypted and mounted
- When it is no longer needed, it is unmounted and encrypted again

# Objectives
---
- [[Objectives#1.5 - Explain different threat actors, vectors, and intelligence sources|1.5 - Explain different threat actors, vectors, and intelligence sources]]
- [[Objectives#2.2 - Summarize virtualization and cloud computing concepts|2.2 - Summarize virtualization and cloud computing concepts]]
- [[Objectives#3.5 - Given a scenario, implement secure mobile solutions|3.5 - Given a scenario, implement secure mobile solutions]]
- [[Objectives#3.6 - Given a scenario, apply cybersecurity solutions to the cloud|3.6 - Given a scenario, apply cybersecurity solutions to the cloud]]