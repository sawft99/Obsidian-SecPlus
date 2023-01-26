---
tags: [CompTia,SecPlus,CyberSec,Certs]
#aliases:
#cssclass:
#publish:
---

# About
---
- Gateway to the internet with all of its abilities and risks
- Web apps are more common now instead of full apps
	- Cross platform and better [[SecBasics#^51b6d8|Availability]]
	- Faster deployment
	- Relies on a browser
	- Browser security is more important in particular if your company uses web apps

# Mitigating
---
- Make sure it has the latest [[Updates and Patches]]
- <u>HOWEVER</u> don't always be the first to download a new version of a browser such as "2.0"
	- Let others figure out issue first
	- You should still be working in a stable and secure [[Supply Chain Assessment#Trusted Computing Environment|Trusted Computing Environment]]

# Updating Methods
---
- Home users will usually use something such as #Windows update or in app updates
- In a corporate environment you should have a [[Patch Management]] system where you test and then deploy further

# Which Browser?
---
- Based on <u>needs of organizations, sites used, OS used</u>, or just preference
	- Can't get IE on #OSX
	- Can't get Safari on #Linux
	- Whatever your company officially supports
- Chrome is arguably the best because it is cross platform, gets frequent [[Updates and Patches]], and is relatively fast

# General Security for Browsers
---
1. Implement good policies
	1. Create and implement web browsing policies such as [[SecBasics#^50e62d|Administrative controls]] and [[SecBasics#^c5223f|Technical controls]]
	2. Such as written policy or [[Group Policies]]
2.  User training
	1. Show users how to go to 'https' version of a site
	2. Close browser with keys instead of mouse
	3. Other safe browsing apps
3. [[Proxy Servers]] and [[Proxy Servers#Content Filter|Content Filters]]]
	1. Proxies cache a website to reduce requests, bandwidth usage, and potentially hide the source of a request ^0799dc
	2. A [[Proxy Servers#Content Filter|Content Filter]] can blacklist specific websites or by entire categories such as "Gambling" websites
4. Prevent malicious code
	1. Configure your browser to prevent ActiveX, Java applets, Flash, and other active content from downloading and running
	2. Do so with controls in browser

# Objectives
---
- [[Objectives#3.2 - Given a scenario, implement host or application security solutions|3.2 - Given a scenario, implement host or application security solutions]]
- [[Objectives#3.3 - Given a scenario, implement secure network designs|3.3 - Given a scenario, implement secure network designs]]