---
tags: [CompTia,SecPlus,CyberSec,Certs]
#aliases:
#cssclass:
#publish:
---

# About
---
- Improvements to [[Wireless Encryption#WIFI Protected Access version 2 (WPA2)|WIFI Protected Access version 2 (WPA2)]]
- Two modes
	- [[#WPA3 - Enterprise Mode]]
	- [[#WPA3 - Personal Mode]]

# WPA3 - Enterprise Mode
---
- Uses [[Disk Encryption#Advanced Encryption Standard (AES)|AES]] 256 encryption with SHA384 hash integrity checking
- Has cryptographic strength of 192 bits <u>in Enterprise Mode</u>
	- Vs 128 bit key in [[Wireless Encryption#WIFI Protected Access version 2 (WPA2)|WIFI Protected Access version 2 (WPA2)]]

# WPA3 - Personal Mode
---
- Uses CCMP-128 as the minimum [[Disk Encryption#^501400|Encryption]] required for secure connectivity
- Can go higher depending on manufacturer and model

# Simultaneous Authentication of Equals (SAE)
---
- A secure password-based [[SecBasics#^45fffd|Authentication]] and password-authenticated key agreement method 
- Replaces [[Wireless Encryption#Pre-Shared Key (PSK)|Pre-Shared Key (PSK)]] used in [[Wireless Encryption#WIFI Protected Access version 2 (WPA2)|WIFI Protected Access version 2 (WPA2)]]

# Forward Secrecy

## About
---
- A feature of key agreement protocols, like [[#Simultaneous Authentication of Equals (SAE)]], that provides assurance that session keys will not be compromised even if long term secrets used in the session key exchange are compromised
- In short, if someone gets the password that you use for your network they can not use it to decrypt previously captured traffic or other sessions on the same network
- Sometimes also called "Perfect Forward Secrecy"

## Steps
---
1. [[Wireless Access Points (WAP)]] and the client use a public key system to generate a pair of long term keys
2. The [[Wireless Access Points (WAP)]] and the client exchange a one time uses session key using a secure algorithm like Diffie-Hellman
	1. Rather than a [[Wireless Encryption#Pre-Shared Key (PSK)|Pre-Shared Key (PSK)]] where they key is directly derived from the password, the [[Wireless Access Points (WAP)]] will generate a random number for the session established
	2. A new session key is generated every time the client connects to the [[Wireless Access Points (WAP)]] which is why only having the password will not allow you to read previous traffic or other clients connected to the same [[Wireless Access Points (WAP)]] or network
3. The AP sends client messages and encrypts them using the session key created in session 2
4. Client decrypts the message received using the same one time use session key
5. The process repeats for every message being sent, starting at step 2 to ensure forward secrecy 

# Videos

## Forward Secrecy
---
![](https://www.youtube.com/watch?v=IkM3R-KDu44)

# Objectives
---
- [[Objectives#3.4 - Given a scenario, install and configure wireless security settings|3.4 - Given a scenario, install and configure wireless security settings]]]

# TODO (Delete when done)
---
- [ ] Added vocab
- [ ] Added and linked objectives in document
- [ ] Linked objectives back to document
- [ ] Linked any relevant backlinks to and from document