---
tags: [CompTia,SecPlus,CyberSec,Certs]
#aliases:
#cssclass:
#publish:
---

# About
---
- A set of rules or policies that can be applied to a set of users or computer accounts within the operating system ^7935c4

# Using in #Windows

## Local
---
- Local Group Policy Editor
	- Creates and manages local computer polices in a #Windows environment
	- GPedit.msc
- Policies ^0cf784
	- Each one acts as a <u>security template</u>
		- A group of policies that can be loaded through one procedure
	- A set of rules that can be applied to users and computers
		- Lockouts, Password complexity, White/Black list apps

```ad-info
title: Local Group Policy Editory - GPEdit.msc
collapse:close
![[Windows_LocalPolicy.png]]
```

## Active Directory
---
- You instead work with Group Policy Objectives (GPOs)
- Used to create a secure [[Unnecessary Applications#Baseline Image|Baseline]]
	- Once created you need to test with a [[#^331295|Baselining]] procedure
	- Everything should be categorized as safe or needing further investigation

```ad-info
title: Active Directory Group Policy
collapse:close

![[Windows_AD_GroupPolicy.png]]
```

# Vocab
---
- Baselining
	- Process of measuring changes in the network, hardware, and software environment ^331295
	- Find what "normal" is so you can latter identify abnormal behavior, deviations, and [[IDS#^ed7614|anomalies]]

# Objectives
---
- [[Objectives#2.1 - Explain the importance of security concepts in an enterprise environment|2.1 - Explain the importance of security concepts in an enterprise environment]]

# TODO (Delete when done)
---
- [x] Added vocab
- [ ] Added and linked objectives in document
- [ ] Linked objectives back to document
- [ ] Linked any relevant backlinks to and from document