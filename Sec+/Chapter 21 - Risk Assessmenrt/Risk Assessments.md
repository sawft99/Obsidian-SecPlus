---
tags: [CompTia,SecPlus,CyberSec,Certs]
#aliases:
#cssclass:
#publish:
---

# About
---
- A process used inside of [[#Risk]] management to identify how much risks exists in a given network or system ^af7f6d
- Used to minimize the likelihood of a negative outcome
- Numerous ways to do
	- Mathematical calculating a possibility
	- Subjective guessing a possibility
	- Assessments and Analysis of information

# Risk
---
- The probability that a threat will be realized ^e71eb7
- Exists between [[#Threats]] and [[#Vulnerabilities]]
- If you have [[#Threats]] but no [[#Vulnerabilities]] then you have no risk
- If you have [[#Vulnerabilities]] but no [[#Threats]] then you have no risk

```ad-example
title: Risk
collapse:close
![[RiskEx1.png]]
```

# Vulnerabilities
---
- Weakness in the design or implementation of a system ^e5340c
- The <u>internal</u> factors you can control
- Can be a result of improperly
	- [[Securing Networks]]
	- [[Securing Network Devices]]
	- [[Securing Applications]]
	- [[Securing Network Media]]
	- [[Securing the BIOS]]
	- [[Securing VMs]]
	- [[Securing WIFI Devices]]
	- [[Access Control]]
	- [[Physical Security]]
	- Other systems and more
- If or how you address vulnerabilities is a decision within [[#Risk]] management
- Ways to measure
	- [[Qualitative Risk]]
	- [[Quantitative Risk]]

# Threats
---
- Any condition that could cause harm loss, damage, or compromise IT systems ^929015
- The <u>external</u> factors you can't control
- Can only attempt to <u>minimize or mitigate</u> since you can't control it
- Can be
	- Natural disasters
	- [[SecBasics#Hackers|Hackers]] or other attackers
	- Data integrity breaches
	- Disclosure of confidential information
	- More

# Strategy

## About
---
- [[#Avoid]]
- [[#Transfer]]
- [[#Mitigate]]
- [[#Accept]]
- [[#Residual]]

## Avoid
---
- A strategy that requires <u>stopping</u> the activity that has [[#Risk]] or choosing a less risky <u>alternatives</u> ^668c5c
- Example
	- 100 computer with 15 still running #Windows XP
	- Avoid [[#Risk]] by taking those machines offline or upgrading them to something newer such as #Windows 10

## Transfer
---
- A strategy that passes [[#Risk]] to a third party; most commonly an insurance company ^ed2084
- Example
	- [[#Risk]] of office flooding
	- Purchase an insurance policy

## Mitigate
---
- A strategy that seeks to minimize the [[#Risk]] to an acceptable level ^c0371e
- Example
	- Server that has [[#Vulnerabilities]] with 5 critical, 2 high, 3 medium, and 1 low
	- Choosing which [[#Vulnerabilities]] you want to address first
	- Policy may dictate that a server with critical [[#Vulnerabilities]] be taken offline
- [[#Risk]] not eliminated but minimized or brought down to an acceptable level

## Accept
---
- A strategy that seeks to accept the current level of [[#Risk]] and the costs associated with it if the [[#Risk]] were realized ^39d67e
- If the asses is low cost or impact to the organization is minimal
- Example
	- Looking to [[#Transfer]] [[#Risk]] on a server because it is worth $10,000+ vs accepting the [[#Risk]] of a $500 laptop being damaged

## Residual
---
- The [[#Risk]] leftover after you have tried to [[#Avoid]], [[#Transfer]] or [[#Mitigate]] it ^da5100
- Uncommon since [[#Risk]] exists in almost everything
- Unique to each organization

# Risk Assessment
---
1. Identify assets
	1. List of servers, [[Routers]], desktops, etc
2. Identify [[#Vulnerabilities]]
	1. Can do a vulnerability scan, penetration test, vulnerability assessment
3. Identify [[#Threats]] and their likelihood to occur
4. Identify monetary [[#Risk]] if it is realized

# Vocab
---
- ![[Supply Chain Assessment#^f72c50]]

# Objectives
---
- [[Objectives#5.4 - Summarize risk management processes and concepts|5.4 - Summarize risk management processes and concepts]]