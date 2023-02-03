---
tags: [CompTia,SecPlus,CyberSec,Certs]
#aliases:
#cssclass:
#publish:
---

# About
---
- Buffer
	- A temporary storage area that a program uses to store data ^80b29e
- Stack
	- Reserved area of memory where the program saves the return address when a function call instruction is received ^f4b832
- Buffer Overflow
	- Occurs when a process stores data outside the memory range ([[#^80b29e|Buffer]]) allocated by the developer ^7e4396
- Buffer Overflow can also e used as a general term to refer to any other section of memory with an overflow issue
- <u>85% of data breaches occur from Buffer Overflows</u> as the initial [[Malware Infections#Attack Vector|Attack Vector]]
- Example
	- A glass can hold 16 oz., if you pour in 20 oz, it will overflow onto the table and create a mess

```ad-info
title: Memory Layout
collapse:close
![[MemoryArea1.png]]
```

```ad-info
title: Stack Layout
collapse:close
![[StackArea1.png]]
```

# First In Last Out
---
- Principle in a [[#^f4b832|Stack]] where the first thing in is the last thing to be removed
- Data is filled from the bottom of the memory to the top (Low address to high address)
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
- Occurs when an attacker fills up the <u>stack portion of the buffer</u> so that the return address may lead into and continue on until it finds the attackers code to run ^3d13e7
- NOP instruction
	- An instruction telling the program to do nothing and continue on to the next part ^fe8100
- A common method to use is adding NOP instructions to fill the space
	- Can lead to a [[#NOP Slide]]

# NOP Slide
---
- When the series of NOPs that occur are hit by the legit app and they finally hit the return pointer that leads to the memory address containing the malicious code/[[Malware]] ^c9fb54

```ad-info
title: NOP Slide Example
collapse:close
![[NOPSlideExample1.png]]
```

# Address Space Randomization Layout (ASLR)
---
- Method used by programmers to randomly arrange the different address spaces used by a program or process to prevent [[Buffer Overflow]] exploits ^15aa75
- Helps prevent attacker form knowing or guessing where a return pointer is in a legitimate program has been set to call back
	- Side channel attacks can potentially bypass
- Primarily made for common apps or OS's
- Introduced in #Windows Vista

# Videos
---
## Short Version - <u>At the 1:22 mark</u>

![](https://www.youtube.com/watch?v=TSeqEN-ZXe4)

## Long Version - <u>At the 1:09 mark</u>

![](https://www.youtube.com/watch?v=1S0aBV-Waeo)

# Objectives
---
- [[Objectives#1.3 - Given a scenario, analyze potential indicators associated with application attacks|1.3 - Given a scenario, analyze potential indicators associated with application attacks]]
- [[Objectives#2.3 - Summarize secure application development, deployment, and automation concepts|2.3 - Summarize secure application development, deployment, and automation concepts]]