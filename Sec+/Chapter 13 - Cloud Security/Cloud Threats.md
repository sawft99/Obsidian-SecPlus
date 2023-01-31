---
tags: [CompTia,SecPlus,CyberSec,Certs]
#aliases:
#cssclass:
#publish:
---

# About
---
- Most forms happen in identity and Access Management
- [[#Insecure API]]
- [[#Improper Key Management]]
- [[#Logging and Monitoring]]
- [[#Unprotected Storage]]

# Insecure API
---
- ALWAYS use over TLS or HTTPS
	- HTTP transmits unencrypted
- Data received should go through server side [[SDLC Principles#Never Trust User Input|Input Validation]]
- How you will perform [[Testing Methods#Errors|Error Handling]], error messages, and [[SDLC Principles#Fail Securely|Failing Securely]]
	- Errors may give attackers hints into how to exploit the system
	- Sanitize errors as well
- Not subject to #DDoS
	- Throttling and Rate limiting
		- Limiting certain amount of input and request from users
- See also [[Application Programming Interface (API)]]

# Improper Key Management
---
- Keys used for multiple purposes including but not limited to cryptography, [[SecBasics#^45fffd|Authentication]], [[SecBasics#^45fffd|Authorization]]
- [[Application Programming Interface (API)|API]] should use secure [[SecBasics#^45fffd|Authentication]] and [[SecBasics#^45fffd|Authorization]] before accessing data such as:
	- SAML
	- OAuth
	- OIDC
- <u>Do not hardcode or embed keys in code </u>
- If keys are no longer needed delete them
- When moving code from development to production regenerate new keys for use
	- Code is exposed to a lot of people in the development process and those people may have been compromised
- Ensure all systems have had [[Hardening]] practices applied and are only running [[Restricting Applications#Whitelisting|Whitelisted]] apps

# Logging and Monitoring
---
- Ensure sufficient logging
- [[As a Service#Software as a Service (SaaS)|Software as a Service (SaaS)]] may not supply access to log files or monitoring tools

# Unprotected Storage
---
-


# Objectives
---
- Obj

# TODO (Delete when done)
---
- [ ] Added vocab
- [ ] Added and linked objectives in document
- [ ] Linked objectives back to document
- [ ] Linked any relevant backlinks to and from document