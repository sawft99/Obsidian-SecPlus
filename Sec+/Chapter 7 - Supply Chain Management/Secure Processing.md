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
- <u>Labeled differently across some brands</u>
	- #AMD
		- Secure Memory Encryption (SME)
		- Secure Encrypted Virtualization (SEV)
	- #Intel
		- Trusted Execution Technology (TXT)
		- Software Guard Extension (SGX)

## Trusted Execution
---
- The CPUs [[#Processor Security Extensions (PSE)]] invoke the [[Disk Encryption#Trusted Platform Module (TPM)|Trusted Platform Module (TPM)]] chip and [[Trusted Firmware#Secure Boot|Secure Boot]] [[Trusted Firmware#Attestation|Attestation]] to ensure that a [[Trusted Operating System]] is running
- When you boot the system want to use[[Trusted Firmware]], [[Trusted Firmware#UEFI|UEFI]], [[Root of Trust#TPM Expanded|TPM]] and [[Trusted Firmware#Secure Boot|Secure Boot]]
- Common to #Microsoft when installing #Windows on #AMD and #Intel hardware

## Secure Enclave
---
- Allows a trusted process to create an encrypted container for sensitive data for sensitive data
- Helps prevent [[Buffer Overflow]]
- Store encryption data inside itself
- Once [[Trusted Operating System]] is running the Secure Enclave can be made

## Atomic Execution
---
- Certain operations that should only be performed once or not at all such as initializing a memory location
- A [[#Processor Security Extensions (PSE)]] in place to make sure an atomic execution should not

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