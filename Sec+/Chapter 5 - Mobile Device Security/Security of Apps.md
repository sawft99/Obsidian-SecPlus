---
tags: [CompTia,SecPlus,CyberSec,Certs]
#aliases:
#cssclass:
#publish:
---

# About
---
- Only install apps from official mobile stores
	- #Android using Google Play Store
	- #IPhone using App Store

# Jailbreaking & Rooting
---
- Jailbreaking ^b2238c
	- Used on #IPhone
	- Remove security protection Apple put in place in order to take it to other carriers or install 3rd party apps
	- See also [[Mobile Malware]]
- Rooting ^6f9cfd
	- Used on #Android
		- Is #Linux at heart
	- Can install apps you want and make phone do things it's not designed to do
	- See also [[Mobile Malware]]

# Browser
---
- Mainstream browsers such as Chrome are well known and trusted
- Can't be sure what is in the application for 3rd party apps
- <u>Always go to Https version of a site when possible</u> so you are using [[#^9255c3|TLS]]

# Enterprise Mobility

## Mobile Device Management (MDM)
---
- <u>Centralized software solution</u> that allows system administrators to create and enforce <u>policies</u> across its mobile devices ^c3e684
- Example
	- Stop people from installing 3rd party apps or block specific websites

## Location Access
---
- Phones have GPS location abilities
- Should consider if location is needed for an app to function or not
	- <u>Turn of location services if the app does not need it</u>

## Geotagging
---
- <u>Embedding of the GPS coordinates</u> in a piece of data such as a photo/video ^463b9f
- #IPhone will automatically embed this information into pictures and videos
- Attackers can abuse this information to gather #Intelligence on a person or group
- Example
	- Manager visits a coffee shop every morning and posts a picture to social media
	- Attackers learn manager is not in office
	- Manager could be targeted at coffee shop or attackers could target someone/something else in the office more easily because the manager is not present
- Needs to be considered when developing organizations security policy
	- <u>Recommended to turn off if not needed</u>

# Vocab
---
- TLS
	- Encrypts connection and tunnel between you and the server to ensure [[SecBasics#Cybersecurity Models|Confidentiality]] and no #MITM attacks ^9255c3

# Objectives
---
- [[Objectives#3.1 - Given a scenario, implement secure protocols|3.1 - Given a scenario, implement secure protocols]]
- [[Objectives#3.5 - Given a scenario, implement secure mobile solutions|3.5 - Given a scenario, implement secure mobile solutions]]