---
tags: [CompTia,SecPlus,CyberSec,Certs]
#aliases:
#cssclass:
#publish:
---

# About
---
- <u>Users bring their own device</u> and use it on the company network
	- Some places are fully for and others are fully against

# Security Issues
---
- BYOD brings new concerns
- Some ones <u>device plugged into your network introduces all of their vulnerabilities</u>
- Companies don't control the device

# Other considerations
---
- <u>Saving money</u> by using BYOD
- Is it company data or personal data?
	- Using [[#Storage Segmentation]] to keep data separate

# Storage Segmentation
---
- Creating a clear <u>separation between personal and company data</u> on a single device ^9579c9
- Many solutions both procedural and highly technical
- Technical example
	- An app named "Work" which uses a <u>virtual environment</u> to keep all company data in one place
	- Once exited you return to your normal/personal device state
- Procedural/Administrative example
	- <u>Separate email apps and clients for work and personal</u>
	- <u>Nothing prevents crossover other than policy</u>

# Patching
---
- [[Security of Apps#Mobile Device Management (MDM)|MDM]] can handle OS and app patching for devices the company hands out
- People may not allow [[Security of Apps#Mobile Device Management (MDM)|MDM]] software to be installed on their device in BYOD instances

# Choose Your Own Device (CYOD)
---
- Company provides a phone from a list of several supported models ^9bf98c
- Company may install [[Security of Apps#Mobile Device Management (MDM)|MDM]] software on device
	- Policy can be dictated to stop certain apps from being installed on the device
	- [[Data Loss Prevention (DLP)]] features may be available
	- Other features can be turned on and off
		- Example
			- Stopping devices from connecting to Wifi
			- Still can not use at home

# Tip
---
- Ensure you have a policy and a choice was not made default by not actually making a choice

# [[Objectives]]
---
- [[Objectives#3.5 - Given a scenario, implement secure mobile solutions|3.5 - Given a scenario, implement secure mobile solutions]]