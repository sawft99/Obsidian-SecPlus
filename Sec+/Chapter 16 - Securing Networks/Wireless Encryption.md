---
tags: [CompTia,SecPlus,CyberSec,Certs]
#aliases:
#cssclass:
#publish:
---

# About
---
- Encryption type you use can make a large difference in security
- Types
	- [[#Wired Equivalent Privacy (WEP)]]
	- [[#WIFI Protected Access (WPA)]]
	- [[#WIFI Protected Access version 2 (WPA2)]]
- See also
	- [[Securing WIFI Devices]] 
	- [[Securing Wireless Devices]]

# Pre-Shared Key (PSK)
---
- Same encryption key is used by the access point and the client to encrypt and decrypt the data ^07c2c5
- Not [[Virtualization#^a6ee8d|Elastic]]
- Have to share a password with many people making distribution hard
- Everyone is also using the same key

# Wireless Encryption Types

## Wired Equivalent Privacy (WEP)
---
- Original 802.11 wireless security standard that claims to be as secure as a wired network ^556421
- Encryption key changed over time originally starting with a 40 bit [[#Pre-Shared Key (PSK)]], then 64 bit, and then 128 bit
- Main flaw however is in the 24 bit Initialization Vector (IV) which is sent in clear text to establish the connection
- Superseded by [[#WIFI Protected Access (WPA)]]
  
## WIFI Protected Access (WPA)
---
- Replacement for [[#Wired Equivalent Privacy (WEP)]] which uses Temporal Key Integrity Protocol (TKIP), Message Integrity Check (MIC), and RC4 encryption ^118526
- Secures data and makes sure it is not modified
- Had some flaws and was superseded by [[#WIFI Protected Access version 2 (WPA2)]]

## WIFI Protected Access version 2 (WPA2)
---
- 802.11i standard to provide better wireless security featuring [[Disk Encryption#Advanced Encryption Standard (AES)|AES]] with s 128-bit key, Counter Mode with Cipher Block Chaining Message Authentication Protocol ( CCMP), and integrity checking ^36aaad
- Uses [[#Pre-Shared Key (PSK)]] or Enterprise mode with [[RADIUS vs TACAS+|RADIUS]]

```ad-tip
title: Exam Tip
collapse: close
![[WifiExamTip1.png]]
```

# WIFI Protected Setup (WPS)

## About
---
- Automated encryption setup for wireless networks at a push of a button ^4cc0b1
- Has severe flaws and vulnerabilities
- <u>Convenient but very insecure</u>
- You join with an 8 digit pin
- Packet is broken into 2 4 digit chunks
	- Easy to brute force 

## Prevention
---
- DISABLE!

# Virtual Private Network (VPN)

## About
---
- Always use on WIFI even if it is your own
- Don't trust WIFI!
- Encryption inside of encryption
- See also
	- [[Virtual Private Network (VPN)]]

```ad-tip
title: Exam Tip
collapse: close
"Encryption" and "VPN" are almost never the wrong answer to a question
```

# Objectives
---
- [[Objectives#1.6 - Explain the security concerns associated with various types of vulnerabilities|1.6 - Explain the security concerns associated with various types of vulnerabilities]]
- [[Objectives#3.4 - Given a scenario, install and configure wireless security settings]|3.4 - Given a scenario, install and configure wireless security settings]]