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
	- Columns are often referred to as "Tables"
- SQL Injection
	- A type of [[#Injection Attack]] consisting of the insertion or injection of a SQL query via input data from the client to a web application ^7df86f
- SQL Injection attacks popular because they interact with databases which often contain
	- Databases are critical to websites and web apps

# Injection Attack
---
- Insertion of additional information or code through data input from a client to an application ^de8163
- Can occur with any code
- SQL,HTML, [[XML Vulnerabilities|XML]], and LDAP are common languages but SQL is the most popular

# How SQL Functions - Example
---
- Logging into website with username and password and hitting login
- Website send U/P to database to see if it is correct
- This lookup is done with a SQL query and will look something like
	- select * from Users where user_id = 'jason' and password = pass123
	- Select any record from the user table in the database where the UID is "jason" and the password is "pass123"
- If the query is correct and returns "true" to the web app, the web app can take its next steps such as logging a user in
- If the query is not correct then "false" is returned to the web app, the web app can take an action such as prompting again for the correct credentials

```ad-info
title: SQL Query Example
collapse:close
![[SQLQuery1.png]]
```

# How SQL Injections Function - Example
---
- Instead of entering normal password you might enter something like
	- <u>'`OR 1=1;'</u>
- So the query would look like
	- select * from Users where user_id = 'jason' and <u>password = '`OR 1=1;'</u>
	- Select any record from the user table in the database where the UID is "Jason" and the password is '`OR 1=1;'
- Everything <u>AFTER</u> the single quote (') will be treated as a command
- The difference now is the lookup is asking
	- Does the jason user have a password of 'password' <u>or does 1=1</u>
- Because 1=1 will return a value of "true" the website will then log you in

```ad-info
title: SQL Injection Example
collapse:close
![[SQLInjection1.png]]
```

# SQL Injection - Demos

## Long Explanation/Demo
---

![](https://www.youtube.com/watch?v=ciNHn38EyRc)

## SQLMap Demo
---

![](https://www.youtube.com/watch?v=cx6Xs3F_1Uc)

## Burp Suite Demo
---

![](https://www.youtube.com/watch?v=cyWmZ2WgnEE)

# Mitigating SQL Injections
---
1. Can be prevented with [[SDLC Principles#Never Trust User Input|Input Validation]]
	1. Web app could have detected the escape character and returned an error instead of allowing the code to be sent to the database
2. Use concept of [[SDLC Principles#Least Privilege|Least Privilege]] when accessing

```ad-tip
title: Exam Tip
collapse: close
Generally, if you see any kind of question with the 1=1 statement or something else that would cause an error that returns true, it will be related to an [[#Injection Attack]] or [[SQL Injection]] in some way
```

# Objectives
---
- [[Objectives#1.3 - Given a scenario, analyze potential indicators associated with application attacks|1.3 - Given a scenario, analyze potential indicators associated with application attacks]]