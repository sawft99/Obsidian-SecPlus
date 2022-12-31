---
tags: [CompTia,SecPlus,CyberSec,Certs]
#aliases:
#cssclass:
#publish:
---

# About
---
- Occurs when a process stores data outside the memory range allocated by the developer ^7e4396
- <u>85% of data breaches occur from Buffer Overflows</u> as the initial [[Malware Infections#Attack Vector|Attack Vector]]
- Example
	- A glass can hold 16 oz., if you pour in 20 oz, it will overflow onto the table and create a mess

# Buffer
---
- A temporary storage area that a program uses to store data ^80b29e

# Stack

## About
---
- Reserved area of memory where the program saves the return address when a function call instruction is received ^f4b832

## First In Last Out
---
- Type of [[#Stack]] where the first thing in is the last thing to be removed
- Data is filled from the bottom of the memory to the top
	- <u>Picture example is inverse of this</u>, as in top to bottom, but this is considered the standard way to represent a stack
- [[Buffer Overflow]] process that is specific to this model
	- If an attacker places too much information in the [[#Stack]] or changes the value of the Return pointer they can carry out an attack
	- Overwrite the return address of the pointer so that it will point to a different place in the [[#Stack]] where an attacker could have left some malicious code or [[Malware]]
	- When the non malicious code (The actual app) is run it hits the return pointer and will execute the malicious code or [[Malware]]
		- AKA [[#Smashing the Stack]]

```ad-info
title: Stack - First In Last Out
collapse:close
![[StackExample1.png]]
```

# Smashing the Stack
---
- Occurs when an attacker fills up the buffer with Non Operational Instruction (NOP) so that the return address may hit a NOP and continue on until it finds the attackers code to run

# Examples & Explanations
---
## Short Version - <u>At the 1:22 mark</u>

![](https://www.youtube.com/watch?v=TSeqEN-ZXe4)

## Long Version - <u>At the 1:09 mark</u>

![](https://www.youtube.com/watch?v=1S0aBV-Waeo)

# Objectives
---
- [[Objectives#1.3 - Given a scenario, analyze potential indicators associated with application attacks|1.3 - Given a scenario, analyze potential indicators associated with application attacks]]

# TODO (Delete when done)
---
- [ ] Added vocab
- [ ] Added and linked objectives in document
- [ ] Linked objectives back to document
- [ ] Linked any relevant backlinks to and from document