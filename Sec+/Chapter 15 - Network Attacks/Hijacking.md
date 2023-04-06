---
tags: [CompTia,SecPlus,CyberSec,Certs]
#aliases:
#cssclass:
#publish:
---

# About
---
- Exploit of a computer session in an attempt to gain unauthorized access to data, services, or other resources on a computer or server
- Types
	- [[#Session Theft/Session Hijacking]]
	- [[#TCP/IP Hijacking]]
	- [[#Blind Hijacking]]
	- [[#Clickjacking]]
	- [[#Man-in-the-Middle]] ^52b103
	- [[#Man-in-the-Browser]]
	- [[#Watering Hole]]
	- [[#Cross-site scripting (XSS)]]

# Session Theft/Session Hijacking
---
- Attacker guesses the session ID for a web session , enabling them to takeover the already authorized session of the client ^de26fb
- Each session has a random string
- Occurs at [[The OSI Model#Session|Session]] layer in the OSI model
- Can occur at [[The OSI Model#Network|Network]] or [[The OSI Model#Transport|Transport]] layer as well
	- When this occurs it is known as a [[#TCP/IP Hijacking]]

```ad-example
title: Session Theft
collapse:close
![[SessionTheftEx1.png]]
```

# TCP/IP Hijacking
---
- Occurs when an attacker takes over a TCP session between two computers without the need of a cookie or other host access ^440dd1
- [[#Session Theft/Session Hijacking]] at the [[The OSI Model#Network|Network]] or [[The OSI Model#Transport|Transport]] layer
- <u>TCP only authenticates during the first handshake</u>
- An attacker can guess the next number in a sequence and 'jump in'
- Can be a form of a [[Denial of Service (DoS)]] against the initial host because it can deny or interrupt access to that server/session

# Blind Hijacking
---
- Occurs when an attacker blindly injects data into the communication stream <u>without being able to see if it is successful</u> or not ^cabfa5

# Clickjacking
---
- Attack that uses multiple transparent layers to trick a user into clicking on a button or link on a page when they were intending to click on the actual page ^32a417
- Hyperlink to malicious site
- Example
	- Clicking on image with a link but it actually redirects to a malicious site

# Man-in-the-Middle (MITM)
---
- An attack that causes data to flow through the attacker's computer where they can then intercept or manipulate data ^29aba5
- [[#Session Theft/Session Hijacking]] uses this method
- Considered a form of [[Active Intercept & Privilege Escalation|Active Interception]]
- See also
	- [[Authentication Attacks#Main in the Middle Attack]]

# Man-in-the-Browser (MITB)
---
- Occurs when a [[Trojans|Trojan]] infects a vulnerable web browser and modifies the webpages or transactions being done within the browser ^72701b
- New term is "On-path attack" 
- To prevent
	- [[Endpoint Analysis#AntiVirus (AV)|AntiVirus (AV)]]
	- [[Updates and Patches]] installed
- See also
	- [[Web Browser Security]]
	- [[Web Browser Concerns]]
	- [[Web Browser Security#Which Browser?]]
	- [[Security of Apps#Browser]]
	- [[Authentication Attacks#Man-in-the-Browser]]

# Watering Hole
---
![[Common Delivery Methods#^740c18]]
- Can be modified to allow for [[#Session Theft/Session Hijacking]] because an attacker can take over a website
- See also
	- [[Common Delivery Methods#Watering hole]]

# Cross-site scripting (XSS)
---
![[XSS and XSRF#^81f3ff]]
- Can be used for [[#Session Theft/Session Hijacking]]
- Trick client into thinking code came from a trusted place
- See also
	- [[XSS and XSRF]]

# Objectives
---
- [[Objectives#1.3 - Given a scenario, analyze potential indicators associated with application attacks|1.3 - Given a scenario, analyze potential indicators associated with application attacks]]
- [[Objectives#1.4 - Given a scenario, analyze potential indicators associated with network attacks|1.4 - Given a scenario, analyze potential indicators associated with network attacks]]