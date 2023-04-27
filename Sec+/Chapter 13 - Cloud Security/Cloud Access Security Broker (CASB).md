---
tags: [CompTia,SecPlus,CyberSec,Certs]
#aliases:
#cssclass:
#publish:
---

# About
---
- Cloud Access Security Broker (CASB)
	- Enterprise management software designed to mediate access to cloud services by users across all types of devices ^d99896
- Middle man for authentication and people are using the services they are supposed to
- Provide visibility into how clients and other network nodes use cloud services
	- Monitoring #UserAction
- Can be done with [[#Forward Proxy]], [[#Reverse Proxy]], or [[#API]]
- Examples
	- Symantec - Blue Coat Proxy
	- Mcafee - Sky High Network
	- Force Point
	- #Microsoft - Cloud App Security
	- Cisco - Cloudlock

```ad-info
title: CASB
collapse:close
![[CASB1.png]]
```

# Features
---
- Single Sign On (SSO)
	- Enforce [[Network Access Control]] and [[SecBasics#^45fffd|Authorization]] across your organization from the enterprise network all the way to the cloud provider ^69ea35
- [[Malware]] Scanning
- [[SecBasics#^45fffd|Monitor and audit]] user activity
- Mitigate data exfil with [[Data Loss Prevention (DLP) - Appliance]] type solutions

# Forward Proxy
---
- A security appliance or host positioned at the client network edge that forwards user traffic to the cloud network if the contents of that traffic comply with policy ^55f9cf
- Can be bypassed
- Inside network to outside network on the internet
- See also
	- [[Proxy Servers]]

```ad-info
title: Forward Proxy
collapse:close

![[ForwardProxy1.png]]
```

# Reverse Proxy
---
- An appliance positioned at the cloud network edge and directs traffic to cloud services if the contents of that traffic comply with policy ^87757c
- Internet clients must connect and go through the reverse proxy before reaching any other resources on that network
- Outside network on the internet to inside network
- Only works if cloud app supports proxies
- See also
	- [[Proxy Servers]]

```ad-info
title: Reverse Proxy
collapse:close

![[ReverseProxy.png]]
```

# Application Programming Interface (API)
---
- A method that uses the brokers connections between the cloud service and the cloud consumer ^0d4b60
- Sending data between cloud ser vice and cloud consumer
- Dependent on API supporting the functions your policy needs
	- An API not having necessary functionality for your needs
- See also
	- [[Application Programming Interface (API)]]

# Objectives
---
- [[Objectives#2.1 - Explain the importance of security concepts in an enterprise environment|2.1 - Explain the importance of security concepts in an enterprise environment]]
- [[Objectives#2.2 - Summarize virtualization and cloud computing concepts|2.2 - Summarize virtualization and cloud computing concepts]]
- [[Objectives#3.3 - Given a scenario, implement secure network designs|3.3 - Given a scenario, implement secure network designs]]
- [[Objectives#3.6 - Given a scenario, apply cybersecurity solutions to the cloud|3.6 - Given a scenario, apply cybersecurity solutions to the cloud]]