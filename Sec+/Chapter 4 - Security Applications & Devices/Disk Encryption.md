---
tags: [CompTia,SecPlus,CyberSec,Certs]
#aliases:
#cssclass:
#publish:
---

# About
---
- [[Securing Storage#Encryption|Encryption]] scrambles data into an unreadable format
- This way no one can read it except for those that have the "secret key"
	- With the key you are able to unlock/unscramble the data into something readable
- Helps ensure [[SecBasics#Cybersecurity Models|Confidentiality]]
- Will lead to lower performance
- There is [[#Full Disk Encryption]] and [[#File Level Encryption]]

# Full Disk Encryption

## Hardware Based
---
- Storage device that performs <u>whole disk</u> [[Securing Storage#Encryption|Encryption]] by using the <u>embedded hardware</u> ^abe3d2
- Faster than [[#Software Based]]
- <u>Self encrypting Drive</u> (SED)
	- Looks like an external hard drive
	- Because it is hardware based it is very fast
	- Also very expensive and therefore not as common vs [[#Software Based]] solutions
- <u>Hardware Security Module</u> (HSM) ^5ffc2c
	- Physical drive that acts as a secure crypto processor during the [[Securing Storage#Encryption|Encryption]] process or digital signing
	- Typically an adapter card over USB or a networked device
	- Usually tamper proof with high levels of security
	- Also very expensive and less common vs [[#Software Based]]

## Software Based
---
- Mac and #OSX  have FileVault built in
	- Slower than [[#Hardware Based]]
	- Whole disk [[Securing Storage#Encryption|Encryption]]
	- "System preferences > Security"
	- Supports [[#Advanced Encryption Standard (AES)]] 128 and 256
- Windows has #Bitlocker built in
	- Whole disk [[Securing Storage#Encryption|Encryption]]
	- "Right click a drive > turn on #Bitlocker"
	- Supports [[#Advanced Encryption Standard (AES)]] 128 and 256
- <u>Most companies use this</u>

# File Level Encryption
---
- Enable encryption on <u>individual files and folders</u>
- Windows
	- Encrypting File System (EFS) ^973f7f
		- Can right click and enable on a folder
		- Will make it so only that user is able to see/access

# #Bitlocker Methods
---
- Can use a [[#Trusted Platform Module (TPM)]] chip
- If you do not have a [[#Trusted Platform Module (TPM)]] chip you can use an external USB drive as a key
	- If you lose the USB drive you can not decrypt your drive

# Trusted Platform Module (TPM)
---
- Chip residing on the motherboard that contains an [[Securing Storage#Encryption|Encryption]]  key
- #Bitlocker  will use the key already inside the TPM chip for its [[Securing Storage#Encryption|Encryption]] operation
- If you take the hard drive out and put it into another computer you would not be able to read it because that computer has a different TPM chip with a different key on it

# Advanced Encryption Standard (AES)
---
- Symmetric key encryption
- 128 or 256 bit keys
	- 256 "Unbreakable"

# [[Objectives]]
---
- [[Objectives#2.1 - Explain the importance of security concepts in an enterprise environment|2.1 - Explain the importance of security concepts in an enterprise environment]]
- [[Objectives#2.8 - Summarize the basics of cryptographic concepts||2.8 - Summarize the basics of cryptographic concepts|]]
- [[Objectives#3.2 - Given a scenario, implement host or application security solutions|3.2 - Given a scenario, implement host or application security solutions]]