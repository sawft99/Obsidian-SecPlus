---
tags: [CompTia,SecPlus,CyberSec,Certs]
#aliases:
#cssclass:
#publish:
---

# About
---
- What each [[Virtualization#Virtual Machine Types|Virtual Machine]] runs on
- Manages the distribution of the physical resources of a host machine (Server) to the virtual machines being run (Guests) ^4158e0
- Includes CPU, memory, and hard disk space

# Types

## Type 1 - System
---
- "Bare metal" or "Native"
- <u>Runs directly on the host hardware</u> and functions as a type of OS
- Faster and more efficient than [[#Type 2]]
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

## Type 2 - Processor
---
- Runs in a normal such as #Microsoft #Windows , #Apple #OSX , and #Linux
- Host OS <u>runs an app that acts as a hypervisor</u>
- Examples
	- #Oracle Virtualbox

```ad-info
title: Virtual - Type 2
collapse:close
![[Virtual_Type2.png]]
```

# Application Containerization
---
- A single operating system [[Rootkits#Kernel|Kernel]] is shared across multiple virtual machine but each virtual machine receives its own user space for programs and data ^9c31f9
- Allows for <u>rapid and efficient</u> deployment of distributed applications without launching a full virtual machine
- More efficient than [[#Type 1]] and [[#Type 2]] if it can meet your needs
- Common on #Linux servers
- Examples
	- Docker
	- Parallels Virtuozzo
	- OpenVZ
- See also [[Threats to VMs#Compromised Containers|Compromised Containers]]

```ad-info
title: Application Container vs [[Hypervisors]]
collapse:close
![[Application_Containerization.png]]
```

# Examples - Installs

## [[#Type 1 - System]]
---
- Installing #VMware ESXI on a bare metal system

![](https://www.youtube.com/watch?v=r3EDlvfQAsw)

## [[#Type 2 - Processor]]
---
- Installing #Windows 10 on a Mac with #Oracle Virtualbox

![](https://www.youtube.com/watch?v=J-S_TvtIm5Y)

# Objectives
---
- [[Objectives#2.2 - Summarize virtualization and cloud computing concepts|2.2 - Summarize virtualization and cloud computing concepts]]