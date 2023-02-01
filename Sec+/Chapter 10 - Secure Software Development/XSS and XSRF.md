---
tags: [CompTia,SecPlus,CyberSec,Certs]
#aliases:
#cssclass:
#publish:
---

# About
---
- These are web app vulnerabilities
- Usually trying to get [[Threats to VMs#Privilege Elevation|Privilege Elevation]] , steal info from victims [[Web Browser Concerns#Cookies|Cookies]], or get other information stored by the victims [[Security of Apps#Browser|Browser]]
- [[#Cross Site Scripting (XSS)]]
	- Occurs when an <u>attacker embeds</u> malicious scripting commands onto a trusted website ^18a429
- [[#Cross Site Request Forgery (XSRF/CSRF)]]
	- Occurs when an attacker <u>forces a user to execute</u> actions on a web server for which they are already authenticated ^eea3e5

# Cross Site Scripting (XSS)

## About
---
- Victim is the <u>user NOT the server</u>
	- Server may or may not already be compromised
- Exploits focus on <u>trust between user and the server they visit</u> ^2512a1
- Attacker is able to insert code into the webpage that's being delivered from the server to the victim/client
	- This code (often JavaScript) is usually injected from a separate “attack site”
	- Can also manifest itself as an embedded JavaScript image tag, header manipulation (as in manipulated HTTP response headers), or other HTML-embedded image object within emails
- Multiple types: [[#Stored/Persistent]], [[#Reflected]], [[#DOM-Based]]

## Stored/Persistent
---
- Attempts to get data provided by the attacker to be saved on the web server by the victim
- Activated by #UserAction on the web site

## Reflected
---
- Attempts to have a <u>non-persistent</u> effect activated by a victims #UserAction by clicking a link on the website

## DOM-Based
---
- Attempts to exploit the [[Security of Apps#Browser|Browser]] itself
- Comes from the Document Object Model (DOM) being vulnerable to attack
	- DOM is part of a users [[Security of Apps#Browser|Browser]]
- AKA "Client Side Cross Site Scripting" attack

## Prevention
---
- Use <u>output encoding</u> to prevent <u>code injection</u> during delivery of content
- Use [[SDLC Principles#Never Trust User Input|Input Validation]] to stop HTML tags from being entered by users when entering information on a web form
- A user can increase security setting for [[Web Browser Concerns#Cookies|Cookies]] and [[Web Browser Concerns#Configuring the Browser - Examples|disabling scripting]] for websites
- [[Firewalls#Web Application Firewall (WAF)|Web Application Firewall (WAF)]]
- [[Cloud Threats#^34f55a|Cross Origin Sharing Policy (CORS)]] Policy

# Cross Site Request Forgery (XSRF/CSRF)

## About
---
- Exploits focus on <u>the trust a website has in a user</u> ^09a7b3
- Example
	- Once logged into bank account the website "trusts" you
	- Attacker sends a command to web server via your [[SecBasics#^45fffd|authenticated]] session
	- Forges request to <u>make it look like it came from the victim</u>
	- An attacker usually can't see the web server response but it could still could be used to do some functions on the site like change a password or transfer money

## Prevention
---
- Require specialized tokens on web pages that have forms like CAPTCHA
- Use good authentication and [[Disk Encryption#^501400|Encryption]] techniques
- Scan XML files submitted by a user
- Submit [[Web Browser Concerns#Cookies|Cookies]] twice to make sure they both match and have the proper [[SecBasics#^51b6d8|Integrity]]
- [[Firewalls#Web Application Firewall (WAF)|Web Application Firewall (WAF)]]
- [[Cloud Threats#^34f55a|Cross Origin Sharing Policy (CORS)]] Policy

```ad-tip
title: Exam Tip - XSS vs XSRF/CSRF
collapse: close
- XSS ![[XSS and XSRF#^18a429]] ![[XSS and XSRF#^2512a1]]
- XSRF/CSRF ![[XSS and XSRF#^eea3e5]] ![[XSS and XSRF#^09a7b3]]
```

# Objectives
---
- [[Objectives#1.3 - Given a scenario, analyze potential indicators associated with application attacks|1.3 - Given a scenario, analyze potential indicators associated with application attacks]]