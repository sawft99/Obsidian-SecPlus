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
- Low level CPU changes and instructions that enable secure processing ^e3b86c
- <u>Labeled differently across some brands</u>
	- #AMD
		- Secure Memory Encryption (SME)
		- Secure Encrypted Virtualization (SEV)
	- #Intel
		- Trusted Execution Technology (TXT)
		- Software Guard Extension (SGX)

## Trusted Execution
---
- The CPUs [[#Processor Security Extensions (PSE)]] invokes the [[Disk Encryption#Trusted Platform Module (TPM)|Trusted Platform Module (TPM)]] chip and [[Trusted Firmware#Secure Boot|Secure Boot]] [[Trusted Firmware#Attestation|Attestation]] to ensure that a [[Trusted Operating System]] is running ^cb8327
- When you boot the system want to use[[Trusted Firmware]], [[Trusted Firmware#UEFI|UEFI]], [[Root of Trust#TPM Expanded|TPM]] and [[Trusted Firmware#Secure Boot|Secure Boot]]
- Common to #Microsoft when installing #Windows on #AMD and #Intel hardware

## Secure Enclave
---
- An extension that allows a trusted process to create an encrypted container for sensitive data for sensitive data ^3a07c7
- Helps prevent [[Buffer Overflow]]
- Store encryption data inside itself
- Once [[Trusted Operating System]] is running the Secure Enclave can be made

## Atomic Execution
---
- Extensions in place to control certain operations that should only be performed once or not at all such as initializing a memory location ^28e559
- Extension in place to make sure an atomic execution
- Help against [[Buffer Overflow]] and race conditions

## Bus Encryption
---
- Data encrypted by an application prior to being placed on the data bus ^010ce7
- Ensures data sent over a network/bus is protected because it has #E2E (End to End Encryption)
- Device at other end is a trusted device
- Example:
	- HDCP unauthorized Roku error

# Objectives
---
- [[Objectives#3.2 - Given a scenario, implement host or application security solutions|3.2 - Given a scenario, implement host or application security solutions]]