---
tags: [CompTia,SecPlus,CyberSec,Certs]
#aliases:
#cssclass:
#publish:
---

# About
---
- A device that acts as a middle man for your clients ^58c4cc
- Allows company to log and filter out traffic
- Types
	- [[#IP Proxy]]
	- [[#Caching Proxy]]
	- [[#Content Filter]]
	- [[#Web Security Gateway]]

```ad-info
title: Proxy Visual
collapse:close
![[ProxyServer1.png]]
```

# IP Proxy
---
- Used to secure a network by <u>keeping its machines anonymous</u> during web browsing
- Computer that is receiving a request from a proxy will see the web request come from the proxy and not the device that originally made the request
- Proxy is using [[Network Address Translation]] to accomplish this

# Caching Proxy
---
- Attempts to serve client requests by delivering the content to the client from itself without contacting the remote server each time
- Once you visit a website the proxy will temporarily hold a copy of that website for a set amount of time depending on the configuration
- The next time someone makes a request for the website the proxy itself will instead deliver the content if it is still cached
- Save on bandwidth and increase web speed
- Most common proxy is an HTTP proxy
	- <u>Not as effective now</u> since there is a lot of custom content from Web 2.0
- Browsers have a Proxy Auto-Configuration (PAC) file to simplify configuring proxy setup
	- Attackers may try to modify in order to redirect to their site
	- <u>Best to disable PAC file</u> and configure either manually or via something like [[Group Policies]] 

# Content Filter
---
- Used in organizations to prevent users from accessing prohibited websites and other content
	- Websites, email, IM
- See also [[Popup Blockers#Content Filter|Popup Blockers]]

# Web Security Gateway
---
- Acts a go-between device that scans for viruses, filters unwanted content, and performs [[Data Loss Prevention]] functions  ^08d731
- Looks both at <u>incoming and outgoing</u> traffic

# Objectives
---
- [[Objectives#3.3 - Given a scenario, implement secure network designs|3.3 - Given a scenario, implement secure network designs]]
- [[Objectives#4.4 - Given an incident, apply mitigation techniques or controls to secure an environment|4.4 - Given an incident, apply mitigation techniques or controls to secure an environment|]]

# TODO (Delete when done)
---
- [x] Added vocab
- [x] Added and linked objectives in document
- [x] Linked objectives back to document
- [x] Linked any relevant backlinks to and from document