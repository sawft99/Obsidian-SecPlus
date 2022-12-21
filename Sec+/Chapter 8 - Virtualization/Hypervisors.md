---
tags: [CompTia,SecPlus,CyberSec,Certs]
#aliases:
#cssclass:
#publish:
---

# About
---
- What each [[Virtualization#Virtual Machine Types|Virtual Machine]] runs on
- Manages the distribution of the physical resources of a host machine (Server) to the virtual machines being run (Guests)
- Includes CPU, memory, and hard disk space

# Types

## Type 1
---
- "Bare metal" or "Native"
-<u> Runs directly on the host hardware</u> and functions as a type of OS
- Faster and more efficient
- Hypervisor doesn't need to waste resources by running a full OS
- <u>Stripped down specialized OS</u> to provide physical resources to a [[Virtualization#Virtual Machine Types|Virtual Machine]] it hosts
- Examples
	- #Microsoft HyperV
	- #Citrix Zen
	- #VMware ESXI
	- #VMware Vsphere

```ad-info
title: Virtual - Type 1
collapse:close
![[Virtual_Type1.png]]
```

## Type 2
---
- Runs in a normal such as #Microsoft #Windows , #Apple #OSX , and #Linux
- Host OS <u>runs an app that acts as a hypervisor</u>
- Examples
	- Virtualbox

```ad-info
title: Virtual - Type 2
collapse:close
![[Virtual_Type2.png]]
```

# Application Containerization
---
- A single operating system [[Rootkits#Kernel|Kernel]] is shared across multiple virtual machine but each virtual machine receives its own user space for programs and data
- Allows for <u>rapid and efficient</u> deployment of distributed applications without launching a full virtual machine

```ad-info
title: Application Containerization - Virtual vs Container
collapse:close
![[Application_Containerization.png]]
```

# Objectives
---
- [[Objectives#2.2 - Summarize virtualization and cloud computing concepts|2.2 - Summarize virtualization and cloud computing concepts]]

# TODO (Delete when done)
---
- [ ] Added vocab
- [ ] Added and linked objectives in document
- [ ] Linked objectives back to document
- [ ] Linked any relevant backlinks to and from document