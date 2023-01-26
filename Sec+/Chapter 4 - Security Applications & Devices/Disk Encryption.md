---
tags: [CompTia,SecPlus,CyberSec,Certs]
#aliases:
#cssclass:
#publish:
---

# About
---
- Encryption <u>scrambles data into an unreadable format</u> ^501400
- This way no one can read it except for those that have the "secret key"
	- With the key you are able to unlock/unscramble the data into something readable
- Helps ensure [[SecBasics#Cybersecurity Models|Confidentiality]]
- Will lead to lower performance
- There is [[#Full Disk Encryption]] and [[#File Level Encryption]]

# Full Disk Encryption

## Hardware Based
---
- <u>Faster</u> than [[#Software Based]]
- <u>Self encrypting Drive</u> (SED)
	- <u>Storage device</u> that performs <u>whole disk</u> [[#^501400|Encryption]] by using the <u>embedded hardware</u> ^abe3d2
	- Looks like an external hard drive
	- Also very expensive and therefore not as common vs [[#Software Based]]
- <u>Hardware Security Module</u> (HSM)
	- <u>Physical device</u> that acts as a <u>secure crypto processor</u> during the [[#^501400|Encryption]] process or digital signing ^5ffc2c
	- Typically an adapter card over USB or a networked device
	- Usually tamper proof with high levels of security
	- Also very expensive and less common vs [[#Software Based]]
- See also [[Root of Trust#Hardware Security Module (HSM)|Root of Trust]]and [[Trusted Firmware#Self-Encrypting Drives|Self-Encrypting Drives]]

## Software Based
---
- Mac and #OSX have #FileVault [[Endpoint Analysis#AntiVirus (AV)|AntiVirus (AV)]]built in
	- Slower than [[#Hardware Based]]
	- [[#Full Disk Encryption]]
	- "System preferences > Security"
	- Supports [[#Advanced Encryption Standard (AES)]] 128 and 256
- Windows has #Bitlocker built in
	- [[#Full Disk Encryption]]
	- "Right click a drive > turn on #Bitlocker"
	- Supports [[#Advanced Encryption Standard (AES)]] 128 and 256 bit
- <u>Most companies use software based</u>

# File Level Encryption
---
- Enable encryption on <u>individual files and folders</u>
- Encrypting File System (EFS) ^973f7f
	- #Windows option
	- Can right click and enable on a folder
	- Will make it so only that user is able to see/access

# #Bitlocker Methods
---
- Can use a [[#Trusted Platform Module (TPM)]] chip
- If you do not have a [[#Trusted Platform Module (TPM)]] chip you <u>can use an external USB drive</u> as a key instead
	- If you lose the USB drive you can not decrypt your drive

# Trusted Platform Module (TPM)
---
- Chip residing on the motherboard that contains an [[#^501400|Encryption]] key
- A specification for hardware based storage of digital certificates, keys, #Hashing (hashed) passwords, and other user and platform identification information ^e5cd31
- Also used for [[Root of Trust]]
- #Bitlocker will use the key already inside the TPM chip for its [[#^501400|Encryption]] operation
- If you take the hard drive out and put it into another computer you would not be able to read it because that computer has a different TPM chip with a different key on it
- See also [[Root of Trust]] and [[Trusted Firmware]]

# Advanced Encryption Standard (AES)
---
- A type of <u>symmetric</u> key encryption ^dccf53
- Common in WIFI
- 128 or 256 bit keys
	- 256 considered "Unbreakable"

# Objectives
---
- [[Objectives#2.1 - Explain the importance of security concepts in an enterprise environment|2.1 - Explain the importance of security concepts in an enterprise environment]]
- [[Objectives#2.8 - Summarize the basics of cryptographic concepts||2.8 - Summarize the basics of cryptographic concepts|]]
- [[Objectives#3.2 - Given a scenario, implement host or application security solutions|3.2 - Given a scenario, implement host or application security solutions]]
- [[Objectives#3.3 - Given a scenario, implement secure network designs|3.3 - Given a scenario, implement secure network designs]]