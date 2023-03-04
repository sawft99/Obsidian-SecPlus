---
tags: [CompTia,SecPlus,CyberSec,Certs]
#aliases:
#cssclass:
#publish:
---

# About
---
- Function as a Service
- A cloud service model that supports [[#Serverless]] software architecture by provisioning runtime [[Hypervisors#Application Containerization|Containers]] in which code is executed in a particular programming language ^565a28
	- Running apps without having your own dedicated servers
- Don't have to worry about [[Updates and Patches]] and other management
- See also 
	- [[Hypervisors#Application Containerizatio]]
	- [[Threats to VMs#Compromised Containers]]

# Serverless

## About
---
- A software architecture that runs functions within a [[Virtualization|Virtualized]] runtime [[Hypervisors#Application Containerization|Containers]] rather than on a dedicated server instance
- Everything is developed as a single function or microservice
	- How applications can be deployed as a collection of services that are highly maintainable and testable and independently deployable ^2e5a22
- Don't need to manage physical or virtual servers
- Don't have to worry about:
	- [[Updates and Patches]]
	- Administration
	- File monitoring
- Only pay for when program is executed and running
- Underlying architecture is handled by a cloud provider
	- [[Misc#^d2ea95|Vendor lockin]]
- [[#Serverless]] relies on [[Workflow Orchestration]]

## Securing
---
- Ensure developers clients and machines have not been compromised
- Secure coding, secure workstation, secure storage of credentials
- See also
	- [[Testing Methods#Forms Of Code Analysis]]
	- [[Hardening]]
	- [[Securing Storage Devices]]

# Objectives
---
- [[Objectives#2.2 - Summarize virtualization and cloud computing concepts|2.2 - Summarize virtualization and cloud computing concepts]]