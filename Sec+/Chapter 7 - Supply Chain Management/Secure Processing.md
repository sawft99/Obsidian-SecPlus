---
tags: [CompTia,SecPlus,CyberSec,Certs]
#aliases:
#cssclass:
#publish:
---

# About
---
- A mechanism to ensure [[SecBasics#^51b6d8|Confidentiality, Integrity, and Availability]] of software code and data as its executed in volatile memory
- Data goes from hard drive to RAM and from RAM to CPU
	- Potential along the way for data to be altered or stolen

# [[Hardening]] Mechanisms

## Processor Security Extensions (PSE)
---
- Low level CPU changes and instructions that enable secure processing
- Labeled differently across some brands
	- #AMD
		- Secure Memory Encryption (SME)
		- Secure Encrypted Virtualization (SEV)
	- #Intel 
		- Trusted Execution Technology (TXT)
		- Software Guard Extension (SGX)

## Trusted Execution
---
- The [[#Processor Security Extensions (PSE)]] invoke the [[Disk Encryption#Trusted Platform Module (TPM)|Trusted Platform Module (TPM)]] chip and [[Trusted Firmware#Secure Boot|Secure Boot]] [[Trusted Firmware#Attestation|Attestation]] to ensure that a [[Trusted Operating System]] is running
- When you boot the system want to use[[Trusted Firmware]], [[Trusted Firmware#UEFI|UEFI]], [[Root of Trust#TPM Expanded|TPM]] and [[Trusted Firmware#Secure Boot|Secure Boot]]
- Common to #Microsoft when installing #Windows on #AMD and #Intel hardware

## Secure Enclave
---

## Atomic Execution
---

## Bus Encryption
---

# Objectives
---
- [[Objectives#3.2 - Given a scenario, implement host or application security solutions|3.2 - Given a scenario, implement host or application security solutions]]

# TODO (Delete when done)
---
- [ ] Added vocab
- [x] Added and linked objectives in document
- [ ] Linked objectives back to document
- [ ] Linked any relevant backlinks to and from document