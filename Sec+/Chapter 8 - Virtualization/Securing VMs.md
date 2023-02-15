---
tags: [CompTia,SecPlus,CyberSec,Certs]
#aliases:
#cssclass:
#publish:
---

# About
---
- Similar to methods used to secure a physical server
	- Ensuring [[Updates and Patches]] are installed and kept up to date
	- Each VM has a good [[Endpoint Analysis#AntiVirus (AV)|AntiVirus (AV)]]
	- [[IDS#HIDS|HIDS]]
	- [[Software Firewalls]]
	- Strong passwords
	- [[Group Policies]]

# Mitigations
---
- Ensuring [[Hypervisors]] are up to date to avoid issues such as [[Threats to VMs#VM Escape|VM Escape]]
- Limit the number of connections between the [[Virtualization#Virtual Machine Types|Virtual Machine]] and the physical host
	- Virtual NIC and Virtual shares
	- Creates more data being transferred and can reduce your ability to isolate
- Remove unnecessary virtual hardware, shared folders, and features
- Spread [[Virtualization#Virtual Machine Types|Virtual Machines]] across several physical computers to minimize potential exhausting of resources and creating a [[Denial of Service (DoS)]] scenario
- Proper [[Patch Management]]
- Keeping track of all [[Virtualization#Virtual Machine Types|Virtual Machines]] and where they are deployed or else "Virtualization Sprawl" can occur ^bfbd7c
	- When [[Virtualization#Virtual Machine Types|Virtual Machines]] are created, used, and deployed, without proper management or oversight by system admins ^089aa0
- Enable [[Disk Encryption#^501400|Encryption]] on the files that make up the [[Virtualization#Virtual Machine Types|Virtual Machine]]

```ad-example
title: VM Folder Example
collapse:close
![[VM_Folder1.png]]
```

# Videos

## VM Encryption
---

![](https://www.youtube.com/watch?v=8U-TAR0aYYQ)

## Shared Folders
---

![](https://www.youtube.com/watch?v=q7CcpuEuI-Q)

# Objectives
---
- [[Objectives#2.2 - Summarize virtualization and cloud computing concepts|2.2 - Summarize virtualization and cloud computing concepts]]