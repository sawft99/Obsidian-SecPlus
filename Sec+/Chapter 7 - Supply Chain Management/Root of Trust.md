---
tags: [CompTia,SecPlus,CyberSec,Certs]
#aliases:
#cssclass:
#publish:
---

# About
---
- Hardware Root of Trust (ROT) ^f30681
	- A cryptographic module embedded in a computer system that can endorse trusted execution and [[Trusted Firmware#Attestation|Attestation]] to boot settings and metrics
	- Used to scan the boot metrics and OS files to verify their signatures, which can then be used to sign a digital report (certificate)

# TPM Expanded

## About
---
- Components
	- Secure I/O
	- Cryptographic processor
		- Random Number Generator (RNG)
		- RSA Key Generator
		- SHA-1 hash generator
		- [[Disk Encryption#^501400|Encryption]]/Decryption signature engine
	- Persistent Memory
		- Endorsement Key (EK)
		- Storage Root Key (SRK)
	- Versatile Memory
		- Platform Configuration Registers (PCR)
		- Attestation Identity Keys (AIK)
		- Storage Keys
	- #Bitlocker and other [[Disk Encryption#Full Disk Encryption|Full Disk Encryption]] technology can utilize [[Disk Encryption#Trusted Platform Module (TPM)|Trusted Platform Module (TPM)]]
- See also [[Disk Encryption#Trusted Platform Module (TPM)|Trusted Platform Module (TPM)]]

```ad-info
title: TPM Design
collapse:close
![[TPM_Design.png]]
```


```ad-tip
title: The main idea
collapse: close
Understand that [[Disk Encryption#Trusted Platform Module (TPM)|Trusted Platform Module (TPM)]] verifies a [[Trusted Firmware#Secure Boot|Secure Boot]] and provides a digital report
```

## Management
---
- Can be done via
	- tpm.msc
	- [[Group Policies]]

# Hardware Security Module (HSM)
---
- An <u>appliance for generating and storing cryptographic keys</u> that is less susceptible to tampering and insider threats than software based storage
- A long key could still be compromised
- Types
	- PCI card
	- Rack mount
	- #IOT
- All can be automated
	- Remove human element so it can not be compromised by a person
- See also [[Disk Encryption#Hardware Based|Disk Encryption]]

# Tampering
---
- Anti-Tamper
	- Method that makes it difficult for an attacker to alter the authorized execution of software ^e22ab4
- Mechanisms
	- Mechanisms include a Field Programable Gate Array (FPGA) and a Physically Unencodable Function (PUF)
		- Zeros out cryptographic key

# Objectives
---
- [[Objectives#3.2 - Given a scenario, implement host or application security solutions|3.2 - Given a scenario, implement host or application security solutions]]