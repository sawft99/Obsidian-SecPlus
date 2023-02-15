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

# Insecure [[Application Programming Interface (API)|API]]
---
- ALWAYS use over TLS or HTTPS
	- HTTP transmits unencrypted
- Data received should go through server side [[SDLC Principles#Never Trust User Input|Input Validation]]
- How you will perform [[Testing Methods#Errors|Error Handling]], error messages, and [[SDLC Principles#Fail Securely|Failing Securely]]
	- Errors may give attackers hints into how to exploit the system
	- Sanitize errors as well
- Not subject to [[Denial of Service (DoS)]]
	- Throttling and Rate limiting
		- Limiting certain amount of input and request from users
- See also
	- [[Application Programming Interface (API)]]

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
- Logs must be copied from  [[Virtualization#^a6ee8d|Elastic]]clients to long term storage
	- Example
		- Storing logs solely on a temporary VM that is then deprovisioned after some time
		- You no longer have access to logs

# Unprotected Storage
---
- Most storage containers refereed to as:
	- Buckets
		- Typically AWS
	- Blobs
		- Typically Azure
- DO NOT nest [[Hypervisors#Application Containerization|Containers]]
- Access control to storage is administered through
	- Container policies
	- Identity Access Management (IAM) authorizations
	- Object [[Routers#Access Control List (ACL)|Access Control List (ACL)]]
- Check for incorrect permissions
	- Buckets and blobs create default permissions
- Incorrect origin settings may occur with [[#^4b8e9c|Content Delivery Networks (CDN)]]
	- You need to configure a Cross Origin Sharing (CORS) policy
		- A CDN policy that instructs the browser to treat requests from domains it specifies as safe ^34f55a
		- A weak CORS policy can expose you to some vulnerabilities such as [[XSS and XSRF]]
- See also
	- [[Hypervisors#Application Containerization]]

# Vocab
---
- Content Delivery Network (CDN)[^1]
	- A distributed network of servers that can efficiently deliver web content to users ^4b8e9c
	- CDNs store cached content on edge servers in point-of-presence (POP) locations that are close to end users, to minimize latency

# Objectives
---
- [[Objectives#1.3 - Given a scenario, analyze potential indicators associated with application attacks|1.3 - Given a scenario, analyze potential indicators associated with application attacks]]
- [[Objectives#1.6 - Explain the security concerns associated with various types of vulnerabilities|1.6 - Explain the security concerns associated with various types of vulnerabilities]]
- [[Objectives#2.1 - Explain the importance of security concepts in an enterprise environment|2.1 - Explain the importance of security concepts in an enterprise environment]]
- [[Objectives#2.2 - Summarize virtualization and cloud computing concepts|2.2 - Summarize virtualization and cloud computing concepts]]

[^1]: https://learn.microsoft.com/en-us/azure/cdn/cdn-overview