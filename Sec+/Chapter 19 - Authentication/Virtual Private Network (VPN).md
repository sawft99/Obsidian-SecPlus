---
tags: [CompTia,SecPlus,CyberSec,Certs]
#aliases:
#cssclass:
#publish:
---

# About
---
- A connection between two or more computers or devices not on the same private network that provides a layer of encryption between your user and the enterprise network ^0e5ea4
- Types
	- [[#Client-to-Site VPN]]
	- [[#Site-to-Site VPN]]
- See also
	- [[Wireless Encryption#Virtual Private Network (VPN)]]

# Client-to-Site VPN
---
- Also known as "Remote Access VPN"
- Enables users to work from <u>remote locations such as their homes, hotels, and other premises</u> as if they were directly connected to their corporate network ^695391

```ad-example
title: Remote VPN
collapse:close
![[VPNEx1.png]]
```

# Site-to-Site VPN
---
- Enables organizations to establish VPN tunnels <u>between two or more network infrastructure devices in different sites</u> so that they can communicate over a shared medium such as the Internet  ^ea5e3f
- Cheaper than dedicated leased line
- Both routers have an encryption key
- Many organizations use IPsec, GRE, PPP , L2TP and MPLS VPNs as site-to-site VPN protocols

```ad-example
title: Site-to-Site VPN
collapse:close
![[VPNEx2-1.png]]
```

# VPN Concentrator
---
- Specialized hardware device that allows for hundred of simultaneous connection for remote workers ^1adb32

# Split-Tunneling
---
- A remote user's work machine diverts internal traffic over the VPN but external traffic over their own internet connection
- Can be good from the perspective of saving bandwidth on the corporate network devices such as [[Routers]], [[Switches]], and [[Firewalls]]
- However this can be considered a security issue since this introduces another [[Malware Infections#Attack Vector|Attack Vector]] since their traffic is not being analyzed by a firewall or other security device
- Prevent with proper configuration and proper network segmentation or [[VLAN]]

# Objectives
---
- [[Objectives#3.3 - Given a scenario, implement secure network designs|3.3 - Given a scenario, implement secure network designs]]