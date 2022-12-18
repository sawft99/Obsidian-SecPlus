---
tags: [CompTia,SecPlus,CyberSec,Certs]
#aliases:
#cssclass:
#publish:
---

# About
---
- Hardware Root of Trust (ROT) ^f30681
	- A cryptographic module embedded in a computer system that can endorse trusted execution and attest to boot settings and metrics
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

```ad-tip
title: The main idea
collapse: close
Understand that [[Disk Encryption#Trusted Platform Module (TPM)|Trusted Platform Module (TPM)]] verifies a secure boot and provides a digital report
```

```ad-info
title: TPM Design
collapse:close
![[TPM_Design.png]]
```

## Management
---
- Can be done via
	- tpm.msc
	- [[Group Policies]]

# Hardware Security Module (HSM)
---
- An appliance for generating and storing cryptographic keys that is less susceptible to tampering and insider threats than software based storage
- A long key could still be compromised
- Types
	- PCI card
	- Rack mount
	- #IOT
- All can be automated
- Remove human element
- See also [[Disk Encryption#^5ffc2c|Disk Encryption]]

# Objectives
---
- Obj

# TODO (Delete when done)
---
- [ ] Added vocab
- [ ] Added and linked objectives in document
- [ ] Linked objectives back to document
- [ ] Linked any relevant backlinks to and from document