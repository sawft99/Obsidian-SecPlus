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
- Do not hardcode or embed keys in code 

# Logging and Monitoring
---
-

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