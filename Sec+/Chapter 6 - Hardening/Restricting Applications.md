---
tags: [CompTia,SecPlus,CyberSec,Certs]
#aliases:
#cssclass:
#publish:
---

# About
---
- Stopping users from downloading, installing, and running software
- Able to centrally manage both [[#Whitelisting]] and [[#Blacklisting]]
	- Microsoft #ActiveDirectory and #GroupPolicy

# Whitelisting
---
- <u>Only applications that are on the list are allowed</u> to be run by the operating system while all other applications are blocked ^80ea87
	- "ACL rule w/ explicit allow"
- <u>More secure</u>
- Everything denied by default with specified apps being the only ones allowed to run
- More difficult to setup and manage
- Every time an update to an app is made you need to adjust your list

# Blacklisting
---
- Any application placed on the list will be <u>prevented from running while all others will be allowed</u> to run ^74bc0c
- Less secure
- Every new version of a program or [[Malware]] evolution would need to be explicitly denied

# Services

## About
---
- Any application that runs in the background and performs various functions ^b13d85
- Any unused services should be disabled
- #Windows update service often disabled because [[Updates and Patches]] are usually handled by a third party service in larger environments

## #Windows

### GUI
---
 1. Start
 2. Services.msc
 3. Double click on a service to see its details
	 1. Startup type
		 1. If you stop a service and it is set to "Automatic", once you reboot the service will start itself again
		 2. Set to "Disable" if you do not want that to happen
	 2. Starting and stopping service

```ad-info
title: Services
collapse:close
![[Win_Service1.png]]
```

```ad-info
title: Service Details
collapse:close
![[Win_Service2.png]]
```

### CLI
---
1. In a command prompt (CMD)
	1. sc stop wuauserv
	2. sc start ...
	3. net stop wuauserv

```ad-info
title: Services CLI
collapse:close
![[Win_Service3.png]]
```

# #OSX

## GUI
---
1. Applications > Utilities > Activity Monitor
2. Sort by process
3. Double click
4. You can see various information about a service
5. Can click "Quit" or "Force Quit" on service
	1. "Quit" will attempt to exit the application cleanly first
	2. For [[Malware]] you likely want "Force Quit"

```ad-info
title: Accessing Activity Monitor
collapse:close
1. Applications
![[OSX_Service1.png]]
2. Utilities
![[OSX_Service2.png]]
3. Activity Monitor
![[OSX_Service3.png]]
```

```ad-info
title: Inside Activity Monitor
collapse:close
1. Opening Activity Monitor 
![[OSX_Service4.png]]
2. Service details
![[OSX_Service5.png]]
3. Stopping a service
![[OSX_Service6.png]]
```

## CLI
---
- See [[#Linux]]

# #Linux

## CLI
---
1. Open "Terminal"
	1. Use "top" command
2. Locate desired service and its [[#^206b5d|PID]]
3. In terminal again
	1. kill pid xxxx

```ad-info
title: Top Command
collapse:close
![[Linux_Service1.png]]
```

```ad-info
title: Kill Command
collapse:close
![[Linux_Service2.png]]
```

# Vocab
---
- Process Identifier (PID) ^206b5d
	- A random number assigned to a running application to represent it
	- Can be used as a reference

# Objectives
---
- [[Objectives#3.2 - Given a scenario, implement host or application security solutions|3.2 - Given a scenario, implement host or application security solutions]]
- [[Objectives#3.3 - Given a scenario, implement secure network designs|3.3 - Given a scenario, implement secure network designs]]
- [[Objectives#4.4 - Given an incident, apply mitigation techniques or controls to secure an environment|4.4 - Given an incident, apply mitigation techniques or controls to secure an environment]]