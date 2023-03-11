---
tags: [CompTia,SecPlus,CyberSec,Certs]
#aliases:
#cssclass:
#publish:
---

# About
---
- Systems used for building automation and physical access security ^e36166
	- Such as [[Door Locks]] or [[Surveillance|Cameras]]
- A different type of network than typical IT or [[ICS & SCADA Vulnerabilities#^c4eb25|Operational Technology]] 
- Should also have its own [[Network Zones]] or some other network segmentation keeping it from the other networks
- Many systems allow monitoring across the corporate network or internet
	- Can be dangerous as an internet connection can be an opening for attackers
 
# Building Automation Systems (BAS)

## About
---
- Components and protocols that facilitate the centralized configuration and monitoring o mechanical and electrical systems within offices and data centers
- <u>Separate</u> from [[ICS & SCADA Vulnerabilities|ICS & SCADA]]
- Specifically for systems related to the building and insuring its functionality
- Examples
	- Elevators
	- Battery backups
	- [[HVAC]]
	- Lights

# Vulnerabilities
---
- Process and memory in [[Embedded System Vulnerabilities#Programmable Logic Controller (PLC)|Programmable Logic Controller (PLC)]]
- Plaintext credentials or keys in code
- Code injection in web interface
	- [[XSS and XSRF]]
	- [[SQL Injection]]
	- [[XML Vulnerabilities|XML Injection]]

# Other concerns
---
- If exploited, can be used to create a [[Denial of Service (DoS)]] since it could affect the way the building functions
	- HVAC turned off and causing systems to overheat
- Systems, if not [[Network Zones|Segmented]] properly, can be used as a [[Malware Infections#Attack Vector|Attack Vector]]or pivot point for #LateralMovement

# Physical access Control Systems (PACS)
---
- Components and protocols that facilitate the centralized configuration and monitoring of security mechanisms within offices and data centers
	- [[Surveillance]]
	- [[Door Locks]]
- Can be integrated into [[#Building Automation Systems (BAS)]] or a completely separate system
	- Often installed and maintained by a third party
	- Often it is omitted from risk analysis or vulnerability assessment
	- The responsibility is still yours unless you specifically get it stated in writing otherwise

# Objectives
---
- [[Objectives#1.2 - Given a scenario, analyze potential indicators to determine the type of attack|1.2 - Given a scenario, analyze potential indicators to determine the type of attack]]
- [[Objectives#1.3 - Given a scenario, analyze potential indicators associated with application attacks|1.3 - Given a scenario, analyze potential indicators associated with application attacks]]
- [[Objectives#1.7 - Summarize the techniques used in security assessments|1.7 - Summarize the techniques used in security assessments]]
- [[Objectives#2.6 - Explain the security implications of embedded and specialized systems|2.6 - Explain the security implications of embedded and specialized systems]]

# TODO (Delete when done)
---
- [ ] Added vocab
- [ ] Added and linked objectives in document
- [ ] Linked objectives back to document
- [ ] Linked any relevant backlinks to and from document