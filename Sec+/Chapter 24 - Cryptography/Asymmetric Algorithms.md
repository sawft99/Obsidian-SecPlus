---
tags: [CompTia,SecPlus,CyberSec,Certs]
#aliases:
#cssclass:
#publish:
---

# About
---
- Examples
	- Diffie-Hellman
	- RSA
	- ECC
- See also
	- [[Symmetric vs Asymmetric]]
	- [[WIFI Protected Access version 3 (WPA3)#TLS/Diffie-Hellman Key Exchange]]

# Diffie-Helman (DH)
---
- Used to conduct key exchanges and secure key distribution over an unsecure network ^e747f6
- Common in a VPN and IPSEC
- A VPN may require a [[Symmetric vs Asymmetric#Symmetric|Symmetric]] key but first uses an [[Symmetric vs Asymmetric#Asymmetric|Asymmetric]] such as this to exchange the key afterwards
- Subject to [[Hijacking#Man-in-the-Middle (MITM)|Man-in-the-Middle (MITM)]]
	- Require [[Authentication]] or a digital certificate

# Rivest, Shamir, and Adleman (RSA) 
---
- [[Symmetric vs Asymmetric#Asymmetric|Asymmetric]] algorithm that relies on the mathematically difficulty of factoring large prime numbers ^98000a
- Often used for a [[Public Key Cryptography#Digital Signature]|Digital Signature]]
- Key size 1024-bit to 4096-bit

# Elliptic Curve Cryptography (ECC)
---
- Algorithm based upon the algebraic structure of elliptic curves over finite fields to define the keys ^f063e3
- ECC with a 256-bit key is considered just as secure as RSA with a 2048-bit key
- Common in mobile devices because of the performance benefits

# Elliptic Curve Diffie-Hellman (ECDH)
---
- An [[#Elliptic Curve Cryptography (ECC)]] variant of [[#Diffie-Helman (DH)]]

# Elliptic Curve Diffie-Helman Ephemeral (ECDHE)
---
- An [[#Elliptic Curve Diffie-Hellman (ECDH)]] which uses a different [[Cryptography#Key|Key]] for each portion of the key exchange

# Elliptic Curve Digital Signature Algorithm (ECDSA)
---
- A Public Key encryption algorithm by the US government for their [[Public Key Cryptography#Digital Signature|Digital Signature]]

# Objectives
---
- [[Objectives#2.8 - Summarize the basics of cryptographic concepts|2.8 - Summarize the basics of cryptographic concepts]]

# TODO (Delete when done)
---
- [ ] Added vocab
- [ ] Added and linked objectives in document
- [ ] Linked objectives back to document
- [ ] Linked any relevant backlinks to and from document