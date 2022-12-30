---
tags: [CompTia,SecPlus,CyberSec,Certs]
#aliases:
#cssclass:
#publish:
---

# About
---
- Bugs are common place today because of the size and complexity of applications
	- Windows 10 has 50+ million lines of code and hundreds of developers that have worked on it
- Various [[#Models]] can assist in helping to eliminate or catch bugs

# Software Development Life Cycle (SDLC)
---
- Organized process of developing a secure applications throughout the life of the project ^f67d9d
- Covers from idea, coding ,testing, deployment, to retirement
- Based on generic [[#Waterfall Model]]

# Waterfall Model

## About
---
- Each project phase is broken into smaller portions and as each is finished you move onto the next ^3b5f48
- Flows from the top down
- Visually looks like a water fall
- Good for <u>complex projects and high levels of security</u>
- But <u>time consuming and not good for rapid deployment and development</u>
- Any changes in requirements would require you to restart
- In stricter waterfall scenarios you can't add new features until the initial product comes out or the cycle finishes

```ad-info
title: Waterfall Model
collapse:close
![[WaterfallModel1.png]]
```

## Phases

### Planning & Analysis
---
- <u>Goals</u> of software are determined
- Needs of stakeholders are assessed
- High level planning
- Rough idea moving towards a formal project

### Software/System Design
---
- Application or system is <u>defined, outlined, and diagramed</u> in detail
- Focus on Input and Output of functions in the final software
- No coding yet

### Implementation
---
- Programmers <u>begin to code</u>
- Basic debugging to ensure functionality along the way
- No formal testing

### Testing
---
- <u>Formal testing</u> via several methods
- Testing programming functionality on its own vs end to end [[#Integration]]

### Integration
---
- App is introduced to the <u>larger environment</u>
	- Possible production environment for testing
	- Limited number of people testing
- App is <u>tested end to end</u> in the network
	- Vs only [[#Testing]] the app on its own
- <u>Ensure all parts can communicate</u> correctly

### Deployment
---
- <u>Placed in production environment</u> and can now be used by all

### Maintenance
---
- Once deployed you need to maintain and release [[Updates and Patches]]
- Educate help desk in order to help end users
- Version Control ^f7f5aa
	- As baseline software is updated, you can <u>use a number sequence to find and identify the newer and older versions</u> of the software ^af2f0a
	- Usually Major, Minor, and build version numbers
		- 1.1.12765, 2.3.13324, etc
- Retired
	- <u>Product is no longer supported</u> and no [[Updates and Patches]] are released ^8ccdc5
	- <u>For CompTia</u> this is part of the [[#Maintenance]] phase but it is common for this to be its own phase in other models
	- #Windows XP is retired and therefore no longer supported
	- Need to <u>develop a migration plan</u> to replace

# Objectives
---
- [[Objectives#2.1 - Explain the importance of security concepts in an enterprise environment|2.1 - Explain the importance of security concepts in an enterprise environment]]
- [[Objectives#2.3 - Summarize secure application development, deployment, and automation concepts|2.3 - Summarize secure application development, deployment, and automation concepts]]

# TODO (Delete when done)
---
- [x] Added vocab
- [x] Added and linked objectives in document
- [ ] Linked objectives back to document
- [ ] Linked any relevant backlinks to and from document