---
tags: [CompTia,SecPlus,CyberSec,Certs]
#aliases:
#cssclass:
#publish:
---

# About
---
- Service that enables dial-up and [[Virtual Private Network (VPN)|VPN]] connections to occur from remote clients ^a00863
- To provide [[Remote Desktop Services (RDS)]] you need a form of Remote Access Services (RAS) to provide a way to authenticate 
- Forms of [[Authentication]]
	- [[#Password Authentication Protocol (PAP)]]
	- [[#Challenge Handshake Authentication Protocol (CHAP)]]
	- [[#Microsoft Challenge Handshake Authentication Protocol (MS-CHAP)]]
	- [[#Microsoft Challenge Handshake Authentication Protocol Version 2 (MS-CHAPv2)]]
	- [[802.1x#Extensible Authentication Protocol (EAP)|Extensible Authentication Protocol (EAP)]]
- See also
	- [[802.1x]]
	- [[RADIUS vs TACAS+]]

# Password Authentication Protocol (PAP)
---
- Used to provide [[Authentication]] but it is not considered secure since it <u>transmits the login credentials unencrypted</u> ^09d807
- Older protocol
- <u>Insecure in any form</u>
- Does not provide [[802.1x#^539a82|Mutual Authentication]]

# Challenge Handshake Authentication Protocol (CHAP)
---
- Used to provide [[Authentication]] by <u>using the user's password to encrypt</u> a challenge string of random numbers  ^d79d29
- Server decrypts using the users stored password making sure original information sent in the challenge matches the encrypted text 
- Password is <u>never sent across network</u> but it is <u>stored unencrypted</u>
- Both client and server need to know a plaintext form of the password
	- Or the result of the password going through MD5 #Hashing
- Does not provide [[802.1x#^539a82|Mutual Authentication]]
  
```ad-example
title: CHAP Process
collapse:close
![[CHAPEx1.png]]
```

# Microsoft Challenge Handshake Authentication Protocol (MS-CHAP)
---
- #Microsoft version of [[#Challenge Handshake Authentication Protocol (CHAP)]] using DES encryption and MD4 #Hashing ^b47bd1
- Both client and server need to know a plaintext form of the password
	- Or the result of the password going through MD4 (yes MD4) #Hashing
- Support dropped after Vista
- <u>Existed</u> as an option for PPP, PPPoE and [[RADIUS vs TACAS+|RADIUS]]

# Microsoft Challenge Handshake Authentication Protocol Version 2 (MS-CHAPv2)
---
- Second version of [[#Microsoft Challenge Handshake Authentication Protocol (MS-CHAP)]] which contains stronger encryption and provides [[802.1x#^539a82|Mutual Authentication]] ^3c0357
- Uses NTLM encryption and SHA-1 #Hashing
- Exists as an option for [[802.1x]] and PPTP

# Comparison
---
| Authentication                                                                   | Mutual Authentication | Encryption | Hashing |
| -------------------------------------------------------------------------------- | --------------------- | ---------- | ------- |
| [[#Password Authentication Protocol (PAP)\|PAP]]                                      |                       |            |         |
| [[#Challenge Handshake Authentication Protocol (CHAP)\|CHAP]]                          |                       |            | MD5     |
| [[#Microsoft Challenge Handshake Authentication Protocol (MS-CHAP)\|MS-CHAP]]             |                       | DES        | MD4     |
| [[#Microsoft Challenge Handshake Authentication Protocol Version 2 (MS-CHAPv2)\|MS-CHAPv2]] | X                     | NTLM       | SHA-1   |

# Objectives
---
- [[Objectives#3.1 - Given a scenario, implement secure protocols|3.1 - Given a scenario, implement secure protocols]]
- [[Objectives#3.8 - Given a scenario, implement authentication and authorization solutions|3.8 - Given a scenario, implement authentication and authorization solutions]]