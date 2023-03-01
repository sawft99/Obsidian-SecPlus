---
tags: [CompTia,SecPlus,CyberSec,Certs]
#aliases:
#cssclass:
#publish:
---

# About
---
- Biometrics rely on the physical characteristics of a person as a way to identify them ^522bda
- Common types are
	- Finger
		- Not just in [[Door Locks]], but also smart phones and other smart devices
	- Eye retina 
	- Distance in face
		- Also common in newer smart devices
	- Voice
- A form of one of the five factors of [[SecBasics#^45fffd|Authentication]]
	- "Something you are"

```ad-example
title: Fingerprint Biometric System
collapse:close
![[BiomentricFingerprintEx1.png]]
```

# False Acceptance Rate (FAR)
---
- Rate that a system authenticates a user as authorized or valid when they should not have been granted access to the system ^7b7faf
- A system mistakes one person for another
- The lower the false acceptance rate the better
- Increase sensitivity type settings to prevent or minimize
	- This may increase the [[#False Rejection Rate (FRR)]]

# False Rejection Rate (FRR)
---
- Rate that a system denies a user as authorized or valid when they should have been granted access to the system ^c60b71
- As much of a problem as [[#False Acceptance Rate (FAR)]]
- Increasing sensitivity in a system may increase the FRR
- May need to reduce sensitivity type settings

# Crossover Error Rate (CER)
---
- Where the [[#False Acceptance Rate (FAR)]] and [[#False Rejection Rate (FRR)]] are equal ^88d065
- Also known as "Equal Error Rate (EER)"
- Is a common measure for biometric equipment's effectiveness

```ad-example
title: CER Equilibrium
collapse:close
![[CEREx1.png]]
```

# Objectives
---
- [[Objectives#2.4 - Summarize authentication and authorization design concepts|2.4 - Summarize authentication and authorization design concepts]]