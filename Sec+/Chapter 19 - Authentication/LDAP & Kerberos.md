---
tags: [CompTia,SecPlus,CyberSec,Certs]
#aliases:
#cssclass:
#publish:
---

# About
---
- Lightweight Directory Access Protocol (LDAP)
	- [[The OSI Model#Application|Application]] layer protocol for accessing and modifying directory services ^defef1
	- A <u>database</u> used to centralize information about <u>clients and objects</u> in the network ^f4cd5e
	- A simplified version of X.500
	- Hierarchical organization of users, groups, servers, and systems
	- Ports
		- 389 - Unencrypted
		- 636 - Encrypted/[[#LDAPS]]
	- [[Group Policies#Active Directory|Active Directory]] is the #Microsoft version of LDAP
	- Can also be used as part of security policies or [[Access Control]] through [[Group Policies]]
- Kerberos
	- An [[Authentication]] protocol used by #Windows to provide [[802.1x#^539a82|Mutual Authentication]] using <u>a system of tickets</u> ^9ae466
	- Port
		- 88 - The 'important parts' are encrypted but the username is sent in the clear at the beginning
- See also
	- [[Defeding the Servers#Domain Controller]]

# LDAPS
---
- Lightweight Directory Access Protocol over SSL ^519fec
- Can be TLS or SSL
- Encrypted since <u>LDAP by default is unencrypted</u>

# Kerberos Process

## About
---
1. User contacts the [[Defeding the Servers#Domain Controller|Domain Controller]] which acts as the <u>Key distribution Center (KDC)</u> to login to the domain
	1. Performs [[Authentication]] and ticket granting
2. If authenticated the client is granted a <u>Ticket Granting Ticket (TGT)</u>
3. Then provided to the [[Defeding the Servers#Domain Controller|Domain Controller]] when a user tries to access a resources
4. The [[Defeding the Servers#Domain Controller|Domain Controller]] then provides the user with session key or service ticket; Whichever is appropriate
5. Tickets are presented to the resource and access is then granted
	1. Resources always trust the [[Defeding the Servers#Domain Controller|Domain Controller]] providing the tickets

# Drawbacks
---
- Because the [[#Kerberos Process]] relies on the [[Defeding the Servers#Domain Controller|Domain Controller]] to server as the KDC this <u>can be a single point of failure</u>
	- If the [[Defeding the Servers#Domain Controller|Domain Controller]] is down then ticket granting is down
	- Many people have a primary and secondary [[Defeding the Servers#Domain Controller|Domain Controller]] to ensure both <u>LDAP and Kerberos</u> are still running
- Time must always be in sync or very close to each other
	- Login locally and correct issue with time

# Objectives
---
- [[Objectives#1.3 - Given a scenario, analyze potential indicators associated with application attacks|1.3 - Given a scenario, analyze potential indicators associated with application attacks]]
- [[Objectives#3.1 - Given a scenario, implement secure protocols|3.1 - Given a scenario, implement secure protocols]]
- [[Objectives#3.8 - Given a scenario, implement authentication and authorization solutions|3.8 - Given a scenario, implement authentication and authorization solutions]]
- [[Objectives#5.4 - Summarize risk management processes and concepts|5.4 - Summarize risk management processes and concepts]]