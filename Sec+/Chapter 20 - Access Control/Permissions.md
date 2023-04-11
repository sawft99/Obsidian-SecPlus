---
tags: [CompTia,SecPlus,CyberSec,Certs]
#aliases:
#cssclass:
#publish:
---

# About
---
- Windows and other operating systems feature [[#Inheritance]] and [[#Propagation]]

# Inheritance
---
- Whenever a new file or folder is created it inherits the permissions from the folder above it 
- Happens by default
- Known as a parent folder and a parent/child relationship
- Any permissions added or removed from the parent folder will pass to the child by default

# Propagation
---
- Occurs when permissions are passed to a subfolder from the parent through [[#Inheritance]]
- Can also refer to when permissions or other changes need to 'propagate' throughout the network and all clients
- If you don't want propagation then [[#Breaking Inheritance]] may be something you want to do

# Breaking Inheritance
---
- Stop permissions from an object such as a folder being inherited to the child object

```ad-example
title: Windows Example
collapse:close
![[WindowsFilePermissionsEx1.png]]
![[WindowsFilePermissionsEx2.png]]
```

# Objectives
---
- [[Objectives#3.8 - Given a scenario, implement authentication and authorization solutions|3.8 - Given a scenario, implement authentication and authorization solutions]]

# TODO (Delete when done)
---
- [ ] Added vocab
- [ ] Added and linked objectives in document
- [ ] Linked objectives back to document
- [ ] Linked any relevant backlinks to and from document