---
tags: [CompTia,SecPlus,CyberSec,Certs]
#aliases:
#cssclass:
#publish:
---

# About
---
- Types of attacks
	- 
- See also
	- [[Securing Wireless Devices]]
	- [[Securing WIFI Devices]]
	- [[Wireless Encryption]]

# War Driving
---
- Act of searching for wireless networks by driving around until you find them ^ff67de
- Can be for the purpose to attack your network or others
	- Using your network as a source to trace back to you rather than them

# War Chalking
---
- Act of physically drawing symbols in public places to denote the open, closed, and protected networks in range ^03ad7c
- Open network
	- )( with SSID above and Bandwidth below
- Closed
	- Full circle with SSID above and bandwidth below
	- If the password is known the SSID is in the top left and the password is in the top right
	- Type of encryption in center of circle some times

```ad-example
title: War Chalking Symbols
collapse:close
![[WarChalkEx1.png]]
```

# IV Attack

## About
---
- Occurs when an attacker observes the operation of a cipher being used with several different keys and finds a mathematical relationship between those keys to determine the clear text data ^d6d994
- This was primarily an issue with [[Wireless Encryption#Wired Equivalent Privacy (WEP)|Wired Equivalent Privacy (WEP)]]

# WIFI Disassociation Attack
---
- Attack that targets an individual client connected to a network, forces it offline by deauthenticating it, and then captures the handshake when it reconnects ^bd2d68
- Part of an attack against [[Wireless Encryption#WIFI Protected Access (WPA)|WIFI Protected Access (WPA)]] and [[Wireless Encryption#WIFI Protected Access version 2 (WPA2)|WIFI Protected Access version 2 (WPA2)]]

# Brute Force
---
- Occurs when an attacker continually guesses a password until the correct one is found ^db660c
- Brute force will always find the password.... eventually
- The longer and more complex the password the longer it will take
- Don't have [[Securing Network Devices#^4c4d3e|Weak Passwords]]
- See aslo
	- [[Password Analysis#Brute Force Attack]]

# Videos

## WEP Crack Demo
---
![](https://www.youtube.com/watch?v=NhnoDS3jtyQ)

# Objectives
---
- [[Objectives#1.2 - Given a scenario, analyze potential indicators to determine the type of attack|1.2 - Given a scenario, analyze potential indicators to determine the type of attack]]
- [[Objectives#1.4 - Given a scenario, analyze potential indicators associated with network attacks|1.4 - Given a scenario, analyze potential indicators associated with network attacks]]
- [[Objectives#1.8 - Explain the techniques used in penetration testing|1.8 - Explain the techniques used in penetration testing]]