---
tags: [CompTia,SecPlus,CyberSec,Certs]
#aliases:
#cssclass:
#publish:
---

# About
---
- Want to prevent [[Securing the BIOS#^9479f4|Firmware]] exploits to create a more secure environment
- Multiple [[#Types]] of firmware

# [[Securing the BIOS#^9479f4|Firmware]] Exploits
---
- A [[Securing the BIOS#^9479f4|Firmware]] exploit gives an attacker an opportunity to run any code at the highest level of CPU privilege
	- By infecting the [[Securing the BIOS#^9479f4|Firmware]] yo can essentially have a [[Rootkits|Rootkit]] over the entire system

# [[Hardening]] Mechanisms

## UEFI
---
- A type of systems firmware providing support for 64-bit CPU operation at boot, full GUI and mouse operation at boot, and better boot security
- Supports various operations related to
- [[Securing the BIOS#^e94ab9|BIOS]] is legacy at this point
- See also [[Securing the BIOS#UEFI|Securing the BIOS]]

## Secure Boot
---
- A [[#UEFI]] feature that prevents unwanted processes from executing during the boot operation ^81f961
- As PC boots it checks for digital signatures from OS vendors
- If OS is not signed it will not boot
- This helps to avoid various types of [[Malware]]

## Measured Boot
---
- A [[#UEFI]] feature that gathers secure metrics to validate the boot process in an [[#Attestation]] report ^c83f3c
	- How long does it take to do X
	- How much CPU to do X
- See also [[Root of Trust]]

## Attestation
---
- Claim that the data presented in the report is valid by digitally signing it using the [[Root of Trust#TPM Expanded|TPM]] chips private key ^f55108
- [[#UEFI]] takes report and digitally signs it sending it off to the OS and CPU
- See also [[Disk Encryption#Trusted Platform Module (TPM)|Trusted Platform Module (TPM)]]

## eFUSE
---
- An "Electronic Fuse"
- A means for software or [[Securing the BIOS#^9479f4|Firmware]] to permanently alter the state of a transistor on a computer chip
- One time programing used to seal cryptographic keys and other security information during [[Securing the BIOS#^9479f4|Firmware]] development
- If altered it will "Blow the fuse" making it no longer valid or trusted

## Trusted Firmware Updates
---
- A [[Securing the BIOS#^9479f4|Firmware]] update that is digitally signed by the vendor and trusted by the system before installation
- Whenever a firmware update is available you need to ensure it is trusted or else you could blow an [[#eFUSE]]

## Self-Encrypting Drives
---
- A disk drive where the controller can automatically [[Disk Encryption#^501400|Encrypt]] data that is written to it ^93fa17
- Hard drives contain [[Securing the BIOS#^9479f4|Firmware]] to run [[Disk Encryption]] when data is being written and read
	- Done at hardware level to take load off of CPU and OS
- See also [[Disk Encryption#^7230a4|Self-Encrypting Drives]]

# Objectives
---
- [[Objectives#3.2 - Given a scenario, implement host or application security solutions|3.2 - Given a scenario, implement host or application security solutions]]