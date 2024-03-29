---
tags: [CompTia,SecPlus,CyberSec,Certs]
#aliases:
#cssclass:
#publish:
---

# About
---
- Software application that protects one computer or server from unwanted traffic ^357ca6
	- Also called "<u>Host based</u>" firewall
- Set rules and polices for in and out traffic
- Example
	- Web server would accept 80 and 443 whereas desktop shouldn't
- Versions
	- #Windows  - #Windows Firewall
	-  #OSX - PF and IPFW
	- #Linux - Iptables
- See also
	- [[Firewalls]]
	- [[Unnecessary Ports]]

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
- Other [[Endpoint Analysis#AntiVirus (AV)|AntiVirus (AV)]] may have their own version of a software firewall
- Some firewalls can heavily use system resources
- Many businesses use [[Firewalls#Hardware Firewalls|Hardware Firewalls]] for a first line of defense
- Best to run both hardware and software based

# Objectives
---
- [[Objectives#3.2 - Given a scenario, implement host or application security solutions|3.2 - Given a scenario, implement host or application security solutions]]