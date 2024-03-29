---
tags: [CompTia,SecPlus,CyberSec,Certs]
#aliases:
#cssclass:
#publish:
---

# About
---
- Term used to describe devices that provide voice communication to users ^9ad8ff
- Originally used in networks to make outside connections

# Modems
---
- A device that can modulate digital information into an analog signal for transmission over a standard dial-up phone line ^6e0cc5
- Could plug directly into a computer/server
- Such as AOL

# War Dialing

## About
---
- Attacker dials random numbers to see if a modem answers
- Servers had dial up modems so support could access their servers

## Prevention
---
- Callback feature on modem
	- When someone calls in the modem hangs up and if it is a recognized number the modem would call back to establish the connection
	- Verifies who a person is
- [[SecBasics#^45fffd|Authentication]]
	- Username and Password
	- 2FA/MFA
- Eliminate modems and switch to SSH
- Keep dialup number secret

# Public Branch Exchange (PBX)

## About
---
- Internal phone system used in large organizations ^7d5fa4
- More common than modem
- Attackers often go after to get free long distance calls

## Prevention
---
- Have PBX in a physically secure location with things such as locks
- Disable remote access
	- How attackers will most often access

# Voice Over Internet Protocol (VOIP)

## About
---
- The newest method
- Cheaper than PBX
- More secure than PBX
- Easier to manage vs PBX
- Common for companies to use [[Subnetting]] and [[VLAN]] to create separate voice and data networks
- Many organizations try to run both on the same network
- Relies on IP phones, software, and VOIP gateways ^0b3233
	- IP phones use an ethernet cable versus a traditional phone cable

## Prevention
---
- Update [[Securing the BIOS#^9479f4|Firmware]] and install [[Updates and Patches]]
- Use good authentication and [[Disk Encryption#^501400|Encryption]]

## Quality of Service (QOS)
---
- The use of mechanisms or technologies that work on a network to control traffic and ensure the performance of critical applications with limited network capacity [^1] ^89467f
- Applies to [[#Voice Over Internet Protocol (VOIP)]]
- Implement to improve [[SecBasics#^51b6d8|Availability]]
- VOIP can use a lot of bandwidth
- High latency can affect phone calls very easily
- Susceptible to [[Denial of Service (DoS)]]

# Objectives
---
- [[Objectives#3.1 - Given a scenario, implement secure protocols|3.1 - Given a scenario, implement secure protocols]]
- [[Objectives#3.3 - Given a scenario, implement secure network designs|3.3 - Given a scenario, implement secure network designs]]

[^1]: https://www.fortinet.com/resources/cyberglossary/qos-quality-of-service