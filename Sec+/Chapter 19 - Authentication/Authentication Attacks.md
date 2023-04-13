---
tags: [CompTia,SecPlus,CyberSec,Certs]
#aliases:
#cssclass:
#publish:
---

# About
---
- Various types of attacks exist
	- [[#Spoofing]]
	- [[#Man-in-the-Middle Attack]]
	- [[#Man-in-the-Browser Attack]]
	- [[#Online Password Attacks]]
		- [[#Password Spraying]]
		- [[#Credential Stuffing]]
	- [[#Offline Password Attacks]]
		- [[#Rainbow Tables]]
	- [[#Broken Authentication]]
- See also
	- [[Authentication]]

# Spoofing
---
- A software-based attack where the goal is to assume the [[Identity]] of a user, process, address, or other unique identifier

# Man-in-the-Middle Attack
---
![[Hijacking#^29aba5]]
- Common in [[Wireless Attacks]]
- See also
	- [[Hijacking#Man-in-the-Middle (MITM)]]

# Man-in-the-Browser Attack
---
![[Hijacking#^72701b]]
- Intercepts [[Application Programming Interface (API)|API]] calls between the browser process and its [[Rootkits#DLL Injection|DLLs]]
- See also
	- [[Hijacking#Man-in-the-Browser (MITB)]]

# Passwords
---
- When storing passwords you don't store the password in plaintext
- Instead the password goes through some form of #Hashing and that value is then saved
- In theory even the administrators can't know the password since you can't reverse a hash
- See also
	- [[Usernames & Passwords]]

# Online Password Attacks
---
- Someone guessing and entering [[#Passwords]] directly into <u>a single site or service</u> ^5e4337
- Sitting at the login screen for a site or service
- Inefficient
- Preventions
	- Rate limiting such as limiting to 3 bad password attempts locking the account or putting a delay on it to stop any more attempts for a set amount of time

```ad-example
title: Signs
collapse:close
![[PasswordGuessEx1.png]]
```

## Password Spraying
---
- A form of [[#Online Password Attacks]] and a [[Wireless Attacks#Brute Force|Brute Force]] attack in which multiple user accounts are tested with a <u>dictionary</u> of common [[#Passwords]] against <u>multiple websites</u> ^f399b3

```ad-example
title: Signs
collapse:close
![[PasswordGuessEx2.png]]
```

## Credential Stuffing
---
- Similar to [[#Password Spraying]] but instead tests <u>stolen user account</u> names and [[#Passwords]] against <u>multiple websites</u> ^6ecb13
- Prevention
	- Don't reuse passwords

# Offline Password Attacks

## About
---
- Attacker already has a list of credentials, but typically in hash form, and is able to attempt to crack the passwords on their own system without interacting with the website ^f13624

## Rainbow Tables
---
- A form of [[#Offline Password Attacks]] where an attacker has a precomputed table of already hashed [[#Passwords]] ^0739c5
- Prevention
	- Salting passwords
		- The generation of random data that is used as an additional input to a one-way function that hashes data, a password, or a passphrase ^0f06de

```ad-example
title: Rainbow Table
collapse:close
![[RainbowTableEx1.png]]
```

```ad-example
title: Salting
collapse:close
![[SaltEx1.png]]
```

# Broken Authentication
---
- A software vulnerability where the [[Authentication]] mechanism allows an attacker to gain entry ^8c266a
- Bad programming or [[Design Vulnerabilities]]
	- Cleartext password, reusing tokens, permitting [[Wireless Attacks#Brute Force|Brute Force]] attacks
	- Credential exposure
		- Exposes tokens or credentials in the code allowing for a [[#Man-in-the-Middle Attack]]
		- Hard coded credentials in code
	- Lack of or weak [[Disk Encryption#^501400|Encryption]]
	- Weak session keys
		- Allows for possible [[Hijacking#Session Theft/Session Hijacking|Session Theft/Session Hijacking]]
- Bad policy
	- Limiting password strength or complexity
	- Weak reset methods
		- Knowledge factors that can be looked up such as Date of Birth or current state you live in

# Objectives
---
- [[Objectives#1.2 - Given a scenario, analyze potential indicators to determine the type of attack|1.2 - Given a scenario, analyze potential indicators to determine the type of attack]]