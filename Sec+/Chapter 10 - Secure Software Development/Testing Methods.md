---
tags: [CompTia,SecPlus,CyberSec,Certs]
#aliases:
#cssclass:
#publish:
---

# About
---
- Analyst often aren't programmers and don't need to know specifics about code techniques
- These methods are applied during the [[Software Development#Testing|Testing]] phase of the [[Software Development#Software Development Life Cycle (SDLC)|Software Development Life Cycle (SDLC)]]
- You are attempting to break the system by stressing or creating an exception
	- Programmers need to ensure that their program [[SDLC Principles#Fail Securely|Fails Securely]]
	- Purposely create error conditions to cause errors and see how the system reacts

# System Testing

## Blackbox Testing
---
- Occurs when a tester is not provided any information about the system or program prior to conducting the test
- Just being handed the program

## Whitebox Testing
---
- Occurs when the tester is provided full details of a system including the source code, diagram, and user credentials

## Graybox Testing
---
- A mixture of [[#Whitebox Testing]] and [[#Blackbox Testing]] where you are given partial information
- Conduct as if you don't have full access
- Examples
	- Getting user credentials but not admin
	- Getting IP of devices but not the version of the software running on it

# Errors
---
- Exceptions
	- Another term for error ^13a069
- Runtime Error
	- A coding error that occurs <u>while the program is running</u> ^ed3630
- Syntax Error
	- A coding error <u>prevents the program from running</u> ^492e68
	- Such as leaving out a semicolon or parentheses by accident in the code

# Structured Exception Handling (SEH)
---
- When an error occurs you want to collect details and discover why the issue occurred
- Provides control over what the application should do when faced with a runtime or syntax error ^f9b49c
- Helpful with debugging and testing
- Test erroneous input as a normal user
- Example
	- Credit card site asking for information like Name, DOB, and SSN
	- Entering information such as a 14th month or an SSN less than 9 characters should be caught
- Using [[SDLC Principles#Never Trust User Input|Input Validation]] should catch or prevent these errors
	- Attackers often abuse input validation to conduct Cross site Scripting (XSS), [[SQL Injection]], and [[Buffer Overflow]]

```ad-example
title: Credit Card Error Example
collapse:close
![[CreditCardInputError1.png]]
![[CreditCardInputError2.png]]
```

# Forms Of Code Analysis

## Static Analysis
---
- Source code of an application is reviewed manually or with automatic tools <u>without running the code</u> ^95dd07
- Reviewed by someone who knows the language it is written in
- Some automation tools can be used to automatically find errors and bring them to your attention

## Dynamic Analysis
---
- Performing an analysis while software is being run ^c957be
- [[#Fuzzing]] is a common method used to perform dynamic analysis

## Fuzzing
---
- Using a piece of software/program to insert randomized data into another software/program in an attempt to find system failures, memory leaks, error handling issues, and improper [[SDLC Principles#Never Trust User Input|Input Validation]] ^e90821
- Does many different types of random inputs to test
- Network fuzzing also exists to stress test the entirety of a network

# Objectives
---
- [[Objectives#2.3 - Summarize secure application development, deployment, and automation concepts||2.3 - Summarize secure application development, deployment, and automation concepts|]]
- [[Objectives#3.2 - Given a scenario, implement host or application security solutions|3.2 - Given a scenario, implement host or application security solutions]]