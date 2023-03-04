---
tags: [CompTia,SecPlus,CyberSec,Certs]
#aliases:
#cssclass:
#publish:
---

# About
---
- A computer system that is designed to perform a specific and dedicated function
- Part of [[IOT Vulnerabilities|IOT Devices]] and smart devices
- Usually referred to in the manufacturing or automation fields
- Can be very simple or very complex or use a full OS like #Linux  or #Android
- Support from manufacturer is limited
- Usually <u>want on a separate network</u> from other devices 
- Example
	- Machine measuring amount of liquid going through an IV drip
	- Water treatment plant making sure water is flowing at a certain rate and automatically opening or closing pipes to make sure it does this
	- A power meter on a house that often times connects to the internet

# Static Environments
---
- An environment where changes don't frequently occur or are not allowed at all
- Embedded systems are considered part of a static environment
- The systems being slimmed down to specific functions can make them more secure
- However if the original code has a vulnerability it can be difficult to install [[Updates and Patches]]
# Programmable Logic Controller (PLC)
---
- A type of computer designed for deployment in industrial or outdoor setting that can automate and monitor mechanical systems
- Run on firmware
- You can apply [[Updates and Patches]] to these
- The patches are typically less frequent though

# System on Chip (SoC)
---
- A processor that integrates the platform functionality of multiple logical controllers onto a single chip
- This makes it an Application Specific Integrated Circuit (ASIC) chip
	- A chip already programed with a specific functionality to perform
- Don't confuse with [[Securing the BIOS#^9479f4|Firmware]] which can be referred to as "Software on a chip"
- Can be power efficient and often on smaller devices that will have an embedded system
	- Robot vacuum cleaner
- Leave room for more functionality or parts
- It comes already programmed with what to do so the opposite of [[#Field Programmable Gate Array (FPGA)]]

# Real-Time Operating Systems (RTOS)
---
- A type of operating system that prioritizes deterministic execution of operations to ensure consistent response for time-critical tasks
- A lot of embedded systems can't handle reboots or crashes well
- Embedded systems need to have response times that are predictable within micro seconds
- Shouldn't use a full operating system like #Windows since the response times can be slower and more subject to crashing 
- Example
	- Opening or shutting a valve in an industrial system

# Field Programmable Gate Array (FPGA)
---
- A processor that can be programmed to perform a specific function by a customer rather than at the time of manufacturing
- Not an ASIC chip

# Objectives
---
- [[Objectives#2.6 - Explain the security implications of embedded and specialized systems|2.6 - Explain the security implications of embedded and specialized systems]]

# TODO (Delete when done)
---
- [ ] Added vocab
- [ ] Added and linked objectives in document
- [ ] Linked objectives back to document
- [ ] Linked any relevant backlinks to and from document