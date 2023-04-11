---
tags: [CompTia,SecPlus,CyberSec,Certs]
#aliases:
#cssclass:
#publish:
---

# About
---
- Implicit Deny ^7d2bd6
	- All access to a resource is <u>denied by default</u> and is only allowed when <u>explicitly</u> stated ^41b476
	- More secure
- Explicit Deny ^d2594e
	- All access to a resource is <u>allowed by default</u> and is only blocked when explicitly stated  ^10abe0
	- Less secure
- Least Privilege
	- Users are only given the lowest level of access needed to perform their job function ^6116b3
- Separation of Duties ^de781b
	- Require more than one person to conduct a sensitive task or operation ^f50190
	- This policy distributes control over a system, infrastructure, or particular task
	- Examples
		- Can use a sign and cosign setup, an approval process, or some other mechanism
		- Can also apply to a single user such as having a normal user account and an admin account for the same person
			- Use your normal user account for most daily operations and only the admin account when you need to perform an admin operation
			- Can help with [[Preventing Malware]] since you would likely not get infected while using an admin account
		- In Windows this can be accomplished with User Account Control (UAC)
- Job Rotation ^bf9191
	- Occurs when users are cycled through various jobs to learn the overall operations better, reduce their boredom, enhance their skill level, and increase security ^48dfa6
	- Helps facilitate [[#^de781b|Separation of Duties]] to prevent fraud and abuse
- Mandatory Vacation ^cc194a
	- Requiring vacation ^8f22f2
	- Helps facilitate [[#^de781b|Separation of Duties]] of forcing someone else to fill your role while gone
- See also
	- [[Access Control]]
	- [[SDLC Principles#Least Privilege]]

# Objectives
---
- [[Objectives#2.7 - Explain the importance of physical security controls|2.7 - Explain the importance of physical security controls]]
- [[Objectives#3.8 - Given a scenario, implement authentication and authorization solutions|3.8 - Given a scenario, implement authentication and authorization solutions]]
- [[Objectives#5.3 - Explain the importance of policies to organizational security|5.3 - Explain the importance of policies to organizational security]]