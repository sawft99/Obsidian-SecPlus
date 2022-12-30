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

## #ActiveDirectory
---
- You instead work with Group Policy Objectives (GPOs)
- Create user and computer policies
- Used to create a secure [[Unnecessary Applications#Baseline Image|Baseline]]
	- Once created you need to test with a [[#^331295|Baselining]] procedure
	- Everything should be categorized as safe or needing further investigation

```ad-info
title: Active Directory Group Policy
collapse:close

![[Windows_AD_GroupPolicy.png]]
```

# Applocker

## About
---
- Allows you to create rules for scripts, installers, packaged app, and executable rules
- [[Restricting Applications#Whitelisting|Whitelisting]] and [[Restricting Applications#Blacklisting|Blacklisting]] rules
- Can make rules based on publisher, path, or file #Hashing
- Examples
	- Allow all programs by default and then [[Restricting Applications#Blacklisting|Blacklist]] apps
	- Deny all programs by default and then [[Restricting Applications#Whitelisting|Whitelist]] apps
	- Any mix

## Process
---
#### Video

![Vid](https://www.youtube.com/watch?v=T-oSIeuNkbk)

#### Step by step

```ad-info
title: Applocker in Group Policy
collapse:close
![[Win_Applocker1.png]]
```

```ad-info
title: Creating an Applocker rule - Select Group
collapse:close
![[Win_Applocker_Rule1.png]]
```

```ad-info
title: Creating an Applocker rule - Select type
collapse:close
![[Win_Applocker_Rule2.png]]
```

```ad-info
title: Creating an Applocker rule - Define path
collapse:close
![[Win_Applocker_Rule3.png]]
```

```ad-info
title: Creating an Applocker rule - Exceptions
collapse:close
![[Win_Applocker_Rule4.png]]
```

```ad-info
title: Creating an Applocker rule - Naming
collapse:close
![[Win_Applocker_Rule5.png]]
```

```ad-info
title: Creating an Applocker rule - Results
collapse:close
![[Win_Applocker_Rule6.png]]
```

# Vocab
---
- Baselining
	- Process of measuring changes in the network, hardware, and software environment ^331295
	- Find what "normal" is so you can latter identify abnormal behavior, deviations, and [[IDS#^ed7614|anomalies]]

# Objectives
---
- [[Objectives#2.1 - Explain the importance of security concepts in an enterprise environment|2.1 - Explain the importance of security concepts in an enterprise environment]]
- [[Objectives#3.2 - Given a scenario, implement host or application security solutions|3.2 - Given a scenario, implement host or application security solutions]]