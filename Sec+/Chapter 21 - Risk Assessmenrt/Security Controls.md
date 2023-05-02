---
tags: [CompTia,SecPlus,CyberSec,Certs]
#aliases:
#cssclass:
#publish:
---

# About
---
- [[Methodologies]] implemented to [[Risk Assessments#Mitigate|Mitigate]] a particular [[Risk Assessments#Risk|Risk]]
- Categories
	- [[#Management Controls]]
		- [[#Administrative Controls]]
	- [[#Operational Controls]]
	- [[#Technical Controls]]
- Types
	- [[#Preventative Controls]]
	- [[#Detective Controls]]
	- [[#Corrective Controls]]
	- [[#Deterrent Controls]]
	- [[#Compensating Controls]]
	- [[#Physical Controls]]
- See also
	- [[Physical Security]]
	- [[SecBasics#^50e62d|Administrative Controls]]
	- [[SecBasics#^c5223f|Technical Controls]]

# Control Categories

## About
---
- There are 3 main categories of controls
	- [[#Management Controls]]
	- [[#Operational Controls]]
	- [[#Technical Controls]]
- A broad explanation
- All other controls fall into these categories

## Management Controls
---
- Techniques and concerns addressed by an organization’s management ^38f80d
	- Includes [[#Administrative Controls]]
- Controls focused on decision making and management of [[Risk Assessments#Risk|Risk]]
- Policy, procedure, legal compliance, [[Software Development]] procedures, [[Risk Assessments#Vulnerabilities|Vulnerability]] management and more 
- How systems security will be managed and overseen

## Operational Controls
---
- The controls executed by people
- Increase security of system by condoling actions of the users using it ^597951
- User training, config management, testing disaster recovery systems, incident handling and more
- Performed by technical people
- Carries out orders dictated by [[#Management Controls]]

## Technical Controls
---
- The logical controls executed by the computer system ^1e1506
- Safeguards and countermeasures used to avoid, detect, counteract, or minimize security risk to maintain systems and information
- Logical controls that are put into a system to help secure it
- Includes [[Authentication]], [[Access Control]], [[SecBasics#^45fffd|Auditing]], [[Authentication Attacks#Passwords|Passwords]], [[Disk Encryption#^501400|Encryption]], [[Authentication#Multi-Factor Authentication (MFA)|MFA]], cryptography and more

# Control Types

## About
---
- Further breakdown of the types of controls within [[#Control Categories]]

## Preventative Controls
---
- Security controls installed <u>before</u> an event happens and are designed to <u>prevent</u> something from occurring ^17b2e8
- Enforces security policy
- The only way to bypass is to find a flaw in implementation or logic
- Usually not optional
- Example
	- RAID redundancy, battery backups, [[Biometric Readers]], [[NIDS & NIPS|IPS]], access lists, [[Authentication Attacks#Passwords|Passwords]], fences. security awareness, [[Access Control Best Practices#^de781b|Separation of Duties]], [[Access Control]], security policies, and [[NIDS & NIPS|IPS]]

## Detective Controls
---
- <u>Monitoring and detecting</u> any unauthorized behavior or hazard ^2a0915
- Used <u>during</u> the event to find out whether something bad may have happened
	- Can also be used after an incident as well though
- Often used to alert about other [[#Control Types]] such as [[#Preventative Controls]], [[#Deterrent Controls]], and [[#Compensating Controls]] failing
- CCTV, [[IDS]], logging review, motion detection, [[SIEM]]

## Corrective Controls
---
- <u>Limit the extent of damage</u> and help the company <u>recover</u> from damage quickly ^9d1cce
- Used <u>after</u> an event occurs
	- Controls include all other [[#Control Types]] used <u>during an incident to correct the problem</u>
- Backups, [[Updates and Patches]], incident response, disaster recovery, switching locations, quarantining an infected computer, sending a guard to block an intruder, and terminating an employee for not following security policy

## Deterrent Controls
---
- Attempts to deter threat actors from executing an offensive assault on their environment ^e56dea
- If potential threat actors see that this type of control is in place they may decide to move on
- Can be similar to [[#Preventative Controls]] but it's primary objective is deterrence
- Example
	- Visible alarm system
	- A system banner warning that any unauthorized attempt to log in will be monitored and punished
	- A threat actor on the internet sees a particular technology implemented that would make their attack difficult

## Compensating Controls
---
- A control put in place to satisfy security requirements that are either impractical or too difficult to implement
- Used whenever you can't meet the requirement for a normal control
- AKA "Alternative Controls"
- Example
	- [[#Physical Controls]] and policy dictate every door should have [[Biometric Readers]] but it is not available in a particular region, so instead you install another type of [[Door Locks|Door Lock]]
	- Instead of using expensive [[Root of Trust#Hardware Security Module (HSM)|HSM]], an organization might opt to use [[Network Access Control|NAC]], [[Data Loss Prevention (DLP)|DLP]] and other security methods
	- Instead of implementing [[Access Control Best Practices#^de781b|Separation of Duties]], an organization might opt to do additional logging and [[SecBasics#^45fffd|Auditing]]

```ad-danger
title: Risk
collapse:close
Any [[Risk Assessments#Residual|Residual Risk]] not covered by the compensating control is considered [[Risk Assessments#Accept|Accepted Risk]] 
```

## Physical Controls
---
- Security measures that are designed to [[#Deterrent Controls|Deter]] <u>or prevent</u> unauthorized access to sensitive information or the systems that contain it ^a078f0
- Can be considered the first line of defense
	- [[Firewalls]] can be considered the first line of defense for a network
- Fences, guards, cameras...

# Administrative Controls
---
- Focused on changing the behavior of people instead of removing the actual [[Risk Assessments#Risk|Risk]] involved
- Policy, procedure, [[Access Control Best Practices#^cc194a|Mandatory Vacation]], Disaster Recovery Plans
- Not something that will actually stop you, just written polices
- Considered part of [[#Management Controls]]

# Multiple Categories
---
- Some controls can be in multiple categories or types
- Example
	- CCTV can be used to monitor making it part of [[#Physical Controls]] but it can also be used to see if something is currently happening making it part of [[#Detective Controls]]
	- Password policy can be part of both [[#Management Controls]] and [[#Administrative Controls]] since both include policies
	- [[Door Locks]] are both [[#Physical Controls]] and [[#Preventative Controls]]

# Objectives
---
- [[Objectives#5.1 - Compare and contrast various types of controls|5.1 - Compare and contrast various types of controls]]