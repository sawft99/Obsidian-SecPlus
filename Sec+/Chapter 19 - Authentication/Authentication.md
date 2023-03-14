---
tags: [CompTia,SecPlus,CyberSec,Certs]
#aliases:
#cssclass:
#publish:
---

# About
---
- See also
	- [[SecBasics#^45fffd|AAA Model]]

# Multi-Factor Authentication

## About
---
- Use of two or more authentication [[#Factors]] to prove a users identity ^a8671c
- Studies show MFA is far more secure than just increasing the password complexity
- AKA "Dual-Factor Authentication
- Example
	- A smart card that asks for a PIN
	- This represents something a user has "Ownership" of (Smart Card) and something a user has "Knowledge" of (The PIN) 

## Factors
---
- Knowledge
	- Piece of memorized info about the user
	- Password, Social Security Number, Birthday
- Ownership
	- Proving a user has something in their possession that uniquely identifies them
	- Passport, Drivers license, Token Devices Smart Card, Random Number Generator on Cell Phone
- Characteristics
	- Something that the user is
	- [[Biometric Readers|Biometrics]] like fingerprint, face shape, or IRIS, speech pattern recognition
- Location
	- Where a user is at when trying to log in
	- An Authentication system may monitor a users login habits and flag a login attempt if it is somewhere outside a certain area or a users typical area
		- Often this may then trigger a prompt for a [[#Multi-Factor Authentication]]
	- Other methods include accessing a cell phones [[Other Wireless Technologies#Global Positioning System (GPS)|GPS]] or an IP address of a device
- Action
	- Something a user does
	- How a user performs something
	- The way a user signs a signature or draws a picture

# Single-Factor Authentication

## About
---
- If you are only using a single Username and Password combo
- You may be able to ask for an additional piece of information, but if it is of the same type it is considered single-factor
- Example
	- Username and password combo is two pieces of information, but they are both from the "Knowledge" factor so this is considered single factor

# One-Time Passwords

## About
---
- [[#Time-Based One-Time Password (TOTP)]] or hash based

## Time-Based One-Time Password (TOTP)
---
- A password is computed from a shared secret and current time
- Common in an RSA fob

```ad-example
title: RSA Fob
collapse:close
![[RSAFobEx1.png]]
![[RSAFobEx2.png]]
```

## HMAC-Based One-Time Password (HOTP)
---
- A password is computed from a secret and is synchronized between the client and server
- Each time a password is entered to log in a new password is created

# Objectives
---
- [[Objectives#2.4 - Summarize authentication and authorization design concepts|2.4 - Summarize authentication and authorization design concepts]]
- [[Objectives#3.5 - Given a scenario, implement secure mobile solutions|3.5 - Given a scenario, implement secure mobile solutions]]
- [[Objectives#3.8 - Given a scenario, implement authentication and authorization solutions|3.8 - Given a scenario, implement authentication and authorization solutions]]

# TODO (Delete when done)
---
- [ ] Added vocab
- [ ] Added and linked objectives in document
- [ ] Linked objectives back to document
- [ ] Linked any relevant backlinks to and from document