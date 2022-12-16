---
tags: [CompTia,SecPlus,CyberSec,Certs]
#aliases:
#cssclass:
#publish:
---

# About
---
- Software app that protect one computer or server ^357ca6
	- Also called "<u>Host based</u>" firewall
- Set rules and polices for in and out traffic
- Example
	- Web server would accept 80 and 443 whereas desktop shouldn't
- Versions
	- #Windows  - #Windows Firewall
	-  #OSX - PF and IPFW
	- #Linux - Iptables


# #Windows Firewall
---
- Every version of #Windows has a software firewall
- Versions
	- Basic version
		- In control panel
		- Home users use
	- #Windows Firewall with with advanced security
		- Businesses usually use
		- WF.msc

```ad-info
title: Windows Advanced Firewall
collapse: Close
![[Windows_Adv_Firewall.png]]
```

# #OSX
---
- Built-in for Mac and #OSX
- Basic version in "System preferences > Security and privacy"
- Two versions
	- CLI version named <u>"PF"</u>
		- Short for Packet filter
		- #OSX <u>10 and up</u>
	- Older ones used <u>"IPFW"</u>
		- <u>Internet protocol firewall</u>
	- Both are in FreeBSD which #OSX is based on

```ad-info
title: PF (Packet Filter)
collapse: close
![[MAC&OSX_Firewall.png]]
```

# #Linux
---
- Built-in called <u>"IPTables"</u>
	- CLI
	- Accept and reject rules

```ad-info
title: IPTables
collapse: close
![[Linux_IPtables_Firewall.png]]
```

# Other
---
- Other [[Endpoint Analysis#AntiVirus (AV)|AntiVirus (AV)]] may have their own [[Software Firewalls]]
- Some firewalls can use system resources
- Many businesses use hardware based firewalls for a first line of defense
- Best to run both hardware and software based

# Objectives
---
- [[Objectives#3.2 - Given a scenario, implement host or application security solutions|3.2 - Given a scenario, implement host or application security solutions]]