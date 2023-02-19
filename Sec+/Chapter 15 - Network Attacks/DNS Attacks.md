---
tags: [CompTia,SecPlus,CyberSec,Certs]
#aliases:
#cssclass:
#publish:
---

# About
---
- Attacks against or by using DNS
- Types
	- [[#DNS Poisoning]]
	- [[#Unauthorized Zone Transfers]]
	- [[#Altered Host Files]]
	- [[#Pharming]]
	- [[#Domain Name Kiting]]

# DNS Poisoning

## About
---
- When name resolution information is modified in the servers cache ^53507b
- Done to redirect client computers to redirect them to fraudulent or malicious sites
- Usually happens to internal DNS servers and not public ones

```ad-example
title: DNS Poisoning
collapse:close
![[DNSPoisoningEx1.png]]
```

## Prevention
---
- DNSSEC ^af0156
	- Encrypted signatures used when passing DNS info between servers ^3d08c9
- Latest [[Updates and Patches]]

```ad-example
title: DNSSEC
collapse:close
![[DNSSECEx1.png]]
![[DNSSECEx2.png]]
```

# Unauthorized Zone Transfers

## About
---
- Occurs when an attacker requests replication of the DNS info to their systems for use in future attacks
- Obtains IPs and names

## Prevention
---
- Zone transfers should be restricted between two servers that trust each other
- Don't allow other servers to ask for transfers

# Altered Host Files

## About
---
- Occurs when an attacker modifies the host file to have a client bypass the DNS server and redirects them to an incorrect or malicious website
- A host file is a plaintext file on a computer with a list of names matched to IP addresses ^2e6ce9
- Is checked before a DNS lookup is sent

## Prevention
---
- Set host file to read only
	- In #Windows `%systemroot%/system 32/drivers/etc`

# Pharming

## About
---
- Occurs when an attacker redirects one websites traffic to another website that is bogus or malicious ^8f19c8
- Done with [[#DNS Poisoning]] or [[#Altered Host Files]]

# Domain Name Kiting
---
- Attack that exploits a process in the way a domain name is registered so that the domain name is kept in limb and cannot be registered by an authenticated buyer ^82b445
- Example
	- 5 day grace period when you want to buy a domain but haven't spent the money yet
	- Attacker keeps removing and readding from their account keeping the domain constantly unavailable without buying it
- More of an abuse than an attack

# Objectives
---
- [[Objectives#1.1 - Compare and contrast different types of Social Engineering techniques|1.1 - Compare and contrast different types of Social Engineering techniques]]
- [[Objectives#1.4 - Given a scenario, analyze potential indicators associated with network attacks|1.4 - Given a scenario, analyze potential indicators associated with network attacks]]
- [[Objectives#3.1 - Given a scenario, implement secure protocols|3.1 - Given a scenario, implement secure protocols]]