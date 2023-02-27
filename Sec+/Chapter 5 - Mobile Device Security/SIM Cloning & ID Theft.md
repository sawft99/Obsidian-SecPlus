---
tags: [CompTia,SecPlus,CyberSec,Certs]
#aliases:
#cssclass:
#publish:
---

# About
---
- Subscriber Identity Module (SIM) card ^f19809
	- Integrated circuit that securely store the International Mobile Subscriber Identity (IMSI) and its related key
	- Tells cellphone towers what Id it should assign to a phone number

# SIM Cloning
---
- Allows <u>two phones to utilize the same service</u> and allows the attacker to <u>gain access to the phones data</u> ^e94d65
	- Someone sends a text to the phone and both phones get it
- Popular in earlier days to use for long distance or international calls
- Modern day use is typically for bypassing #2FA on websites that utilize a call or SMS verification method
- This translates to "ID Theft" or "Account takeover"
- SIMv2 made cloning more difficult

# #SocialEngineering schemes
---
1. Calling service provider to impersonate real person trying to activate a phone
2. Provider asks for info such as where they went to high school, etc.
	1. Easy to obtain with #Reconnaissance and #OSINT or #Intelligence
3. Provider transfers phone service to the attacker

# Protecting
---
- Be conscious of where you post your phone number
- Google voice number
	- Single phone number but no one knows the real number behind it

# Objectives
---
- [[Objectives#1.1 - Compare and contrast different types of Social Engineering techniques|1.1 - Compare and contrast different types of Social Engineering techniques]]
- [[Objectives#2.4 - Summarize authentication and authorization design concepts|2.4 - Summarize authentication and authorization design concepts]]
- [[Objectives#2.6 - Explain the security implications of embedded and specialized systems|2.6 - Explain the security implications of embedded and specialized systems]]
- [[Objectives#3.5 - Given a scenario, implement secure mobile solutions|3.5 - Given a scenario, implement secure mobile solutions]]