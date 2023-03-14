---
tags: [CompTia,SecPlus,CyberSec,Certs]
#aliases:
#cssclass:
#publish:
---

# About
---
- A provisioning architecture in which deployment of resources is performed by scripted automation and [[Workflow Orchestration]] ^c5efc7
- Core component of [[Cloud Computing]] and [[DevSecOps]] to allow for rapid deployment
- Robust [[Workflow Orchestration]] can lower overall IT costs, speed up deployments, and increase security ^b35aaa

# Security
---
- IAC considered more secure because it allows for scripted approaches to provisioning #Infrastructure to the cloud
- Scripts generally don't have mistakes so once you have a configuration that you like and it is secure, you can guarantee something is deployed properly
	- Templates and standardization
	- [[#Idempotence]]
- Some people or instances may call for an exception to the standard scripts and templates which is nicknamed "Snowflake Systems" ^6fdc48
	- Can lead to security, config, inefficiency, and support issues

# Idempotence
---
- A property of IAC where an automation or [[Workflow Orchestration]] action always produces the same result <u>regardless of the components previous state</u> ^eeddf2
- Consistent and compliant
- Runbooks are scripts inside of [[Workflow Orchestration]]
	- A series of conditional steps to perform actions such as enriching data, containing threats, and sending notifications automatically as part of the incident response or security operations process ^35a93c
	- Should have a VERY good reason to be an exception with a decision from higher up allowing it

# Objectives
---
- [[Objectives#1.7 - Summarize the techniques used in security assessments|1.7 - Summarize the techniques used in security assessments]]
- [[Objectives#2.2 - Summarize virtualization and cloud computing concepts|2.2 - Summarize virtualization and cloud computing concepts]]
- [[Objectives#2.3 - Summarize secure application development, deployment, and automation concepts|2.3 - Summarize secure application development, deployment, and automation concepts]]