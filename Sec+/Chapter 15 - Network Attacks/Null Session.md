---
tags: [CompTia,SecPlus,CyberSec,Certs]
#aliases:
#cssclass:
#publish:
---

# About
---
- An unauthenticated connection to the #Windows IPC$ share ^506470
-  Interprocess communications share (IPC$)
	- An admin share that allows computers to send info about files, folders, users, groups, computers, and servers to each other ^a3b0a8
- An attacker can use as part of information gathering

# Demo
---
-  `net use \\x.x.x.x\ipc$ "" /u:""`
	- Blank user and blank password 

```ad-example
title: Command Prompt
collapse:close
![[NullSessionEx1.png]]
```

# Prevention
---
- Blocking ports
	- 445 - SMB
	- 139 - NetBIOS
- [[NIDS & NIPS|IPS]] at the [[Perimeter Security|Perimeter]] to stop any outside connections from attempting to enumerate your computer

# Objectives
---
- [[Objectives#1.6 - Explain the security concerns associated with various types of vulnerabilities|1.6 - Explain the security concerns associated with various types of vulnerabilities]]