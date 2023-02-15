---
tags: [CompTia,SecPlus,CyberSec,Certs]
#aliases:
#cssclass:
#publish:
---

# About
---
- [[#Blackholing or Sinkholing]]
- [[NIDS & NIPS|IPS]]
	- Good for small scale attacks but you will likely not have enough processing power to handle anything larger or a [[Distributed Denial of Service (DDOS)]]

# Blackholing or Sinkholing
---
- Identifies any attacking IP address and routes all their traffic to a non existent server through the null interface ^b44ba7
- Attackers can move to a new IP often making this a temporary fix 

# Elastic Cloud Infrastructure
---
- Having an [[Virtualization#^a6ee8d|Elastic]] [[Cloud Based Infrastructure]] so that the provider can handle for you
	- Scaling up and down as demand increases you can often wait it out
- Most providers often charge for your resources so you will get a larger bill than normal
- No return of investment based on increased traffic because it was all junk
- There are some specialized cloud providers such as #Cloudflare or #Akahmi specifically for mitigating [[Distributed Denial of Service (DDOS)]] attacks
	- [[Firewalls#Web Application Firewall (WAF)|Web Application Firewall (WAF)]]
	- content Distribution on behalf of your organization
- Additional [[SDLC Principles#Defense In Depth|Defense]] within your [[The OSI Model|OSI]]

# Objectives
---
- [[Objectives#2.1 - Explain the importance of security concepts in an enterprise environment|2.1 - Explain the importance of security concepts in an enterprise environment]]
- [[Objectives#2.3 - Summarize secure application development, deployment, and automation concepts|2.3 - Summarize secure application development, deployment, and automation concepts]]