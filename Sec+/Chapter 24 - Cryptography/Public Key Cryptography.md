---
tags: [CompTia,SecPlus,CyberSec,Certs]
#aliases:
#cssclass:
#publish:
---

# About
---
- Doesn't require a shared secret key
- Instead uses a "key pair"
	- Public key and Private key
- Can provide
	- [[SecBasics#^fc61e9|Confidentiality]]
		- Data should be encrypted by using recipients Public [[Cryptography#Key|Key]]
		- No one else can read, even the sender
		- Only the recipients private key can decrypt
	- [[Authentication]]
	- [[SecBasics#^48ae1d|Integrity]]
	- [[Symmetric vs Asymmetric#Non-repudiation|Non-repudiation]]
		- Data should be encrypted by using senders Private [[Cryptography#Key|Key]]
		- Anyone with access to your public key can then read the message
		- Lacks [[SecBasics#^fc61e9|Confidentiality]] in this scenario
- See also
	- [[Symmetric vs Asymmetric#Asymmetric]]

```ad-example
title: Cofidentiality
collapse:close
![[ConfidentialityEx1.png]]
```

# Digital Signature
---
- A #Hashiing digest of a message is encrypted with the sender's private [[Cryptography#Key|Key]] to let the recipient know the document was created and sent by the person claiming to have sent it ^2db298
- Provides [[SecBasics#^48ae1d|Integrity]] for the message as well as [[Symmetric vs Asymmetric#Non-repudiation|Non-repudiation]] because only the sender has access to the [[Cryptography#Key|Key]]
- Message is taken and encrypted with the recipients public [[Cryptography#Key|Key]] and provides [[SecBasics#^fc61e9|Confidentiality]]

# Objectives
---
- [[Objectives#2.8 - Summarize the basics of cryptographic concepts|2.8 - Summarize the basics of cryptographic concepts]]