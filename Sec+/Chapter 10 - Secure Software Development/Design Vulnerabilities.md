---
tags: [CompTia,SecPlus,CyberSec,Certs]
#aliases:
#cssclass:
#publish:
---

# About
---
- Vulnerabilities often arise from the general design of the software code
- Bad design = More vulnerabilities

# Insecure Components
---
- Any code that is used or invoked outside the main program development process ^a1d24f
- Several forms
	- Code reuse
		- Copy code from another app or the internet and apply it to your program
		- If you don't check that code it may be insecure
	- Third Party Libraries
		- Anytime you bring a library in you may be importing that insecure code such as a #DLL or a Shared Object Library in Linux
	- [[SDLC Principles#Rely on Trusted SDKs|Software Development Kits (SDK)]]
		- Helpful because there are prebuilt functions
		- However the code from the SDK may be insecure and importing it into your program can invite risk
- In Particular with an SDK or Third Party Library, if a vulnerability is found and patched you have have to update those components to ensure you are using the most secure form of code
	- See also [[Updates and Patches]]

# Insufficient [[SecBasics#^45fffd|Logging and Monitoring]]
---
- Any program that does not properly record or log detailed enough information for an analyst to perform their job ^ec410b
- [[SecBasics#^45fffd|Logging and Monitoring]] must support your use case and answer the "who, what, when, where, and how"
- Organization determines level of [[SecBasics#^45fffd|Logging]] and other details

# Weak or Default Configurations
---
- Any program that uses ineffective credentials or configurations, or one in which the defaults have not been changed for security ^4eadc3
- Many applications ask for root or local admin as default
	- Does this program really need to run as admin?
	- Apply [[SDLC Principles#Least Privilege|Least Privilege]]
- Permissions may be too permissive on files or directories due to a weak configuration
- In particular, hardware sometimes has [[Software Vulnerabilities & Exploits#Backdoors|Backdoors]] built in or U/P being something like admin/admin

# Best Practice
---
- Utilize scripted installations and [[Unnecessary Applications#Baseline Image|Baseline]] configuration templates to secure applications during installation

# Objectives
---
- [[Objectives#1.3 - Given a scenario, analyze potential indicators associated with application attacks|1.3 - Given a scenario, analyze potential indicators associated with application attacks]]
- [[Objectives#1.6 - Explain the security concerns associated with various types of vulnerabilities|1.6 - Explain the security concerns associated with various types of vulnerabilities]]
- [[Objectives#2.3 - Summarize secure application development, deployment, and automation concepts|2.3 - Summarize secure application development, deployment, and automation concepts]]
- [[Objectives#2.6 - Explain the security implications of embedded and specialized systems|2.6 - Explain the security implications of embedded and specialized systems]]