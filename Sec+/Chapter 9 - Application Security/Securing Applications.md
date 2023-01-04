---
tags: [CompTia,SecPlus,CyberSec,Certs]
#aliases:
#cssclass:
#publish:
---

# About
---
- #Microsoft  Office is one of the largest productivity suites
	- Excel - Spreadsheets
	- Word - Word Processor
	- Outlook - Email
	- More

# Protecting Files
---
- Password protect
	- Built in to many apps in Office suite
- Read Only
	- Stops from being modified
- [[Viruses#^dd31c6|Macros]]
	- Check settings
	- By default <u>SHOULD</u> set to "Disable all macros without notification"
		- Can sett with [[Group Policies]]
	- #Microsoft defaults to allowing
- Digital Certificates
	- Set to only open files from valid signatures
- Encrypt documents
	- Office or #Bitlocker

```ad-example
title: Password Protect
collapse:close
Tools > Password Protect
![[Windows_OfficePassProtect1.png]]
```

```ad-example
title: Macros
collapse:close
Preferences/Tools > Security
![[Windows_Macros1.png]]
```

# Protecting Emails
---
- Digital signatures and digital certificates
	- Relies on Public Key #Infrastructure  (PKI)
- Archive
	- File should be password protected and/or encrypted
- Junk mail
	- Filter in server and client

# Other Apps
---
- User Account Control (UAC)
	- Prevents unauthorized access and avoids #UserAction errors in the form of accidental changes ^b1fab1
	- When running it asks if you want to run as admin and you will need to put in admin credentials

```ad-example
title: UAC Popup
collapse:close
![[Windows_UAC1.png]]
```


# Objectives
---
- [[Objectives#1.4 - Given a scenario, analyze potential indicators associated with network attacks|1.4 - Given a scenario, analyze potential indicators associated with network attacks]]
- [[Objectives#3.2 - Given a scenario, implement host or application security solutions|3.2 - Given a scenario, implement host or application security solutions]]

# TODO (Delete when done)
---
- [ ] Added vocab
- [ ] Added and linked objectives in document
- [ ] Linked objectives back to document
- [ ] Linked any relevant backlinks to and from document