---
tags: [CompTia,SecPlus,CyberSec,Certs]
#aliases:
#cssclass:
#publish:
---

# About
---
- Both smart cars and older cars have vulnerabilities
- With the addition of Cellular, wifi, Bluetooth and other connections this can make a car and #IOT device

# Controller Area Network (CAN)
---
- Digital serial data communication network used within vehicles ^658041
- Vehicles systems that connect together including things like [[HVAC]], cruise control, steering, etc  
- Not to be confused with Campus Area Networks (CAN)
- [[#Controller Area Network (CAN)]] Bus similar to Ethernet that because it assumes anything connected to it is trusted 
- If a CAN is isolated from other networks it can be considered more secure
	- However, there are now cars that come with cellular, Bluetooth, WIFI and other connections to the outside world
- A CAN bus has <u>no form of source addressing or message authentication</u>
- So any traffic on a CAN bus is allowed to run

# Onboard Diagnostic (ODB-II)
---
- Started in 1990's
- Provides a port to plug into in order to get diagnostic codes from a [[#Controller Area Network]] ^c86dc0

```ad-example
title: ODB-II Car Port
collapse:close
![[ODB2PortEx1.png]]
```

```ad-example
title: [[#Controller Area Network (CAN)]] Bus Diagram
collapse:close
![[CANEx1.png]]
```

# Accessing
---
- Locally
	- Common to be under dashboard 
	- So someone could attach a remotely accessible ODB2 module
- Cellular
	- If your car has it
	- Most cars have 2 networks, an entertainment network (radio, wifi, streaming music), and the vehicle
- Wireless
	- Similar to cellular issues but over wireless

# Objectives
---
- [[Objectives#2.6 - Explain the security implications of embedded and specialized systems|2.6 - Explain the security implications of embedded and specialized systems]]