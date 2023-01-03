---
tags: [CompTia,SecPlus,CyberSec,Certs]
#aliases:
#cssclass:
#publish:
---

# About
---
- Structured Query Language
	- The language a web app communicates to a database server to ask for information ^c4ac0f
- SQL Injection
	- A type of [[#Injection Attack]] consisting of the insertion or injection of a SQL query via input data from the client to a web application ^7df86f
- SQL Injection attacks popular because they interact with databases which often contain

# Injection Attack
---
- Insertion of additional information or code through data input from a client to an application ^de8163
- Can occur with any code
- SQL, HTML, XML, and LDAP are common languages but SQL is the most popular

# How SQL Functions
---
- Example
	- Logging into website with username and password and hitting login
	- Website send U/P to database to see if it is correct
	- This lookup is done with a SQL query
	- If the query is correct and returns "true" to the web app, the web app can take its next steps such as logging a user in
	- If the query is not correct then "false" is returned to the web app, the web app can take an action such as prompting again for the correct credentials

```ad-info
title: SQL Query Example
collapse:close
Select any record from the user table in the database where the UID is "Jason" and the pass is "Pass123"

![[SQLQuery1.png]]
```

# A SQL Injection Exmaple
---




# Objectives
---
- [[Objectives#1.3 - Given a scenario, analyze potential indicators associated with application attacks|1.3 - Given a scenario, analyze potential indicators associated with application attacks]]

# TODO (Delete when done)
---
- [ ] Added vocab
- [ ] Added and linked objectives in document
- [ ] Linked objectives back to document
- [ ] Linked any relevant backlinks to and from document