---
tags: [CompTia,SecPlus,CyberSec,Certs]
#aliases:
#cssclass:
#publish:
---

# About
---
- Types
	- [[#Continuous Integration]]
	- [[#Continuous Delivery]]
	- [[#Continuous Deployment]]
- Each change in code should trigger an automated build-and-test sequence
- As automated as possible
- See also [[Software Development#Phases|Software Development Phases]] and [[SDLC Principles]]

```ad-example
title: Traditional Development Process
collapse:close

![[TraditionalDevProc.JPG]]
```

```ad-example
title: CICD Process
collapse:close
![[CICDProc.jpg]]
```

# Traditional Development Workflow

## Process
---
- Develop Code
- Testing
- Integrating
	- Buy new servers and software
- Staging
	- Put new code into servers that operate like the staging environment
- Production
	- Final deployment of software where it is available to all end uses

## Issues
---
- Slow if done linear and in order
- Different stage could be run by different people

# Continuous Integration

## About
---
- Software development method where code updates are tested and committed to a development or build server/code repository rapidly
- Allows you to test and commit updates multiple times a day
- <u>Speeds up development</u>
	- [[#Continuous Deployment]] and [[#Continuous Delivery]] contribute more to this
- <u>Main purpose is to detect and resolve development conflicts early and often</u>

## Process
---
- Using a common source repository that all teams use
- When ready to move on you can take that code and move it onto the CI/CD server
- Code is built, tested, and then reports any success or fails
- Then goes back to developers so that it can move onto the next phase

# Continuous Delivery
---
- Software development method where the application and platform requirements are frequently tested and validated for immediate availability
- Main purpose is to <u>perform automated testing of code in order to get it READY for release</u>
- This makes it ready for potential staging and production
- In order to do [[#Continuous Delivery]] you have to be doing [[#Continuous Integration]] but not vice versa necessarily

# Continuous Deployment
---
- A software development method where application and platform update are committed to production and rapidly
- Place in staging and then move to production at regular intervals
- Main purpose is to <u>perform automated testing and release of code in order to get it INTO the production environment</u> more quickly 

# Objectives
---
- [[Objectives#2.3 - Summarize secure application development, deployment, and automation concepts|2.3 - Summarize secure application development, deployment, and automation concepts]]

# TODO (Delete when done)
---
- [ ] Added vocab
- [ ] Added and linked objectives in document
- [ ] Linked objectives back to document
- [ ] Linked any relevant backlinks to and from document