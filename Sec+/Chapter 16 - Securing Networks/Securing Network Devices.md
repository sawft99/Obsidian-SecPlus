---
tags: [CompTia,SecPlus,CyberSec,Certs]
#aliases:
#cssclass:
#publish:
---

# About
---
- Includes
	- [[IDS]]
	- [[NIDS & NIPS]]
	- [[Switches]]
	- [[Routers]]
	- [[Firewalls]]

# Common Vulnerabilities
---
- Default Accounts
	- A user or administrator level account that is installed on a device by the manufacturer during production
- Naming schemes
	- Try not to have easy to guess naming schemes
	- Naming schemes are common though such as first initial last and last name for user accounts
	- See also
		- [[Usernames & Passwords]]
- Device usernames
	- Rather than "Router" or "Switch" for device usernames pick something else such as "RTR283"
- Weak Passwords ^4c4d3e
	- A password should be long, strong, and complex
	- Require 14 characters with a mix of uppercase, lowercase, numbers, and special symbols
	- Don't use dictionary words
- [[Active Intercept & Privilege Escalation|Privilege Escalation]]
	- Attacker obtains access to an account and attempts to get additional access via other accounts such as other users or admins
	- Can be
		- #VerticalMovement
			- A user gains a higher level of access such as to an admin account
		- #LateralMovement 
			- Moving parallel to other users who have the same or similar access as the current account
- [[Backdoors & Logic Bombs|Backdoors]]
	- Bypasses normal authentication in a system
	- Manufacturer could have placed a chip or code in a device that does this
	- [[Supply Chain Assessment]] is crucial for mitigating and preventing risk
		- Where your device comes from ad who's been getting them
		- Buy directly from manufacturer
- [[Network Attacks]]
	- [[NIDS & NIPS]]
	- [[Network Zones]] and Segmentation
		- [[VLAN]]
		- [[Network Zones#DMZ|DMZ]]
	- [[Firewalls]]
	- [[Updates and Patches]]
		- Including [[Trusted Firmware|Firmware]]
	- Secure configurations
- Telnet
	- Sends all information in the clear including username and passwords

# Objectives
---
- [[Objectives#1.2 - Given a scenario, analyze potential indicators to determine the type of attack|1.2 - Given a scenario, analyze potential indicators to determine the type of attack]]
- [[Objectives#1.6 - Explain the security concerns associated with various types of vulnerabilities|1.6 - Explain the security concerns associated with various types of vulnerabilities]]
- [[Objectives#2.1 - Explain the importance of security concepts in an enterprise environment|2.1 - Explain the importance of security concepts in an enterprise environment]]
- [[Objectives#3.3 - Given a scenario, implement secure network designs|3.3 - Given a scenario, implement secure network designs]]
- [[Objectives#3.7 - Given a scenario, implement identity and account management controls|3.7 - Given a scenario, implement identity and account management controls]]