---
tags: [CompTia,SecPlus,CyberSec,Certs]
#aliases:
#cssclass:
#publish:
---

# About
---
- [[Hardening]]
	- Increasing overall device security
- See also 
	- [[Hardening]]

# Methods
---
1. Update device to latest version Software, [[Securing the BIOS#^9479f4|Firmware]], and OS
	1. <u>Most devices are hacked due to not being patched against vulnerabilities</u>
	2. [[Updates and Patches]]
	3. [[Patch Management]]
	4. [[Security of Apps#Mobile Device Management (MDM)|Mobile Device Management (MDM)]]
2. Install [[Endpoint Analysis#AntiVirus (AV)|AntiVirus (AV)]]
3. Train users on proper security and use of the device
	1. Safe websites
	2. How to use social media correctly
	3. What apps are allowed
		1. [[Restricting Applications]]
4. Only install apps from official mobile stores
	1. Stores at least have [[Endpoint Analysis#AntiVirus (AV)|AntiVirus (AV)]]
	2. Google Play Store and Apple App Store
5. Do not [[Security of Apps#Jailbreaking & Rooting|Jailbreak]] #IPhone or [[Security of Apps#Jailbreaking & Rooting|Root]] #Android
	1. Bypasses built-in protection
6. Only use [[SIM Cloning & ID Theft#^f19809|SIMv2]]
7. Turn off all unneeded features
	1. NFC
		1. Short range wireless. Usually within inches.
		2. Such as credit cards
	2. Wifi
	3. Bluetooth
		1. Make device undiscoverable unless pairing
		2. [[Bluetooth Attacks#Protecting|Bluetooth Attacks]]
	4. Mobile Hotspot ^16a462
		1. A place where wireless internet is accessible
		2. Using your phone as a hotspot is known as [[#^092f4f|Tethering]]
	5. Tethering ^092f4f
		1. Using your mobile device to allow other devices to access the internet
		2.  Can be over BLE, Wifi, USB
		3. When using mobile device as [[#^16a462|Mobile Hotspot]]
	6. Location services
8. Turn on encryption for voice and data
	1. Bluetooth
	2. NFC
	3. Wifi
9. Use strong password or biometrics
10. Turn on Find my phone
	1. Setup [[Mobile Device Theft#^4bafd6|Remote Lock]] and [[Mobile Device Theft#^75caa3|Remote Wipe]]
11. Don't allow [[Bring Your Own Device (BYOD)]]
	1. "Bring your own disaster"
	2. [[Bring Your Own Device (BYOD)#Choose Your Own Device (CYOD|Choose Your Own Device (CYOD)]] better policy
12. Employ good security policies

# Objectives
---
- [[Objectives#3.5 - Given a scenario, implement secure mobile solutions|3.5 - Given a scenario, implement secure mobile solutions]]