---
tags: [CompTia,SecPlus,CyberSec,Certs]
#aliases:
#cssclass:
#publish:
---

# About
---
- Examples
	- [[#Data Encryption Standard (DES)]]. [[#Triple DES (3DES)]]. [[#International Data Encryption Algorithm (IDEA)]], [[#Advanced Encryption Standard (AES)]], [[#Blowfish]], [[#Twofish]], RC4, RC5, RC6
- See also
	- [[Symmetric vs Asymmetric]]

# Data Encryption Standard (DES) 
---
- [[Cryptography#^e590e3|Encryption]] algorithm which breaks the input into 64-bit blocks and uses transportation and substitution to create [[Symmetric vs Asymmetric#^d56ba1|Ciphertext]] using an effective [[Cryptography#Key|Key]] strength of 56-bits
- Often a standard for encryption from ~1970 - 2000
- A type of [[Symmetric vs Asymmetric#Block Cipher|Block Cipher]]
- Superseded by [[#Triple DES (3DES)]] 

# Triple DES (3DES)
---
- [[Cryptography#^e590e3|Encryption]] algorithm which uses three separate [[Symmetric vs Asymmetric#Symmetric|Symmetric]] [[Cryptography#Key|Keys]] to encrypt, decrypt, then encrypt the plaintext into ciphertext in order to increase the strength of [[#Data Encryption Standard (DES)]]
- Essentially 112-bit key
- A type of [[Symmetric vs Asymmetric#Block Cipher|Block Cipher]]
- 3x slower than [[#Data Encryption Standard (DES)]]

# International Data Encryption Algorithm (IDEA)
---
- [[Symmetric vs Asymmetric#Symmetric|Symmetric]] [[Symmetric vs Asymmetric#Block Cipher]|Block Cipher]] which uses 64-bit blocks to encrypt plaintext into [[Symmetric vs Asymmetric#^d56ba1|Ciphertext]] 
- Key size is 128-bits
- Harder to break and faster than [[#Data Encryption Standard (DES)]]
- Not as common as [[#Advanced Encryption Standard (AES)]]

# Advanced Encryption Standard (AES)
---
- [[Symmetric vs Asymmetric#Symmetric|Symmetric]] [[Symmetric vs Asymmetric#Block Cipher]|Block Cipher]] that uses 128-bit, 192-bit, or 256-bit blocks and a matching encryption key size to encrypt plaintext into [[Symmetric vs Asymmetric#^d56ba1|Ciphertext]]
- Sometimes called the "Rijndael Algorithm"
- Standard for federal government sensitive but unclassified information
- See also
	- [[Disk Encryption#Advanced Encryption Standard (AES)]]

# Blowfish
---
- [[Symmetric vs Asymmetric#Symmetric|Symmetric]] [[Symmetric vs Asymmetric#Block Cipher]|Block Cipher]] that uses 64-bit blocks and a variable length encryption key to encrypt plaintext into [[Symmetric vs Asymmetric#^d56ba1|Ciphertext]]
- Made as a replacement for [[#Data Encryption Standard (DES)]] but not popular
- Never patented and open source

# Twofish
---
- [[Symmetric vs Asymmetric#Symmetric|Symmetric]] [[Symmetric vs Asymmetric#Block Cipher]|Block Cipher]] that replaced [[#Blowfish]] and uses 128-bit blocks and a 128-bit, 192-bit, or 256-bit encryption [[Cryptography#Key|Key]] to encrypt plaintext into [[Symmetric vs Asymmetric#^d56ba1|Ciphertext]]
- Never patented and open source

# RC Series

## Rivet Cipher (RC) 1 - 3
---
- RC1
	- Never released to public
- RC2
	- Skipped over and considered week
- RC3
	- Broken before public release

## RC4 
---
- [[Symmetric vs Asymmetric#Symmetric|Symmetric]] [[Symmetric vs Asymmetric#Stream Cipher|Stream Cipher]] using a variable [[Cryptography#Key|Key]] size from 40-bits to 2048-bits used in SSL and [[Wireless Encryption#Wired Equivalent Privacy (WEP)|Wired Equivalent Privacy (WEP)]]

## RC5
---
- [[Symmetric vs Asymmetric#Symmetric|Symmetric]] [[Symmetric vs Asymmetric#Block Cipher|Block Cipher]] with a [[Cryptography#Key|Key]] size up to 2048-bits

## RC6
---
- [[Symmetric vs Asymmetric#Symmetric|Symmetric]] [[Symmetric vs Asymmetric#Block Cipher|Block Cipher]] that was introduced as a replacement for [[#Data Encryption Standard (DES)]] but was beat by [[#Advanced Encryption Standard (AES)]] instead

# Table
---

| Cipher                                              | Symmetric | Asymmetric | Key Bits          | Block Bits    |
| --------------------------------------------------- | --------- | ---------- | ----------------- | ------------- |
| [[#Data Encryption Standard (DES)]]                 | X         |            | 56                | 64            |
| [[#Triple DES (3DES)]]                              | X         |            | 56/112            | 64            |
| [[#International Data Encryption Algorithm (IDEA)]] | X         |            | 128               | 64            |
| [[#Advanced Encryption Standard (AES)]]             | X         |            | 128/192/256       | 128/192/256   |
| [[#Blowfish]]                                       | X         |            | 32-248          | 64            |
| [[#Twofish]]                                        | X         |            | 128/192/256       | 128           |
| [[#RC4]]                                            | X         |            | 40-2048           | <u>Stream</u> |
| [[#RC5]]                                            | X         |            | 0-2040            | 32/64/128     |
| [[#RC6]]                                            | X         |            | 128/192/256..2040 | 128           |

# Objectives
---
- [[Objectives#2.8 - Summarize the basics of cryptographic concepts|2.8 - Summarize the basics of cryptographic concepts]]

# TODO (Delete when done)
---
- [ ] Added vocab
- [x] Added and linked objectives in document
- [x] Linked objectives back to document
- [ ] Linked any relevant backlinks to and from document