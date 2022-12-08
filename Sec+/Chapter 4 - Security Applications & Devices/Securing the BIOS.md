---
tags: [CompTia,SecPlus,CyberSec,Certs]
#aliases:
#cssclass:
#publish:
---

# About
---
- Basic Input Output System ^53321f
- Firmware ^9479f4
	- Software on a chip ^28d134
- Modern BIOS has been replaced by [[#UEFI]]
	- Term BIOS may still be used to reference
-  Gives computer instructions on how it will send and receive input ^e94ab9
	- BIOS tells PC how and what to check to boot to
	- BIOS will take over the machine to load the OS
	- Responsible for any interactions with hardware

# UEFI
---
- Unified Extensible Firmware Interface
	- "YouFee"
- Newer modern standard
- Replaces BIOS but may be used interchangeably
# Securing
---
1. <u>Flash BIOS</u>
	1. Making sure firmware is the most up to date
	2. Manufacturer usually releases it on their site
	3. May need USB drive
2. <u>Setting an admin password</u> on BIOS
	1. Strong password
	2. Unique to BIOS and <u>not the same as a pc login</u>
3. Configure boot order
	1. <u>Deselect unneeded devices</u> such as CD drive, Floppy, and USB drives
	2. May only want to boot from internal HD or network
	3. Stops people from booting into a live CD or something similar
4. <u>Disable any ports and devices</u> not being used
	1. Parallel port, Serial port, unused network card
5. Enable Secure boot
	1. Additional processes during boot
	2. Loads Public key from [[Disk Encryption#Trusted Platform Module (TPM)|TPM]]
	3. <u>Verifies code and has been signed by manufacturer and has not been modified</u> ^e16786

# [[Objectives]]
---
- [[Objectives#3.2 - Given a scenario, implement host or application security solutions|3.2 - Given a scenario, implement host or application security solutions]]