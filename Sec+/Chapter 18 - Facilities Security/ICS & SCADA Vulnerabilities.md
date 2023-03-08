---
tags: [CompTia,SecPlus,CyberSec,Certs]
#aliases:
#cssclass:
#publish:
---

# About
---
- A form of Operational Technology (OT)
	- A communication network designed to implement an industrial control system rather than data networking ^c4eb25
	- Doing things in the physical world, closing valves, manufacturing, generating power, etc
	- Not typical end user machines
- <u>Prioritizes Integrity and Availability</u> over Confidentiality
	- [[SecBasics#^51b6d8|CIA Model]]
	- When ICS systems were first created they did not talk to an outside network and so had a physical separation from the rest of the world
- See also
	- [[HVAC#ICS & SCADA Systems]]
	- [[Mitigating ICS & SCADA Vulnerabilities]]

```ad-example
title: ICS Equipment
collapse:close
![[ICSEx1.png]]
```

# Industrial Control Systems (ICS)

## About
---
- A network that manages [[Embedded System Vulnerabilities|Embedded Systems]] ^071964
- Used in many places such
	- Electrical power stations
	- Water suppliers
	- Health services
	- Telecom
	- Manufacturing
	- Defense systems

## Fieldbus
---
- Digital serial data communications used in [[#^c4eb25|Operational Technology]] networks to link [[Embedded System Vulnerabilities#Programmable Logic Controller (PLC)|Programmable Logic Controller (PLC)]] ^5c39a5
- Links everything together

## Human-Machine Interface (HMI)
---
- Input and output controls on a [[Embedded System Vulnerabilities#Programmable Logic Controller (PLC)|Programmable Logic Controller (PLC)]] to allow a user to configure and monitor the system ^c8f818
- Where you actually push buttons or interact with the system in some way

## Data Historian
---
- Software that aggregates and catalogs data from multiple sources within an [[#Industrial Control Systems (ICS)]] ^08d1ed
- Important for a team such as Incident Response

## The Flow
---
- An [[#Industrial Control Systems (ICS)|ICS]] manages the process automation by linking together [[Embedded System Vulnerabilities#Programmable Logic Controller (PLC)|Programmable Logic Controllers (PLC)|PLCs]] using a [[#Fieldbus]] to make changes in the physical world
- A human sees output, gauges, screens, etc and can control this system from a [[#Human-Machine Interface (HMI)]] 

# Supervisory Control and Data Acquisition (SCADA)
---
- A type of [[#Industrial Control Systems (ICS)]] that manages large scale, multiple site, devices and equipment spread over a geographic region ^272ef1
- Typically runs as software on  ordinary computers to gather data from and manage plant devices and equipment with embedded [[Embedded System Vulnerabilities#Programmable Logic Controller (PLC)|Programmable Logic Controller (PLC)]]
- Uses a WAN in some way but always goes back to a central server

# Modbus
---
- A communications protocol used in [[#^c4eb25|Operational Technology]] networks ^6f4846
- Allows [[#Industrial Control Systems (ICS)]] and [[#Supervisory Control and Data Acquisition (SCADA)]] to communicate to each other
- Equivalent to a TCPI/IP function on a normal network
- Gives [[#Industrial Control Systems (ICS)]] and [[#Supervisory Control and Data Acquisition (SCADA)]] hosts the ability to change and query each [[Embedded System Vulnerabilities#Programmable Logic Controller (PLC)|Programmable Logic Controller (PLC)]]
- Proprietary

```ad-example
title: Modbus Traffic
collapse:close
![[ModbusEx1.png]]
```

# Objectives
---
- [[Objectives#2.1 - Explain the importance of security concepts in an enterprise environment|2.1 - Explain the importance of security concepts in an enterprise environment]]
- [[Objectives#2.5 - Given a scenario, implement cybersecurity resilience|2.5 - Given a scenario, implement cybersecurity resilience]]
- [[Objectives#2.6 - Explain the security implications of embedded and specialized systems|2.6 - Explain the security implications of embedded and specialized systems]]