---
tags: [CompTia,SecPlus,CyberSec,Certs]
#aliases:
#cssclass:
#publish:
---

# About
---
![[Software Development#Software Development Life Cycle (SDLC)]]

# Developer Fundamentals
---
1. The CIA Model ![[SecBasics#^51b6d8]]
2. Code review
	1. During testing phase of [[Software Development#Waterfall Model|Waterfall Model]] perform an in depth review to meet CIA model
	2. Generally done by programmers and not the security team
3. Good security is put in place from the beginning
	1. During the [[Software Development#Planning & Analysis|Planning & Analysis]] and [[Software Development#Implementation|Implementation]] phases
	2. Cheaper to do <u>thorough testing before product release</u> than after

# Threat Modeling
---
- Prioritizes vulnerability identification and patching  throughout the [[Software Development#Software Development Life Cycle (SDLC)|SDLC)]] ^666e21
- By prioritizing threats an analyst can identify applications or systems that should receive additional protections, which ones have known vulnerabilities, which threats are most likely to affect the system
- Can then appropriately assign resources to address any issues

# Secure Coding Practices

## Least Privilege
---
- Users and processes should run using the <u>lease amount of access necessary</u> to perform any given function ^a507db
- Program should run as user and not admin
- Don't confuse with [[Unnecessary Applications#Least Functionality|Least Functionality]]

## Defense In Depth
---
- Layering of security controls is more effective and secure than relying on a single control ^526bd3

## Never Trust User Input
---
- Any input that is received from #UserAction and input should undergo "input validation" prior to allowing it to be utilized by the application
	- Ensuring information entered is valid and not able to negatively affect a system

## Minimize Attack Surface
---
- Reduce the amount of code used by a program, eliminate unneeded functionality, and require authentication prior to running additional plugins

## Create Secure Defaults
---
- Default installations should include secure configurations instead of requiring a user or administrator to add additional security
- Users will often accepts the defaults a program provides

## Authentication & Integrity
---
- Applications should be deployed using code signing to ensure the program is not changed inadeptly or maliciously prior to delivery to an end user
- Digital signatures prove the software is authentic and can maintain [[SecBasics#^1f11b5|Integrity]] throughout its lifecycle

## Fail Securely
---
- Every app will fail at some point
- Applications should be coded to properly conduct error handling for exceptions in order to fail securely instead of crashing or being exploited
- [[#Never Trust User Input|Input validation]] is able to assist by making sure only valid data and input goes through

## Fix Security Issues
---
 - If a vulnerability is identified then it should quickly AND correctly patched to remove the vulnerability
 - Otherwise it leaves opportunities for attackers

## Rely on Trusted SDKs
---
- Allows programmers to use code made by others in order to save time and effort ^e6f72a
- For example you don't need to recreate code to open a file on #Windows
- Software Development Kits (SDK) must come from trusted sources to ensure no malicious code is being added
- Applies to 3rd party libraries as well

# Objectives
---
- [[Objectives#1.6 - Explain the security concerns associated with various types of vulnerabilities|1.6 - Explain the security concerns associated with various types of vulnerabilities]]
- [[Objectives#2.3 - Summarize secure application development, deployment, and automation concepts|2.3 - Summarize secure application development, deployment, and automation concepts]]
- [[Objectives#3.2 - Given a scenario, implement host or application security solutions|3.2 - Given a scenario, implement host or application security solutions]]
- [[Objectives#5.3 - Explain the importance of policies to organizational security|5.3 - Explain the importance of policies to organizational security]]

# TODO (Delete when done)
---
- [ ] Added vocab
- [ ] Added and linked objectives in document
- [ ] Linked objectives back to document
- [ ] Linked any relevant backlinks to and from document