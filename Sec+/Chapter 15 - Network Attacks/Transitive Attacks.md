---
tags: [CompTia,SecPlus,CyberSec,Certs]
#aliases:
#cssclass:
#publish:
---

# About
---
- Conceptual rather than a specific type of attack or method
- Transitive logic
	- If (A = B = C) then (A = C)
- The focus is on trust between networks
- If Network A trusts Network B which trust Network C, then Network A also likely trusts Network C directly or indirectly ^f79b9a
- If an attacker can get into any of the 3 networks then they can likely also get into the other 2
- "Whoever you trust, you are inherently trusting the others that they also trust"
- You are also assuming the risk of the ones you trust as well as your own risks

![[TransitiveAttackEx1.png]]

# Enterprise
---
- An enterprise company might reuse trust between [[Defeding the Servers#Domain Controller|Domain Controller]] to eliminate amount of time and number of times someone needs to authenticate in [[Group Policies#Active Directory|Active Directory]] for a resource
- Often sacrificing security for convenience adds on additional risk

# Objectives
---
- [[Objectives#2.4 - Summarize authentication and authorization design concepts|2.4 - Summarize authentication and authorization design concepts]]
- [[Objectives#3.1 - Given a scenario, implement secure protocols|3.1 - Given a scenario, implement secure protocols]]